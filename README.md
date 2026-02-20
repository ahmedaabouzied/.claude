# Claude Code Configuration

Portable Claude Code configs tracked via git.

## What's tracked

| Path | Purpose |
|------|---------|
| `settings.json` | Global settings (plugins, preferences) |
| `agents/` | Custom agent definitions |
| `skills/` | Custom skills |
| `projects/*/CLAUDE.md` | Per-project instructions |
| `projects/*/memory/` | Per-project memory files |

## Setup on a new machine

```bash
# Clone into ~/.claude (must be empty or non-existent)
git clone <your-remote-url> ~/.claude

# Or if ~/.claude already exists:
cd ~/.claude
git init
git remote add origin <your-remote-url>
git fetch
git checkout main
```

Everything else (history, caches, telemetry, session data) is gitignored and will be regenerated locally.
