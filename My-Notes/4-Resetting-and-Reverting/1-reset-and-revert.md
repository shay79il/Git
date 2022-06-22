# Resetting and Reverting

## Mostly needed when we made a mistake commit

## 1. Revert

```bash
# We use 'revert' when we want to save the revert history
git revert '<COMMIT-HASH>'
```

## 1. Reset

```bash
# soft reset - which means keeping the changes made
git reset --soft HEAD~1
# Or
git reset --soft '<COMMIT-HASH>'

# hard reset - which means loosing the changes made
git reset --hard HEAD~1
# Or
git reset --hard '<COMMIT-HASH>'

```
