# A list of commonly used Git commands

If you're looking for more details on my Git aliases, check out my [bash_profile](https://github.com/joshnh/bash_profile/blob/master/.bash_profile).

---

## Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

---

## Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check the status of your working directory |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit your changes with a message |
| `git rm -r [file-name.txt]` | Remove a file (or folder) from the repository |
| `git remote -v` | View the remote repository linked to your project |

---

## Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List local branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch-name]` | Create a new branch |
| `git branch -d [branch-name]` | Delete a local branch |
| `git push origin --delete [branch-name]` | Delete a remote branch |
| `git checkout -b [branch-name]` | Create and switch to a new branch |
| `git checkout -b [branch-name] origin/[branch-name]` | Clone a remote branch and switch to it |
| `git branch -m [old-branch-name] [new-branch-name]` | Rename a local branch |
| `git checkout [branch-name]` | Switch to a branch |
| `git checkout -` | Switch to the last branch you were on |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch-name]` | Merge a branch into the active branch |
| `git merge [source-branch] [target-branch]` | Merge one branch into another |
| `git stash` | Stash your current changes |
| `git stash clear` | Remove all stashed changes |
| `git stash pop` | Apply the most recent stashed changes |

---

## Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch-name]` | Push a branch to your remote repository |
| `git push -u origin [branch-name]` | Push changes and set upstream branch for future pushes |
| `git push` | Push changes to the remote repository (current branch) |
| `git push origin --delete [branch-name]` | Delete a remote branch |
| `git pull` | Pull the latest changes from the remote repository |
| `git pull origin [branch-name]` | Pull changes from a specific remote branch |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Change the remote URL to SSH |

---

## Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View the commit history |
| `git log --summary` | View detailed commit history |
| `git log --oneline` | View brief commit history |
| `git diff [source-branch] [target-branch]` | Preview changes before merging branches |
