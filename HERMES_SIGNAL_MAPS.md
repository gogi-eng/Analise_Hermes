---
hermes_feed: true
generated_at: 2026-06-26T05:59:25.904133+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T05:59:25.904133+00:00 | окно **72 ч** | сигналов: **4329**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4329 |
| status `skipped` | 4305 |
| status `executed` | 21 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 77 |
| Вирт. TP (skipped/virtual) | 125 |
| Вирт. SL (skipped/virtual) | 152 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `7dec28db1a6d` **SOLUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `64e6c57d13a4` **BTCUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `e629e2299f52` **SLXUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `2ea8eb01fc08` **SOLUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `7794983a5a04` **BTCUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `05bb23ef1c25` **SOLUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `6ecea86114ef` **BTCUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `c2855f38414c` **BTCUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `913d5cd09e22` **BTCUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `615024f47139` **BTCUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `5c6db0dc52ae` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `92a3d6b4b954` **LABUSDT** BUY `skipped` conf=0.84 virt=— trail=— real_pnl=
- `c62e9c6c6b46` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `6f291931b4da` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `3c21a9c55968` **BTCUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
