# Git Branches

## Working on a project in a separate version can be done by git branch which **points** to a **certain** commit in time

### 1. git checkout -b feature1

```bash
# Create a new branch on git and check it out
git checkout -b feature1

# output
Switched to a new branch 'feature1'
```

### 2. git branch

```bash
# List all branches
git branch

# Output
* feature1 # Active branch!!
  main
```

### 3. git checkout <branch-name>

```bash
# Switch to main branch
git checkout main
```

### 4. git branch -d <branch-name>

```bash
# Delete a branch
git branch -d feature1
```

### 5. Discover branch source

```bash
git checkout feature1
git log --graph --decorate
```

## Note

> HEAD points to the last commit of the current working branch
> HEAD will switch when we switch branches
