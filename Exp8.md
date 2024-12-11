# Experiment 8: Git Commands: `git show <commit-id>` and `git log -n 1 <commit-id>`

This README explains the usage of the Git commands `git show <commit-id>` and `git log -n 1 <commit-id>`. These commands are commonly used to inspect commits and retrieve detailed information about them.

---

## `git show <commit-id>`

### Description
The `git show` command displays detailed information about a specific commit. This includes:
- Commit hash
- Author name and email
- Commit date
- Commit message
- Changes made in the commit (diff)

### Syntax
```bash
git show <commit-id>
```

### Example
```bash
git show abc1234
```
This displays all details and changes associated with the commit `abc1234`.

### Output
The output will look like this:
```
commit abc1234
Author: John Doe <john.doe@example.com>
Date:   Wed Dec 11 10:00:00 2024 +0000

    Add README file for Git commands

--- a/README.md
+++ b/README.md
@@ -1,4 +1,10 @@
+## New Section
+This is an example of added content.
...
```

---

## `git log -n 1 <commit-id>`

### Description
The `git log` command is used to view the commit history. Using the `-n 1` option with a specific `<commit-id>` limits the output to the details of that single commit.

### Syntax
```bash
git log -n 1 <commit-id>
```

### Example
```bash
git log -n 1 abc1234
```
This displays the details of the commit `abc1234`, limited to one log entry.


---

## Differences Between `git show` and `git log -n 1`
| Feature             | `git show`                                   | `git log -n 1`                        |
|---------------------|----------------------------------------------|---------------------------------------|
| Details about commit| Displays full diff and metadata              | Displays metadata only                |
| Use case           | Inspecting detailed changes in a commit      | Viewing concise commit information    |

---

## Use Cases
- **Debugging**: Use `git show` to review code changes in detail.
- **Tracking commits**: Use `git log -n 1` for a summary of a specific commit.

---

## Notes
- Always replace `<commit-id>` with the actual hash of the commit you want to inspect.
- Ensure your repository is up-to-date to get accurate commit information.

---
# Screenshot
