# Experiment 7: Git Commands to Create a Lightweight Git Tag (v1.0)

## Prerequisites

- A local Git repository must be initialized. If you don’t have one, initialize it with:
  ```bash
  git init
  ```
---

## Steps to Create a Lightweight Tag

### 1. Verify the Repository State
Ensure that you are in a valid Git repository:
```bash
git status
```
This command will show the current state of your repository.

### 2. Identify the Commit to Tag
To create a tag, you need the commit hash of the commit you want to tag. Use the following command to view the commit history:
```bash
git log --oneline
```
This will display the commit history in a concise format. Note down the desired commit hash.

### 3. Create the Lightweight Tag
Use the `git tag` command to create a lightweight tag. Replace `<commit-hash>` with the commit hash you noted earlier:
```bash
git tag v1.0 <commit-hash>
```
If you want to tag the latest commit (HEAD), you can simply run:
```bash
git tag v1.0
```

### 4. Verify the Tag
To confirm that the tag has been created, list all tags in the repository:
```bash
git tag
```
You should see `v1.0` in the list of tags.

---

### View Detailed Information About a Tag
For a lightweight tag, you can view its associated commit details:
```bash
git show v1.0
```

---
# ScreenShot

![Screenshot 2024-12-11 104640](https://github.com/user-attachments/assets/2d7025c4-9606-44ed-833f-1d620f05ed13)


![Screenshot 2024-12-11 104707](https://github.com/user-attachments/assets/409e395b-33d5-4f9d-9c7e-f30d7d15be26)
