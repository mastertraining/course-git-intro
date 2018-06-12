# Git
## An Introduction

---

## Why Git?

---

## Basic Git Commands

Added all files to staging area

```
git add .
```

Commit the staging area to the repository

```
git commit -m "Commit message"
```

---

## View the log

```
git log
```

or in condense version

```
git log --oneline
```
or

```
git log --oneline --graph
```

---

## Getting help

```
git --help
```

or

```
git <command> --help
```

For example:

```
git log --help
```

---

## Checkout

```
git checkout HEAD~2
```

or

```
git checkout HEAD~1 -- Content.md
```

---

## Branching

---

## Branching
### Create a branch

**PREFER**

```
git checkout -b branch_name
```

instead of

```
git branch branch_name
git checkout branch_name
```

---

## Branching
### Merging a branch

**PREFER**

```
git checkout master
git merge --no-ff branch_name
```

instead of

```
git checkout master
git merge branch_name
```

For checking into master (master is a base)

---

## Handling conflicts

---

## Branching
### Rebase a branch

```
git checkout branch_name
git rebase master
```

Then merge

---

## Working with history

---

## Git Revert

For one recent commit

```
git revert HEAD~1
```

For more than one commit

```
git revert HEAD~3..HEAD~1
```

---

## Git Reset

Reset the last 2 commits

```
git reset HEAD~2
```

---

## Recovering the deleted commit

Finding the recovering target

```
git reflog
```

Then use git reset or revert

---

# For Academy