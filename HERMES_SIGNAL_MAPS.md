---
hermes_feed: true
generated_at: 2026-06-26T14:59:49.029005+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T14:59:49.029005+00:00 | окно **72 ч** | сигналов: **4655**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4655 |
| status `skipped` | 4626 |
| status `executed` | 25 |
| status `rejected` | 4 |
| Сопоставлено с реальной сделкой | 89 |
| Вирт. TP (skipped/virtual) | 149 |
| Вирт. SL (skipped/virtual) | 152 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `21d8ed479d54` **BTCUSDT** BUY `skipped` conf=0.92 virt=— trail=stop_loss real_pnl=
- `7284d7ea369a` **ETHUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `413675626c03` **BTCUSDT** BUY `executed` conf=0.94 virt=— trail=stop_loss real_pnl=
- `4546e2178e2e` **ETHUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `4a9bbd998848` **HYPEUSDT** BUY `skipped` conf=0.85 virt=— trail=— real_pnl=
- `df2acf574b4f` **SOLUSDT** BUY `skipped` conf=0.85 virt=— trail=— real_pnl=
- `83808421c005` **AAVEUSDT** BUY `rejected` conf=0.85 virt=— trail=— real_pnl=
- `e334be1152a0` **ZECUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `8c49cfc356f3` **ZECUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `520508770a84` **ZECUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `2f070ee2b3ff` **ZECUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `13ff93dcce18` **ZECUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `ab46d0d73f8d` **ZECUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `58122e55ed00` **SOXLUSDT** SELL `skipped` conf=0.88 virt=— trail=— real_pnl=
- `64c2720c12a5` **AAVEUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
