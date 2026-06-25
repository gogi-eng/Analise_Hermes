---
hermes_feed: true
generated_at: 2026-06-25T11:59:11.065392+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T11:59:11.065392+00:00 | окно **72 ч** | сигналов: **4980**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4980 |
| status `skipped` | 4958 |
| status `executed` | 19 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 58 |
| Вирт. TP (skipped/virtual) | 89 |
| Вирт. SL (skipped/virtual) | 98 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `b704a2fa140a` **HYPEUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `67820b88c61e` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `a398d2797600` **SOLUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `4e73f16761ee` **HYPEUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `f73819d0d5c2` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `768a67cd4a1c` **BTCUSDT** SELL `skipped` conf=0.90 virt=— trail=— real_pnl=
- `e4fc692d395c` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `9548b54a18d1` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `110861f4aea3` **HYPEUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `e5289081aec8` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `a01131104ac1` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `1ffc98b5654c` **ETHUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `2c2e471af08f` **BTCUSDT** SELL `skipped` conf=0.90 virt=— trail=— real_pnl=
- `04ec40c49862` **ETHUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `7f0bf6816ef2` **BTCUSDT** SELL `skipped` conf=0.90 virt=— trail=— real_pnl=
