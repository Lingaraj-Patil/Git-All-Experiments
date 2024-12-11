# Experiment 2: Creating a Repository, Branching, and Merging

This guide explains how to perform the following Git operations:
1. Create a new directory and initialize it as a Git repository.
2. Add and commit files in the repository.
3. Create and switch to a new branch.
4. Add and commit files in the new branch.
5. Merge the new branch back into the main branch (master).

## Steps

### 1. Create a New Directory and Initialize Git
```bash
# Create a new directory
mkdir exp2
cd exp2

# Initialize an empty Git repository
git init
```

### 2. Create a File and Add It to the Repository
```bash
# Create a new file
echo "Initial content" > file1.txt

# Stage the file for commit
git add file1.txt

# Commit the file to the repository
git commit -m "Added initial file"
```

### 3. Create a New Branch and Switch to It
```bash
# Create and Switch to the 'feature' branch
git checkout  -b feature
```

### 4. Create Another File in the Feature Branch
```bash
# Create a new file in the 'feature' branch
echo "Feature branch content" > file2.txt

# Stage the file for commit
git add file2.txt

# Commit the file to the repository
git commit -m "Add file2.txt in feature branch"
```

### 5. Switch Back to the Master Branch and Merge the Feature Branch
```bash
# Switch back to the 'master' branch
git checkout master

# Merge the 'feature' branch into 'master'
git merge feature
```
## Screenshot