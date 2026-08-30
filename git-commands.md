# Git Commands Reference

1. Setup & Config
- `git --version` or `git -v` : Check Installation. Shows the currently installed git version. 
- `git config --global user.email "yourmail@email.com" : Set Email. Sets your author email globally for all repositories on your system.
- `git config --global user.name "username" : Set Name. Sets your author name globally, which will attach to all future commits.
- `git config --global --list` : Verify settings. Display all global configuration settings. 


2. Basic Workflow
- `git init` : Initialize Repository. Creates a new, hidden '.git' subdirectory in your current folder, turning it into a tracked Git repository.
- `git add filename` : Add untracked files to Staging area.
- `git commit -m "Commit Message"` : Commit all staged files in repository.

3. Viewing Changes
- `git status` : Check Repository State. Displays the state of the working directory and staging area (shows tracked, untracked and modified files).
- `git log` : Default View of git history with full Details (SHA,author,date,comment message)
- `git log --oneline` : Compact View of git history i.e. One line per commit.
- `git log -n 5` : Limit count. Show only the last N commits history.
- `git log -p` : Shows actual file changes for each commit
- `git log --author="name"`: Filters history by a specific author

4. Branching Commands
- `git branch` or `git branch -a` : To find the all branches from repo.
- `git branch <branch-name>` : To create new branch without switching to it at the same time.
- `git switch <branch-name>` : Switch between branches.
- `git checkout -b <branch-name>`: Create and switch branch immediately.
- `git log master..feature-1 --oneline` : See commits on feature that are not on main branch. (Target branch is second.)
- `git log feature-1..master --oneline` : See commits on main that are not on feature branch. (Target branch is second.)
- `git branch -d <branch-name>` : Safe delete (Recommended)
- `git branch -D <branch-name>` : Force delete
