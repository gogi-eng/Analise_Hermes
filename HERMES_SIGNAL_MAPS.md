---
hermes_feed: true
generated_at: 2026-06-25T23:59:21.446834+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T23:59:21.446834+00:00 | окно **72 ч** | сигналов: **4475**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4475 |
| status `skipped` | 4453 |
| status `executed` | 18 |
| status `rejected` | 4 |
| Сопоставлено с реальной сделкой | 56 |
| Вирт. TP (skipped/virtual) | 129 |
| Вирт. SL (skipped/virtual) | 145 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `1b5e455ee27a` **SOLUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `ffa8cb746f06` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `c8be9bf0bb5c` **SOLUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `ff3b53f106e0` **BTCUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `b1e0508b1f45` **SOLUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `def49021d702` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `4d820af4ccd3` **BTCUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `b84135fa74e2` **HYPEUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `8985331ee6c0` **AAVEUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `fa91b8255be0` **AAVEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `244ebf1dd113` **AAVEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `2047950c7f43` **AAVEUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `023a62af23ab` **AAVEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `6b0bce7ce03c` **AAVEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `87ba1f2b7b89` **AAVEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
