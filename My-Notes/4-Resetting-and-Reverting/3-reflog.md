# Reflog

## Needed when accidentally made HARD reset

## 1. git reflog

```bash
# accident
git reset --hard HEAD~1

# take a breath :)
# look at the history
git reflog

# look in 'reflog' for the action we accidentally made
git reset --hard '<COMMIT-HASH>'

```
