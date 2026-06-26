---
hermes_feed: true
generated_at: 2026-06-26T02:59:23.402826+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T02:59:23.402826+00:00 | окно **72 ч** | сигналов: **4409**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4409 |
| status `skipped` | 4386 |
| status `executed` | 19 |
| status `rejected` | 4 |
| Сопоставлено с реальной сделкой | 57 |
| Вирт. TP (skipped/virtual) | 109 |
| Вирт. SL (skipped/virtual) | 141 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `492feb3f2c4a` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `338b26aa416c` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `3c9f4165331b` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `00825ed7b26b` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `be192c9b533a` **SOXLUSDT** SELL `skipped` conf=0.84 virt=— trail=— real_pnl=
- `587202eac121` **ETHUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `b17babdec939` **ETHUSDT** SELL `skipped` conf=0.91 virt=— trail=— real_pnl=
- `b6014b2631f7` **BTCUSDT** SELL `skipped` conf=0.84 virt=— trail=— real_pnl=
- `9e766548ecf0` **ETHUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `52461a391ab7` **BTCUSDT** SELL `skipped` conf=0.84 virt=— trail=— real_pnl=
- `98952270b00e` **HYPEUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `5a3a62c081c1` **BTCUSDT** SELL `skipped` conf=0.88 virt=— trail=— real_pnl=
- `a97409a65925` **BTCUSDT** SELL `skipped` conf=0.88 virt=— trail=— real_pnl=
- `4b61ca0a75e6` **BTCUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `9f7d813d04bb` **SOXLUSDT** SELL `skipped` conf=0.83 virt=— trail=— real_pnl=
