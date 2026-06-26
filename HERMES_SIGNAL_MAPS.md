---
hermes_feed: true
generated_at: 2026-06-26T17:59:58.755600+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T17:59:58.755600+00:00 | окно **72 ч** | сигналов: **4856**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4856 |
| status `skipped` | 4822 |
| status `executed` | 28 |
| status `rejected` | 6 |
| Сопоставлено с реальной сделкой | 93 |
| Вирт. TP (skipped/virtual) | 132 |
| Вирт. SL (skipped/virtual) | 154 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `7d053f9f947b` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `26ea459ddb16` **SOLUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `c419c04c27e5` **AAVEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `57ac537d91bd` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `f5b1b87d1d1d` **SOLUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `da2ab8f90ca4` **HYPEUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `ae74e2ddbc87` **ETHUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `612ce68c22c8` **SOLUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `c0a11e886a6f` **HYPEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `c3789be2835b` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `d1d43569bc3a` **SOLUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `00992a81d236` **HYPEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `c933df78d78c` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `481c7e237ad0` **SOLUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `8387cedb9eba` **HYPEUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
