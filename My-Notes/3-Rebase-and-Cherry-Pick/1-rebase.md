# Rebase

- ## Instead of merging from `'master'` ==>> Rebase!
- ## When we want to squash our previous commits on our branch

## 1. Rebase

```bash
# 1. checkout feature-branch to work on
git checkout feature-branch

# 2. rebase from master to be aligned
git rebase master

# 3. Create PR-pull request :)
```

## 2. Change commit history on a branch

```bash
# rebase last 4 commits
git rebase -i HEAD~4
```
