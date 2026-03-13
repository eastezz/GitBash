# Git Branching Tutorial

## What is a Branch?

A branch is an independent line of development.

It allows you to work on new features without affecting the main project.

---

## Why Use Branches?

Branches allow safe development:

* develop new features
* fix bugs
* experiment freely
* collaborate without conflicts

---

## View Existing Branches

```bash id="d1t7om"
git branch
```

---

## Create a New Branch

```bash id="5dth5f"
git branch feature-name
```

---

## Create and Switch to a Branch

```bash id="x71q7m"
git checkout -b feature-name
```

This is the most common command.

---

## Switch Between Branches

```bash id="3ch1v3"
git checkout main
```

---

## Delete a Branch

```bash id="i9nq0m"
git branch -d feature-name
```

---

## Typical Feature Workflow

```bash id="srrxxy"
git checkout -b new-feature
# make changes
git add .
git commit -m "Add new feature"
git push origin new-feature
```

---

## Why Companies Use Branches

Branches allow teams to:

* work simultaneously
* review code before merging
* maintain stable releases
* isolate unfinished work
