# Hermes → Cursor (живой брифинг)

Репозиторий-синхронизатор для [PRD-BOT](https://github.com/gogi-eng/PRD-BOT-03-26).

Сервер **AGENT-WORLD** публикует сюда рекомендации Hermes.  
На **любом ПК** с Cursor — `git pull` и копия в `.cursor/HERMES_LIVE.md`.

## Файлы

| Файл | Назначение |
|------|------------|
| `HERMES_LIVE.md` | Главный брифинг для агента Cursor |
| `winning_entry_rules_report.md` | Полный отчёт |
| `winning_entry_rules.json` | JSON для скриптов |
| `hermes_cursor_feed.jsonl` | История обновлений |
| `meta.json` | Время и источник последней публикации |

## На сервере (один раз)

```bash
cd /root
git clone https://github.com/gogi-eng/Analise_Hermes.git
cd /root/AGENT-WORLD
export HERMES_GITHUB_DIR=/root/Analise_Hermes
./venv/bin/python3 scripts/hermes_cursor_feed.py --hours 336 --git-clone --git-push
```

Постоянно (systemd `hermes-cursor-feed`):

```bash
export HERMES_GITHUB_DIR=/root/Analise_Hermes
./venv/bin/python3 scripts/hermes_cursor_feed.py --watch --interval 120 --git-clone --git-push --github-only --hours 336
```

На сервере нужен **deploy key** или **Personal Access Token** для `git push` в этот репозиторий.

## На любом ПК с Cursor

```bash
# рядом с папкой PRD-BOT
git clone https://github.com/gogi-eng/Analise_Hermes.git
cd PRD-BOT-ALL
powershell -ExecutionPolicy Bypass -File scripts/hermes_sync_from_github.ps1
```

Авто каждые 5 мин (Windows):

```powershell
powershell -ExecutionPolicy Bypass -File scripts/hermes_sync_from_github.ps1 -InstallTask
```

Или добавьте папку `Analise_Hermes` в workspace Cursor — агент читает `HERMES_LIVE.md` напрямую.

## Правило ZeroOne

Hermes **не меняет** config и **не ставит** ордера. Максимум **одна** правка за сессию — только по вашей просьбе.
