---
hermes_feed: true
generated_at: 2026-06-25T08:59:08.657323+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T08:59:08.657323+00:00 | окно **72 ч** | сигналов: **4904**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4904 |
| status `skipped` | 4881 |
| status `executed` | 20 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 60 |
| Вирт. TP (skipped/virtual) | 89 |
| Вирт. SL (skipped/virtual) | 99 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `35a79004a5ef` **BTCUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `73a4eaf1da02` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `7dc7561843b7` **SOLUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `52e07e2244da` **BTCUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `d8b136551a4d` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `cd1fd57b8458` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `ffe7ccc56240` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `248a000c5939` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `a6ead3385f15` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `2b9ffebe5ea8` **ETHUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `009255d70f9e` **BTCUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `808da0f10f10` **ETHUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `373fb0fd4710` **BTCUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `01f5c137ca0a` **ETHUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `ff2d54a80157` **BTCUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
