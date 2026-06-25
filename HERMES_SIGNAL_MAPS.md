---
hermes_feed: true
generated_at: 2026-06-25T14:59:12.615919+00:00
source: PRD-BOT-ALL
lookback_hours: 72.0
---

# HERMES — карты сигналов (исполнение)

> **Для Hermes / Cursor:** полные карты — `hermes_signal_maps.jsonl` (одна строка = один сигнал).
> Бот пишет **все** сигналы в `signal_ledger`; виртуальный исход — для пропущенных; реальный PnL — для открытых.

**Обновлено:** 2026-06-25T14:59:12.615919+00:00 | окно **72 ч** | сигналов: **4998**

## Сводка

| Метрика | Значение |
|---------|----------|
| Всего сигналов | 4998 |
| status `skipped` | 4978 |
| status `executed` | 17 |
| status `rejected` | 3 |
| Сопоставлено с реальной сделкой | 54 |
| Вирт. TP (skipped/virtual) | 106 |
| Вирт. SL (skipped/virtual) | 118 |

## Структура карты (JSONL)

Поля: `entry_params` (индикаторы, стакан), `price_movement` (MFE/MAE, свечи),
`virtual_sl_tp`, `virtual_trailing` (если бы трейлинг работал), `real_trade` (+/−).

## Последние 15 сигналов

- `5e64f96cf5fd` **SOLUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `94d93fb4f323` **ETHUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `ecc80e8f29de` **DOGEUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `2bad781a757f` **HYPEUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `82d555b957ec` **MUUSDT** SELL `skipped` conf=0.91 virt=— trail=— real_pnl=
- `50638da62865` **ZECUSDT** SELL `skipped` conf=0.90 virt=— trail=— real_pnl=
- `4a9a1a106b0e` **ZECUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `e384fb24c1be` **ZECUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `8f8149dd8467` **ZECUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `302c44d3647c` **ZECUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `3266da4dadbf` **ZECUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `0c61781ffa71` **ZECUSDT** SELL `skipped` conf=0.89 virt=— trail=— real_pnl=
- `1407a89bf0cd` **MUUSDT** SELL `skipped` conf=0.93 virt=— trail=— real_pnl=
- `d26c83156f0f` **MUUSDT** SELL `skipped` conf=0.94 virt=— trail=— real_pnl=
- `156c0f2deddb` **MUUSDT** SELL `skipped` conf=0.88 virt=— trail=— real_pnl=
