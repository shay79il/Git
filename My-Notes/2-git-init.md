# `git init` command

## We go to a folder we want to `git init` so we have the git app start to do its magic there we will have the hidden folder of `.git`

## Now lets play with git

### 1. Create a new file

```bash
touch story1.txt
echo "This is a beautiful story" >> story1.txt
```

### 2. git status

We can see 1 file which is **untracked** - story1.txt

```bash
git status
```

### 3. git add

We want to add `story1.txt` to be tracked by git

```bash
git add story1.txt
```

### 4. git commit

We want to commit `story1.txt` to be committed
which is a copy of the file in its current state

```bash
git commit -m "Add the first story"
```

### 5. git status

We can see now

```bash
git status

# Output
On branch main
nothing to commit, working tree clean
```

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

### 4. git commit

We want to commit `story1.txt` to be committed

```bash
git commit -m ""update story"
```
