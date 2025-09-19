[⬅️ Back to Index](./readme.md)

# 📋 All Git Commands  

This file contains a list of commonly used Git commands with their descriptions. Use it as a quick reference guide.  

---

## 🔹 Basic Commands  

| Command | Description |
|---------|-------------|
| `git init` | Initialize a new Git repository |
| `git status` | Show the current state of the working directory and staging area |
| `git add <file>` | Add a file to the staging area |
| `git add .` | Stages all changes (new, modified, and deleted files) in the current directory and its subdirectories for the next commit |
| `git commit -m "message"` | Save changes with a commit message |
| `git log` | View commit history |

---

## 🔹 Commit History  

| Command | Description |
|---------|-------------|
| `git log` | Shows commit history (newest → oldest by default) |
| `git log --oneline` | Shows commit history in a condensed format (short hash + message) |
| `git log --reverse` | Displays commits in reverse order (oldest → newest) |
| `git log -n 5` | Shows only the last 5 commits (`-n` or `--max-count`) |
| `git log --oneline -n 3` | Shows the last 3 commits in one-line format |
| `git log --reverse -n 3` | Shows the first 3 commits ever made |

---

## 🔹 Remote Repository Commands (GitHub)

| Command | Description |
|---------|-------------|
| `git remote -v` | Show all remote repositories linked to your project |
| `git remote add origin <repo-url>` | Link your local repo with a remote repo (usually GitHub) |
| `git remote remove origin` | Remove the remote connection named `origin` |
| `git push -u origin main` | Push local code to remote `main` branch for the first time |
| `git push --set-upstream origin <branch>` | Same as `-u`, long version of the flag, sets upstream branch tracking |
| `git push` | Push latest commits to remote repository |
| `git pull` | Fetch and merge changes from remote to local repo |
| `git fetch` | Download changes from remote without merging |
| `git clone <repo-url>` | Copy (clone) a remote repository into your system |

---

## 🔹 Branch Commands

| Command | Description |
|---------|-------------|
| `git branch` | List all local branches |
| `git branch <branch-name>` | Create a new branch |
| `git checkout <branch-name>` | Switch to an existing branch |
| `git checkout -b <branch-name>` | Create and switch to a new branch |
| `git branch -d <branch-name>` | Delete a branch (safe delete, prevents if branch has unmerged changes) |
| `git branch -D <branch-name>` | Force delete a branch |
| `git switch <branch-name>` | Switch to a branch (modern alternative to `checkout`) |
| `git switch -c <branch-name>` | Create and switch to a new branch |
| `git merge <branch-name>` | Merge a branch into the current branch |
| `git push origin <branch-name>` | Push a branch to remote repository |
| `git push origin --delete <branch-name>` | Delete a branch from remote repository |
| `git branch -m <new-name>` | Rename the current branch |

---

## 🔹 Fix Mistakes (Undo & Revert)

| Command | Description |
|---------|-------------|
| `git checkout -- <file>` | Undo changes in a file (go back to last committed version) |
| `git restore <file>` | Modern way to undo changes in a file (similar to above) |
| `git restore --staged <file>` | Unstage a file (move from staged area back to working directory) |
| `git reset HEAD <file>` | Unstage a file (older syntax, same as above) |
| `git reset --soft <commit-hash>` | Move HEAD to a commit, keep changes staged |
| `git reset --mixed <commit-hash>` | Move HEAD to a commit, keep changes unstaged (default mode) |
| `git reset --hard <commit-hash>` | Move HEAD to a commit and discard all changes after it |
| `git revert <commit-hash>` | Create a new commit that undoes the changes of the given commit |
| `git log` | View commit history (to find commit hashes for checkout/reset/revert) |
| `git checkout <commit-hash>` | Move (time travel) to a specific commit in "detached HEAD" state |
| `git switch -` | Quickly switch back to the previous branch |
