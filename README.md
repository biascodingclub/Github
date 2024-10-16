
# Basic Git CLI Commands

## 1. `git status`
Displays the current status of the working directory and staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git.

## 2. `git add <file>`
Adds changes from the working directory to the staging area. Use `.` to add all files.

Example:
```
git add .
```

## 3. `git commit -m "<message>"`
Records or snapshots the changes made to the repository with a descriptive message.

Example:
```
git commit -m "Initial commit"
```

## 4. `git push <remote> <branch>`
Uploads your local repository content to a remote repository. By default, it will push to the branch you are currently working on.

Example:
```
git push origin main
```

## 5. `git pull <remote> <branch>`
Fetches and integrates changes from the remote repository into your current branch. It is a combination of `git fetch` and `git merge`.

Example:
```
git pull origin main
```

## 6. `git branch`
Lists all the branches in your repository. You can also create or delete branches with the `git branch` command.

Example:
```
git branch -a  # list all branches
git branch new-feature  # create a new branch
```

## 7. Merge Conflicts
A merge conflict occurs when Git is unable to automatically resolve differences in code between two commits. This typically happens when two branches modify the same line in a file differently.

To resolve:
- Edit the conflicting files to your preference.
- Once resolved, mark the conflicts as resolved using `git add <file>`.
- Commit the merge.

Example resolution:
```
git add conflicted-file.txt
git commit -m "Resolved merge conflict in file"
```

## Useful Tip
Always ensure you `pull` changes before you start working to avoid unnecessary merge conflicts later on.
