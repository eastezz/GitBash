# Git Status Tutorial

## What is `git status`?

`git status` shows the current state of your repository.

It tells you:

* modified files
* staged files
* untracked files
* current branch

## Basic Usage

```bash
git status
```


## Why It Is Important

Use it frequently to understand what Git is tracking.


## Example Output

```
On branch main
Changes not staged for commit:
  modified: main.c

Untracked files:
  newfile.txt
```


## Tip

Run `git status` before committing to avoid mistakes.
