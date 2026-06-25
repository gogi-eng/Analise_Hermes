---
hermes_feed: true
generated_at: 2026-06-25T17:59:18.284615+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T17:59:18.284615+00:00 | окно **72 ч** | сигналов: **4718**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4718 |
| status `skipped` | 4697 |
| status `executed` | 18 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 55 |
| Вирт. TP (skipped/virtual) | 124 |
| Вирт. SL (skipped/virtual) | 123 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `e384fb24c1be` **ZECUSDT** SELL `skipped` conf=0.93 virt=still_open trail=— real_pnl=
- `8f8149dd8467` **ZECUSDT** SELL `skipped` conf=0.93 virt=still_open trail=— real_pnl=
- `302c44d3647c` **ZECUSDT** SELL `skipped` conf=0.89 virt=stop_loss trail=— real_pnl=
- `3266da4dadbf` **ZECUSDT** SELL `skipped` conf=0.89 virt=still_open trail=— real_pnl=
- `0c61781ffa71` **ZECUSDT** SELL `skipped` conf=0.89 virt=still_open trail=— real_pnl=
- `1407a89bf0cd` **MUUSDT** SELL `skipped` conf=0.93 virt=still_open trail=— real_pnl=
- `d26c83156f0f` **MUUSDT** SELL `skipped` conf=0.94 virt=stop_loss trail=— real_pnl=
- `156c0f2deddb` **MUUSDT** SELL `skipped` conf=0.88 virt=still_open trail=— real_pnl=
- `dff0090bac96` **ETHUSDT** SELL `skipped` conf=0.89 virt=still_open trail=— real_pnl=
- `41ea472358fa` **ETHUSDT** SELL `skipped` conf=0.88 virt=still_open trail=— real_pnl=
- `fe4efad3f886` **LABUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
- `84b60c39c5b0` **SOXLUSDT** SELL `skipped` conf=0.92 virt=— trail=— real_pnl=
- `1442947ed7ac` **LABUSDT** BUY `executed` conf=0.92 virt=— trail=stop_loss real_pnl=
- `71e59b540b8c` **MUUSDT** BUY `skipped` conf=0.90 virt=— trail=— real_pnl=
- `2620f47fb1f3` **MUUSDT** BUY `skipped` conf=0.91 virt=— trail=— real_pnl=
