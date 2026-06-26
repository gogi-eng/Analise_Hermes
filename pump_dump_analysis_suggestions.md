# Анализ признаков пампов/дампов и предложения по улучшению сканера PRD-BOT

## Введение
Данный документ предназначен для сбора и систематизации информации о потенциальных признаках пампов и дампов на крипторынке, а также для формулирования предложений по совершенствованию встроенного сканера PRD-BOT.

## Наблюдаемые признаки (для исследования)
Предварительный список признаков, которые могут указывать на пампы или дампы:

*   **Резкий рост/падение объема торгов:** Значительное отклонение текущего объема от среднего за определенный период (например, 5m, 15m, 1h, 4h, 24h).
*   **Резкое изменение цены:** Быстрый и неестественный рост или падение цены без очевидных фундаментальных причин.
*   **Изменение рыночной глубины (Order Book Depth):** Внезапное появление/исчезновение крупных лимитных ордеров, указывающее на манипуляции.
*   **Соотношение Buy/Sell Ratio:** Резкое преобладание покупателей или продавцов.
*   **Финансирование (Funding Rate) на фьючерсах:** Аномальные значения Funding Rate могут указывать на дисбаланс позиций и возможное "выдавливание" определенных позиций.
*   **Открытый интерес (Open Interest):** Резкий рост или падение Open Interest на фьючерсах.
*   **Активность в социальных сетях/новостях:** Внезапное увеличение упоминаний актива в медиа, особенно в сочетании с аномальным движением цены.

## Связь с текущим сканером PRD-BOT
Текущий сканер PRD-BOT уже анализирует некоторые параметры, такие как `intraday_range_pct` (price movement) и `volume_ratio` (volume change). Он также использует `external_sentiment.coinugget_style.volume_spike_mult` и имеет секцию `pump_dump_trade`.
Модуль `analysis/market_structure.py` уже содержит логику `volume_spike`, `spread_expansion` и `momentum_confirmed` для выявления сильных движений цены и объема.
Функция `market_scanner_bos_confirmed` в `telegram_agent/market_scanner_levels.py` подтверждает пробой `BOS` уровня для сценариев `PUMP`/`DUMP`.
Функция `analyze_spike_setup` в `telegram_agent/pump_dump_spike_scan.py` отвечает за окончательное определение `scenario` (PUMP/DUMP) и `spike_mode` на основе `min_move_pct` и `min_volume_ratio`.

## Предложения по совершенствованию сканера (план исследования)

### 1. Более Чувствительное и Адаптивное Обнаружение Пампов/Дампов:

*   **Использование `MarketStructure.momentum_confirmed` для активации `spike_mode`:**
    *   **Текущая логика:** В `pump_dump_spike_scan.py` `scenario` и `spike_mode` определяются на основе `candle_move_pct` и `volume_ratio` последней свечи.
    *   **Предложение:** Модифицировать функцию `analyze_spike_setup` (или добавить дополнительную логику в `_analyze_spike_setup` в `telegram_signal_agent.py`) так, чтобы **интегрировать `MarketStructure.momentum_confirmed`**. Если `momentum_confirmed` (объединяющий `volume_spike` и `spread_expansion` из `MarketStructureEngine`) является `True`, это должно служить дополнительным или основным критерием для установки `spike_mode=True` и `scenario="PUMP"/"DUMP"`. Это объединит сигналы от анализа рыночной структуры с прямым обнаружением свечных импульсов.
    *   **Обоснование:** `momentum_confirmed` уже учитывает как объем, так и диапазон свечи, что делает его более надежным индикатором сильного движения, чем просто `move_pct > min_move_pct`.

*   **Динамическая настройка `min_move_pct` и `min_volume_ratio`:**
    *   **Текущая логика:** `pump_dump_spike_scan.py` использует фиксированные `min_move_pct: 3.0` и `min_volume_ratio: 1.25` (по умолчанию).
    *   **Предложение:** Вместо фиксированных порогов, рассмотреть возможность использования **адаптивных порогов**, основанных на:
        *   **Волатильности рынка:** Например, `min_move_pct` может быть кратным текущему ATR.
        *   **Стандартных отклонениях:** `min_volume_ratio` может быть рассчитан как N стандартных отклонений от среднего объема за длительный период.
    *   **Дополнение:** Создать пресеты для памп/дамп стратегии в `config.yaml` с различными, более чувствительными `pump_dump_trade.min_move_pct_aggressive` или `pump_dump_trade.min_volume_ratio_aggressive` для разных условий рынка.

