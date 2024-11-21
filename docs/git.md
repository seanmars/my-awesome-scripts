# Git

## Get one commit date

```sh
git show -s --date=format:'%Y.%m%d.%H%M%S' --format=%cd <commit id>

# 2024.0630.220643
```

## Get latest commit id

```sh
git log --oneline -n 1 --pretty=format:"%h"

# c868157
```
