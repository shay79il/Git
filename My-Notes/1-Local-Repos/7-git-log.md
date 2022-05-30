# Git Log

### 1. git log

```bash
git log

# output
commit dc3eb7363b28d2b6c9b42ffd9e6e4cdfd8e56f1d (HEAD -> main)
Author: Shay Goldstein <shay79il@gmail.com>
Date:   Mon May 30 13:07:40 2022 +0300

    update .gitignore
```

### 2. git log --oneline

```bash
git log --oneline

# Output
dc3eb73 (HEAD -> main) update .gitignore
2885202 update story1
b392e9e update story1
325ea9c Create new story2
118d328 update story1
b2516c0 update story
```

### 3. git log --name-only

```bash
# List changed files
git log --name-only

# Output
commit dc3eb7363b28d2b6c9b42ffd9e6e4cdfd8e56f1d (HEAD -> main)
Author: Shay Goldstein <shay79il@gmail.com>
Date:   Mon May 30 13:07:40 2022 +0300

    update .gitignore

.gitignore

commit 28852024224f414a156284234412d42d20b5d094
Author: Shay Goldstein <shay79il@gmail.com>
Date:   Mon May 30 12:56:24 2022 +0300

    update story1

story1.txt
```

### 4. git log --oneline -3

```bash
# List in one line last 3 commits
git log --oneline -3

# Output
commit dc3eb7363b28d2b6c9b42ffd9e6e4cdfd8e56f1d (HEAD -> main)
Author: Shay Goldstein <shay79il@gmail.com>
Date:   Mon May 30 13:07:40 2022 +0300

    update .gitignore

.gitignore

commit 28852024224f414a156284234412d42d20b5d094
Author: Shay Goldstein <shay79il@gmail.com>
Date:   Mon May 30 12:56:24 2022 +0300

    update story1

story1.txt
```
