---
hermes_feed: true
generated_at: 2026-06-27T06:00:15.785945+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-27T06:00:15.785945+00:00 | окно **72 ч** | сигналов: **5205**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 5205 |
| status `skipped` | 5162 |
| status `executed` | 31 |
| status `rejected` | 12 |
| Сопоставлено с реальной сделкой | 110 |
| Вирт. TP (skipped/virtual) | 134 |
| Вирт. SL (skipped/virtual) | 144 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `7559a4eb0ac3` **LABUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `ade9acc5ec32` **LABUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `9cdaf73704c4` **LABUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `b74e28b6eac1` **LABUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `3c40bd600d31` **LABUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `344749c2cb6f` **LABUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `98a35cd14a77` **LABUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `4f47cfed236e` **LABUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `e03dd64c8ac4` **LABUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `51c30a2ab575` **LABUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `4b6b225c3b54` **LABUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `52dd6f8adfd6` **LABUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `a0b2b050a05a` **AGLDUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `0466e56df2ea` **LABUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `72218b4d1d74` **AGLDUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
