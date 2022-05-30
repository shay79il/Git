# Remove staged file

### 1. Make a change

```bash
echo "This is another new line" >> story1.txt
echo "These are my notes - not to be committed" > notes.txt
```

### 2. git status

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
        notes.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

### 3. git add `.` - accidentally

If we want to save the new state of the file

```bash
# Stage both files
# The untracked one and the changed one
git add .
```

### 4. git status - again

We can see we added the notes file by accident

```bash
git status

# Output
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   notes.txt
        modified:   story1.txt
```

### 5. git [-f] [--cached] rm

In order to remove staged file and delete it we will use '-f' flag **but** if we just need to remove the file from the staging area **and** retain the file we can use the '--cached' flag and add the file to '.gitignore'

```bash
git rm --cached notes.txt
```
