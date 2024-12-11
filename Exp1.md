# Experiment 1

---

## 1. Initialize a Git Repository

### Command:
```bash
git init
```

### Explanation:
- `git init` initializes a new Git repository in your project directory.
- This command creates a hidden `.git` folder that stores all necessary files and configurations for version control.
- Run this command at the root of your project to start tracking files.

---

## 2. Create a New File

### Command:
```bash
    touch file.txt
```

### Explanation:
- The above command creates a new file named `example.txt` 
- Alternatively, you can manually create the file using a text editor and save it in the project directory.

---

## 3. Add the File to the Staging Area

### Command:
```bash
git add file.txt
```

### Explanation:
- `git add <filename>` stages the file for the next commit.
- Staging allows you to select specific changes or files you want to include in the next commit.
- You can add multiple files at once by using `git add .` to stage all changes in the directory.

---

## 4. Commit the Changes

### Command:
```bash
git commit -m "Initial commit"
```

### Explanation:
- `git commit` saves the changes you staged with `git add` to the repository's history.
- The `-m` flag allows you to add a commit message directly in the command. For example, "Initial commit" is the message describing this commit.
- A good commit message provides context about the changes made.

---

## Summary of Commands

```bash
# Step 1: Initialize a Git repository
git init

# Step 2: Create a new file
echo "Sample content" > example.txt

# Step 3: Add the file to the staging area
git add example.txt

# Step 4: Commit the changes
git commit -m "Initial commit"
```

With these steps, you've successfully initialized a Git repository, added a file, and committed it. This is the foundation for using Git effectively in your projects.

# ScreenShots
 