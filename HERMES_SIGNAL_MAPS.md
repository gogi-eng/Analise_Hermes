---
hermes_feed: true
generated_at: 2026-06-25T05:59:06.536951+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T05:59:06.536951+00:00 | окно **72 ч** | сигналов: **4648**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4648 |
| status `skipped` | 4626 |
| status `executed` | 19 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 41 |
| Вирт. TP (skipped/virtual) | 89 |
| Вирт. SL (skipped/virtual) | 101 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `491d00d308d9` **SOLUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `a6499b6844bb` **ETHUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `4170afabf0dc` **AAVEUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `6f1a4bbf8bcd` **BTCUSDT** BUY `skipped` conf=0.87 virt=— trail=— real_pnl=
- `31835f16403b` **AAVEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `931214cb20df` **AAVEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `f66e4960f6ad` **AAVEUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `1edf28e60971` **BTCUSDT** SELL `executed` conf=0.85 virt=— trail=— real_pnl=
- `8e2629161f26` **ETHUSDT** SELL `executed` conf=0.85 virt=— trail=— real_pnl=
- `bd37f5998f96` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `9fb15b1634f9` **AAVEUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `5b2edfad98bd` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `368db464bab6` **BTCUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `c609cef09279` **ETHUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `9a0e5f4c5a4b` **HUSDT** SELL `skipped` conf=0.92 virt=— trail=— real_pnl=
