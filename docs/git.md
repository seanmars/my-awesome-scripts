# Git

- [Get one commit date](#get-one-commit-date)
- [Get latest commit id](#get-latest-commit-id)

## Get one commit date

```sh
git show -s --date=format:'%Y.%m%d.%H%M%S' --format=%cd <commit id>
```
output:
```sh
2024.0630.220643
```

## Get latest commit id

```sh
git log --oneline -n 1 --pretty=format:"%h"
```
output:
```sh
cc9956a
```
