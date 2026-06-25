---
hermes_feed: true
generated_at: 2026-06-25T20:59:19.964217+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T20:59:19.964217+00:00 | окно **72 ч** | сигналов: **4608**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4608 |
| status `skipped` | 4588 |
| status `executed` | 16 |
| status `rejected` | 4 |
| Сопоставлено с реальной сделкой | 53 |
| Вирт. TP (skipped/virtual) | 128 |
| Вирт. SL (skipped/virtual) | 140 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `51e2521ee4ed` **HYPEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `c9d3060a6ede` **HYPEUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `10eca5ca05b1` **HYPEUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `1e694f2985d0` **HYPEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `0174dea674ff` **HYPEUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `b23405b508db` **HYPEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `6121ae1cec12` **HYPEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `0426392e6251` **HYPEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `403df8bcac14` **HYPEUSDT** BUY `skipped` conf=0.95 virt=— trail=— real_pnl=
- `d6fafbf9c827` **HYPEUSDT** BUY `skipped` conf=0.94 virt=— trail=— real_pnl=
- `4bb3030571b2` **HYPEUSDT** BUY `skipped` conf=0.93 virt=— trail=— real_pnl=
- `11ea16cdda0d` **HYPEUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `f0fc124a278b` **HYPEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `10a36f515cff` **HYPEUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `f1dc21bc04b2` **HYPEUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
