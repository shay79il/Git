# Git Merge

## When we want to merge 2 branches into 1

## Usually we will merge into `'main'` branch

### 1. git checkout main

```bash
# Checkout main
git checkout main
git merge feature1
```

- ## fast-forward merge
  - is when the current branch has **no extra** commits compare to the branch we want to merge **from**
  - meaning we will see all commits from the 'other' branch on the timeline of the 'master' branch
- ## **no**-fast-forward merge
  - is when the current branch has **extra** commits compare to the branch we want to merge **from**
  - meaning we will see **first** all **master** commits on the 'master' log timeline and next all commits from the branch we are merging from
