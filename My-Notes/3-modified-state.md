# Modified state

### 1. Make a change

```bash
echo "This is a new line" >> story1.txt
```

### 2. git status - again

We can see now the file in a modified state

```bash
git status

# Output
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   ../My-Notes/2-git-init.md
        modified:   story1.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

### 3. git add `story1.txt`

If we want to save the new state of the file

```bash
git add story1.txt
```

### 3.1 git restore `story1.txt`

In case we regret the change and did **not** committed already we will get the file in its previous state before the change we made

```bash
git restore story1.txt
```

### 4. git commit

We want to commit `story1.txt` to be committed

```bash
git commit -m "update story"
```