*   **Добавление "скорости" изменения цены (`Price Change Acceleration`):**
    *   **Предложение:** В `pump_dump_spike_scan.py` добавить вычисление **скорости изменения цены** (например, `move_pct` на меньших таймфреймах, если возможно, или дельта `move_pct` за N свечей) и использовать это как дополнительный фактор скоринга в `compute_spike_score`. Пампы/дампы часто характеризуются ускоряющейся динамикой, а не просто большим `move_pct` одной свечи.

### 2. Улучшенное Скоринг и Классификация Пампов/Дампов:

*   **Распределение скора в `compute_spike_score`:**
    *   **Предложение:** Добавить в `compute_spike_score` бонусные очки, если `MarketStructure.momentum_confirmed` (полученное от `MarketStructureEngine`) является `True`. Это позволит сигналам с подтвержденным моментумом получать более высокий скор.
    *   **Предложение:** Пересмотреть систему бонусов так, чтобы экстремальные значения `move_pct` (значительно выше `min_move_pct`) получали экспоненциально больший бонус, а не линейный (`bump = min(24, int(max(0.0, excess) * 4.0))`).

*   **Разделение скоров для пампов/дампов:**
    *   **Предложение:** Возможно, стоит ввести отдельный "памп/дамп" скор, который будет рассчитываться по более агрессивным правилам и не будет ограничен `market_scanner_max_range_pct` (6.5%) сверху, так как пампы по своей природе могут давать гораздо больший `range_pct`.

### 3. Интеграция с секцией `pump_dump_trade` в `config.yaml`:

*   **Текущая логика:** Если `pump_dump_trade.enabled` `True` и сигнал `is_pump_dump_signal` `True`, то применяются более широкие `entry_drift_limits`.
*   **Предложение:** Добавить в секцию `pump_dump_trade` в `config.yaml` параметры, управляющие стратегией входа/выхода специально для памп/дамп сигналов, например:
    *   `pump_dump_trade.aggressive_tp_rr_mult`: Множитель для более агрессивного TP.
    *   `pump_dump_trade.fast_entry_mode`: Флаг для использования market-ордеров с более высоким допуском проскальзывания.
    *   `pump_dump_trade.min_momentum_confirmed_score`: Минимальный скор `momentum_confirmed` для активации памп/дамп режима.

## План по реализации изменений кода (High-Level):

### A. Изменения в `telegram_signal_agent.py`:

1.  **Импортировать `MarketStructureEngine`** из `analysis.market_structure`.
2.  **Добавить `self._structure_engine = MarketStructureEngine(...)` в `TelegramSignalAgent.__init__`**: 
    *   Параметры `volume_spike_mult` и `spread_expansion_mult` для `MarketStructureEngine` будут взяты из `config.yaml`. 
    *   `(Ремарка: в `config.yaml` эти параметры как раз в `external_sentiment.coinugget_style.volume_spike_mult` и нет `spread_extension_mult`.) Необходимо будет выбрать, какие использовать или добавить новые.`
3.  **Модифицировать `_analyze_spike_setup`**: 
    *   Вычислить `atr_value` из `klines` (или передать его из вызывающей функции, если он уже доступен).
    *   Вызвать `structure = self._structure_engine.analyze(klines, atr_value)`.
    *   Передать `structure.momentum_confirmed` (и, возможно, `structure.volume_spike`, `structure.spread_expansion`) как новый параметр в `analyze_spike_setup`.

### B. Изменения в `telegram_agent/pump_dump_spike_scan.py`:

1.  **Модифицировать `analyze_spike_setup`**: 
    *   Добавить новый параметр `momentum_confirmed: bool = False`.
    *   Использовать этот флаг для:
        *   **Усиления определения `scenario`**: Если `momentum_confirmed` True, это может быть достаточным условием для установки `scenario="PUMP"` или `"DUMP"`, даже если `candle_move_pct` не достиг `min_move_pct`.
        *   **Бонусов в `compute_spike_score`**: Добавить бонусные очки, если `momentum_confirmed` True.

## Следующие шаги
Я начну с фактического изучения `telegram_signal_agent.py` и его `__init__` метода, чтобы определить наилучшее место для инстанцирования `MarketStructureEngine` и получения `volume_spike_mult` и `spread_expansion_mult` из `config.yaml`.
