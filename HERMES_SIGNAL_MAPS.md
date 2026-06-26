---
hermes_feed: true
generated_at: 2026-06-26T11:59:37.889604+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T11:59:37.889604+00:00 | окно **72 ч** | сигналов: **4422**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4422 |
| status `skipped` | 4397 |
| status `executed` | 22 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 73 |
| Вирт. TP (skipped/virtual) | 147 |
| Вирт. SL (skipped/virtual) | 151 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `c875308fe402` **BTCUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `5a0bf10f664e` **SOLUSDT** SELL `skipped` conf=0.91 virt=— trail=take_profit real_pnl=
- `17e66a9a0ed2` **BTCUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `23f20b886b0f` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `1df07b95ecf7` **HYPEUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `274f031e1721` **SOLUSDT** SELL `skipped` conf=0.93 virt=— trail=take_profit real_pnl=
- `1c77197290c2` **BTCUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `626eba437c66` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `50bb53050c61` **HYPEUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `485ad139860b` **SOLUSDT** SELL `skipped` conf=0.94 virt=— trail=take_profit real_pnl=
- `028e6b136af7` **ETHUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `391521b3bb53` **BTCUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `f952df420b10` **SOXLUSDT** SELL `skipped` conf=0.82 virt=— trail=— real_pnl=
- `0d3619bdd622` **HYPEUSDT** SELL `skipped` conf=0.95 virt=— trail=— real_pnl=
- `b3f90f8d1062` **SOLUSDT** SELL `executed` conf=0.93 virt=— trail=take_profit real_pnl=
