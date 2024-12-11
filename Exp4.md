# Experiment 4: Stashing

This repository documents a series of Git commands used to initialize a repository, manage files, and utilize Git's stash feature.

## Commands Overview

### 1. Create a New Directory
```bash
$ mkdir exp4
```
- Creates a new directory named `exp4`.

### 2. Navigate into the Directory
```bash
$ cd exp4
```
- Changes the current working directory to `exp4`.

### 3. Initialize a Git Repository
```bash
$ git init
```
- Initializes a new empty Git repository in the current directory.

### 4. Create a New File
```bash
$ touch file.txt
```
- Creates a new, empty file named `file.txt` in the current directory.

### 5. Stage Files for Commit
```bash
$ git add .
```
- Stages all changes in the current directory for the next commit.

### 6. Commit Changes
```bash
$ git commit -m "initial commit to master"
```
- Commits the staged changes with the message `initial commit to master`.

### 7. Create Another File
```bash
$ touch file2.txt
```
- Creates a new, empty file named `file2.txt` in the current directory.

### 8. Attempt to Stash Changes
```bash
$ git stash save "stashing file2.txt"
```
- The first attempt to stash fails with the message `No local changes to save` because the file was not yet staged.

### 9. Stage the File
```bash
$ git add file2.txt
```
- Stages `file2.txt` for the next commit.

### 10. Stash the Staged Changes
```bash
$ git stash save "stashing file2.txt"
```
- Saves the current working directory and index state (including staged `file2.txt`) to the stash, allowing you to save work without committing it.

### 11. Apply the Stash
```bash
$ git stash apply
```
- Reapplies the stashed changes to the working directory. The staged changes are restored.

## Notes
- **Stashing**: Git stash allows you to save and temporarily set aside changes without committing them. You can later apply or drop the stashed changes.
- **Staging**: Files must be staged before stashing if you want to stash changes in the index.
- **Applying the Stash**: When applying the stash, the changes are reapplied, but the stash remains in the stash list. Use `git stash pop` to apply and remove the stash in one step.

## Problem You may face : If you don't first commit and then use stash


## ScreenShot
