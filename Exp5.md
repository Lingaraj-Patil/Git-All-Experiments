# Experiment 5: Git fetch and rebase

Follow the steps below to complete the Git experiment:

## Steps

### 1. Clone a Remote Repository
Run the following command to clone the remote repository to your local machine:

```bash
git clone <repository-url>
```
Replace `<repository-url>` with the URL of the remote repository you want to clone.

---

### 2. Make Changes to the README File
Navigate to the repository folder:

```bash
cd <repository-folder>
```

Open the `README.md` file and make some changes using your preferred text editor. For example, add a new line:

```markdown
## Experiment
This is a Git experiment for practicing commands like fetch, rebase, and push.
```
Save the file.

---

### 3. Fetch Changes from the Remote Repository
To fetch updates from the remote repository without merging, run:

```bash
git fetch origin
```

---

### 4. Rebase Your Branch with the Remote `main`
Rebase your local branch with the latest changes from the remote `main` branch:

```bash
git rebase origin/main
```

Resolve any conflicts that may arise during the rebase process. After resolving conflicts, continue the rebase process:

```bash
git rebase --continue
```

---

### 5. Push Changes to the Remote Repository
Finally, push your changes to the remote `main` branch:

```bash
git push origin main
```

If you encounter issues due to updates on the remote branch, you may need to force push (use with caution):

```bash
git push origin main --force
```

---

## Notes
- Always ensure that you have saved your work and are aware of the implications of rebasing and force-pushing.
- Use `git status` frequently to check the state of your working directory and staging area.

# Screenshot
![Screenshot 2024-12-11 103841](https://github.com/user-attachments/assets/16438d39-3b3a-4e93-bb8e-82a6ed79f7fe)

![Screenshot 2024-12-11 103927](https://github.com/user-attachments/assets/6bb9fe2e-7b9d-4d9e-8723-aa791bc98b51)

