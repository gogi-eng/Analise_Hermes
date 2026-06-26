---
hermes_feed: true
generated_at: 2026-06-26T21:00:00.071927+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T21:00:00.071927+00:00 | окно **72 ч** | сигналов: **4946**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4946 |
| status `skipped` | 4906 |
| status `executed` | 29 |
| status `rejected` | 11 |
| Сопоставлено с реальной сделкой | 95 |
| Вирт. TP (skipped/virtual) | 135 |
| Вирт. SL (skipped/virtual) | 134 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `b12e1e02ffd7` **BTCUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `1ee518196ca5` **SOXLUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `1bf7e090ad98` **BTCUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `603c3ac30421` **SOXLUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `3a6dcb8c7bcb` **BTCUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `137726fbc8d1` **SOXLUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `2827aadf8787` **BTCUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `c9840ec57f62` **SOXLUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `5fc0c7f9fa04` **BTCUSDT** SELL `skipped` conf=0.90 virt=— trail=— real_pnl=
- `ff081991ad6f` **SOXLUSDT** SELL `rejected` conf=0.95 virt=— trail=— real_pnl=
- `5f02ff9b65c8` **BTCUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `e2f553324b91` **BTCUSDT** SELL `skipped` conf=0.91 virt=— trail=— real_pnl=
- `de10a210dfe4` **BTCUSDT** SELL `skipped` conf=0.91 virt=— trail=— real_pnl=
- `45a0146a9a82` **BTCUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `64fd57fb0524` **BTCUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
