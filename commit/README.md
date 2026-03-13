# Git Commit Tutorial

## What is `git commit`?

`git commit` saves staged changes to the local repository history.

---

## Basic Commit

```bash
git commit -m "Your message"
```

---

## Writing Good Messages

Good commit messages:

* describe what changed
* are short and clear
* use present tense

Example:

```bash
git commit -m "Add login feature"
```

---

## Commit All Tracked Changes

```bash
git commit -am "Update files"
```

Note: This does NOT add new untracked files.

---

## Why Commits Matter

Commits create a timeline of your project:

* track progress
* revert mistakes
* collaborate safely
