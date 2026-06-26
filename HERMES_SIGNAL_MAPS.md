---
hermes_feed: true
generated_at: 2026-06-26T08:59:27.237599+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-26T08:59:27.237599+00:00 | окно **72 ч** | сигналов: **4291**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4291 |
| status `skipped` | 4267 |
| status `executed` | 21 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 69 |
| Вирт. TP (skipped/virtual) | 148 |
| Вирт. SL (skipped/virtual) | 157 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `869b8efc3710` **SOLUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `6faf743d8b5e` **BTCUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `a3aee3737627` **ETHUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `392ea1251839` **SOLUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `fad9cac7ef5e` **ETHUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `739882d9f522` **SOLUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `0b2fee1e1fe4` **BTCUSDT** BUY `skipped` conf=0.88 virt=— trail=— real_pnl=
- `173ffa37fef3` **ETHUSDT** BUY `skipped` conf=0.92 virt=— trail=— real_pnl=
- `fa5201fc73dd` **SOLUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `3241a6ba6b11` **ETHUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `3529cd03ff87` **SOLUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `8fdf399c2feb` **ETHUSDT** BUY `skipped` conf=0.89 virt=— trail=— real_pnl=
- `ade673c198d6` **ETHUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `394749a57e4d` **ETHUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `20896f6b08ad` **SLXUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
