# Cherry Picking

- ## When we want to have a specific commit from an other branch
- ## It can happen when we are on the `'master'` branch or on an other `'feature'` branch and we need/want a specific commit from an other branch.

## 1. Cherry Pick

```bash
# 1. Find the hash of the commit we need from whatever branch we want

# 2. cherry-pick it
git cherry-pick '<COMMIT-HASH>'
```
