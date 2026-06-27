---
hermes_feed: true
generated_at: 2026-06-27T03:00:11.559237+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-27T03:00:11.559237+00:00 | окно **72 ч** | сигналов: **5096**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 5096 |
| status `skipped` | 5053 |
| status `executed` | 31 |
| status `rejected` | 12 |
| Сопоставлено с реальной сделкой | 110 |
| Вирт. TP (skipped/virtual) | 134 |
| Вирт. SL (skipped/virtual) | 130 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `6c40ffe0b8df` **AAVEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `ce813011452c` **AAVEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `c2e7ca28f471` **AAVEUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `d9a50fa62dff` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `21b6591d651b` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `1e13595f0c37` **AAVEUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `92d93ad6cbdd` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `33658d6b8227` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `49876388c4a1` **AAVEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `e985a1e5c213` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `15b7e03fc6e9` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `5f6333c97e64` **AAVEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `9514bf2eaecc` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `4331e6ea2d33` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `57525fc2ec1a` **AAVEUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
