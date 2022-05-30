# Modify staged file

## 1. Make a change

```bash
echo "This is another new line to story1" >> story1.txt
```

## 2. git status

We can see now the file in a modified state

```bash
git status

# Output
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   story1.txt

no changes added to commit (use "git add" and/or "git commit -a")
```

## 3. git add `.`

```bash
# Stage the changes
git add .
```

## 4. Make a change - again

```bash
echo "This is a whole new story1" > story1.txt
```

## 5. git status - again

### We can see now the file in a **modified** state **and** in **staged** state

```bash
git status

# Output
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   story1.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   story1.txt
```

### 6. git restore [--staged]

In case we regret the change in the **staged** area and did **not** committed already we will get the file in its previous state before the change we made
OR
In case we regret the change in the we will get the file in its previous state before the change we made

```bash
git restore story1.txt
```

### 7. commit separately

If the 2 stories sre **unrelated** so we wold like want to make 2 separately commits, that's why we have the **staging** area

```bash
git add story1.txt
git commit -m "update story1"

git add story2.txt
git commit -m "create new story2.txt"
```

## Note

### Commits best practice is to make each commit atomic which means that all the changes committed belong to the same feature/problem solution.
