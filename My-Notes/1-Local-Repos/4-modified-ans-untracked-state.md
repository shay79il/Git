# Modified **and** untracked state

### 1. Make a change

```bash
echo "This is another new line" >> story1.txt
echo "This is a new story2" > story2.txt
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
        modified:   story1.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        story2.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

### 3. git add `.`

If we want to save the new state of the file

```bash
# Stage both files
# The untracked one and the changed one
git add .
```

### 4. git commit

We want to commit all staged files

```bash
git commit -m "update story1 and create new story2.txt"
```

### 5. commit separately

If the 2 stories sre **unrelated** so we wold like want to make 2 separately commits, that's why we have the **staging** area

```bash
git add story1.txt
git commit -m "update story1"

git add story2.txt
git commit -m "create new story2.txt"
```

## Note

### Commits best practice is to make each commit atomic which means that all the changes committed belong to the same feature/problem solution.
