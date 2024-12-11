![Screenshot 2024-12-11 111857](https://github.com/user-attachments/assets/a4cd7f13-c781-4ddf-9327-6d74b7cdd4ad)# Experiment 9: 
This guide shows how to initialize a new Git repository, make some commits, and use `git log` to list commits by a specific author within a date range.

## Steps

### Step 1: Initialize a New Git Repository

```bash
git init my-repo
cd my-repo
```

### Step 2: Create and Commit Files

Create some files and make commits.

```bash
echo "First commit" > file1.txt
git add file1.txt
git commit -m "Initial commit by Lingaraj Patil"

echo "Second commit" > file2.txt
git add file2.txt
git commit -m "Added second file by Lingaraj Patil"

```

### Step 3: View Commits by Author and Date Range

Run the following command to list commits by "Lingaraj Patil" between 2024-12-01 and 2024-12-11:

```bash
git log --author="Lingaraj Patil" --since="2024-12-01" --until="2024-12-11" --pretty=format:"%h %ad | %s" --date=short
```

## Notes
- Replace "Lingaraj Patil" with the desired author name.
- Modify the date range (`--since` and `--until`) as needed.

# ScreenShot
![Screenshot 2024-12-11 111857](https://github.com/user-attachments/assets/9d31c90a-e94f-433a-a0e3-f2b152bc2a61)

![Screenshot 2024-12-11 111914](https://github.com/user-attachments/assets/e18b2128-35e1-445d-ba36-3608f8968ae6)


