# Git Add Tutorial

## What is `git add`?

`git add` stages changes before committing.

Git tracks changes in two steps:

1. Add files (staging)
2. Commit changes


## Add One File

```bash
git add filename
```


## Add All Files

```bash
git add .
```


## Add Only Modified Files

```bash
git add -u
```


## Why Staging Exists

Staging allows you to:

* select specific files
* create clean commits
* review changes before saving


## Example Workflow

```bash
git add main.c
git add README.md
```
