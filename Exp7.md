# Experiment 7: Cherry-Pick a Range of Commits

This guide provides step-by-step instructions to cherry-pick a range of commits from a "source branch" into the current branch.

## Steps to Cherry-Pick a Range of Commits

1. **Switch to the Target Branch**  
   Ensure you are on the branch where you want to cherry-pick the commits. Run:

   ```bash
   git checkout <target-branch>
   ```

2. **Identify the Commit Range**  
   Find the hash of the first and last commit you want to cherry-pick from the "source branch." You can use the following command to view the commit history:

   ```bash
   git log <source-branch>
   ```

   Copy the hashes of the starting commit (`<start-commit>`) and the ending commit (`<end-commit>`).

3. **Cherry-Pick the Commit Range**  
   Use the following command to cherry-pick the range of commits:

   ```bash
   git cherry-pick <start-commit>^..<end-commit>
   ```

   - The `^` before `<start-commit>` ensures that the range includes the `<start-commit>` itself.

4. **Resolve Any Conflicts**  
   If there are conflicts during the cherry-pick process, Git will pause and allow you to resolve them. Follow these steps:

   - Open the conflicted files, resolve the conflicts manually, and save the changes.
   - After resolving conflicts, mark them as resolved:

     ```bash
     git add <file>
     ```

   - Continue the cherry-pick process:

     ```bash
     git cherry-pick --continue
     ```

5. **Verify the Changes**  
   After successfully cherry-picking, review the changes to ensure they match the intended commits:

   ```bash
   git log
   ```
# Screenshot

![Screenshot 2024-12-11 110116](https://github.com/user-attachments/assets/abac2dc2-4905-4e6e-87f8-9d280003e5cc)

![Screenshot 2024-12-11 110216](https://github.com/user-attachments/assets/9908d7b4-fb5a-4acd-86d4-f0edaad8a4d6)




