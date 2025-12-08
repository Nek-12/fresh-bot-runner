# fresh-bot-runner

Personal GitHub Actions runner for [c-hive/fresh-bot](https://github.com/c-hive/fresh-bot). The workflow runs daily and replies to stale bot warnings on issues you're subscribed to.

## Setup

1. Create a classic Personal Access Token with `repo` scope (covers public repos too).
2. Add it as a secret named `PERSONAL_ACCESS_TOKEN` in this repository.
3. Watch the repositories whose issues you want kept alive (set "All activity"):
   - `anthropics/claude-code`
   - `InsertKoinIO/koin`

The scheduled workflow (`.github/workflows/fresh-bot.yml`) runs at 01:00 UTC daily. You can also trigger it manually via `workflow_dispatch`.
