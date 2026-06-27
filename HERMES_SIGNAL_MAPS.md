---
hermes_feed: true
generated_at: 2026-06-27T00:00:10.392455+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-27T00:00:10.392455+00:00 | окно **72 ч** | сигналов: **5009**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 5009 |
| status `skipped` | 4968 |
| status `executed` | 29 |
| status `rejected` | 12 |
| Сопоставлено с реальной сделкой | 95 |
| Вирт. TP (skipped/virtual) | 134 |
| Вирт. SL (skipped/virtual) | 155 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `5ad77723ad61` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `1baaaea40070` **ETHUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `52528178dff9` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `5d4c1e42a69e` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `b77934b0db6a` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `c297a47a8b7f` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `2a512f17b764` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `2404f6583049` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `a87f8df225bc` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `5853bad85b89` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `423425e6e435` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `fb672eabc635` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `9271cc1b6c2c` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `bc13ba141ecc` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `c9e5d3945f08` **BTCUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
