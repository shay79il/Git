# Cloning remote repositories

> ## Make sure to upload to the remote repo a public SSH-KEY

## 1. Clone remote repo

```bash
git clone git@github.com:shay79il/Git.git
```

### 2. List remote repo

```bash
git remote -v
```

### 3. Remove remote repo

```bash
git remote rm origin
```

### 3. Git push

```bash
git push origin main
```

### 4. Git push to non-created remote repo

```bash
git push --set-upstream origin <branchName>
```
