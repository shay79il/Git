# Stashing

## Mostly needed when we want to save current state of work in progress which is **not** done and go to another brach to work on

## 1. Stash

```bash
# enter WIP into stash
git stash

# Pop WIP from stash
git stash pop
```

## 2. Stash list

```bash
git stash list
```

## 3. Stash show

```bash
# show a specific stashed state
git stash show stash@{1}
```

## 4. Stash specific pop

```bash
git stash pop stash@{1}
```
