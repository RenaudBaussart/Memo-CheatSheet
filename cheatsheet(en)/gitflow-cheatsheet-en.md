## Cheat Sheet

| Command | Function | Example |
| --- | --- | --- |
| **Setup & Initialization** | | |
| `git init` | Initializes a Git repository in the current directory | |
| `git clone [url]` | Retrieves the entirety of a remote repository via URL | `git clone git@github.com:Simplon-hdf/cheats-sheets-git-flow.git` |
| **Index** | | |
| `git status` | Displays modified files in the working directory | |
| `git add [file]` | Moves a file to the staging area | `git add example.md` |
| `git reset [file]` | Removes a file from the index while keeping changes in the working directory | `git reset example.md` |
| `git diff` | Shows differences in changes outside of the index | |
| `git diff --staged` | Shows differences between the index and the last commit | |
| `git diff [local branch] [remote branch]` | Compares differences between a local and remote branch | `git diff develop main` |
| `git commit -m [message]` | Commits files in the index | `git commit -m "Renamed example.md"` |
| **Branches** | | |
| `git branch -av` | Lists branches. A * will appear next to the current branch | |
| `git branch [branch]` | Creates a new branch | `git branch main` |
| `git switch [branch]` | Changes the current branch | `git switch develop` |
| `git branch -d [branch]` | Deletes the local branch | `git branch -d develop` |
| `git checkout --track` | Creates a new local branch from a remote branch and tracks it | |
| `git tag [tag-name]` | Creates a tag on the current commit | `git tag v1.0` |
| **History** | | |
| `git log` | Displays commit history | |
| `git log -p [file]` | Displays commit history on a specific file | `git log -p example.md` |
| `git blame [file]` | Displays modification history, including authorship, on a specific file | `git blame example.md` |
| **Update & Publish** | | |
| `git remote -v` | Lists configured remotes | |
| `git remote show [remote]` | Displays information about the remote | `git remote show origin` |
| `git remote add [remote] [url]` | Creates a connection with a remote repository under a shortcut | `git remote add origin git@github.com:Simplon-hdf/cheats-sheets-git-flow.git` |
| `git fetch [remote]` | Retrieves all changes from the remote without merging changes | `git fetch origin` |
| `git pull [remote] [branch]` | Retrieves changes from the branch and merges them | `git pull origin main` |
| `git push [remote] [branch]` | Pushes commits from a local branch to a remote repository | `git push origin main` |
| **Merge & Rebase** | | |
| `git merge [branch]` | Merges the specified branch with the current branch | `git merge main` |
| `git rebase [branch]` | Reapplies commit history of the current branch on top of the specified branch | `git rebase main` |
| `git rebase --abort` | Cancels the ongoing rebase process | |
| `git rebase --continue` | Continues the rebase process after resolving conflicts | |
| `git mergetool` | Opens a merge tool to resolve conflicts | |
| **Undo/Redo** | | |
| `git reset --hard HEAD` | Resets the index and the working directory to the commit referenced by HEAD | `git reset --hard @~1` |
| `git checkout HEAD [file]` | Restores a specific file in the working directory to the last commit (HEAD) | `git checkout HEAD example.md` |
| `git revert [commit]` | Undoes changes from a specific commit | `git revert 8d6fe82` |
| `git reset --hard [commit]` | Resets the index and the working directory to the specified commit | `git reset --hard 8d6fe82` |
| `git reset [commit]` | Moves the current branch to the specified commit | `git reset 8d6fe82` |
| `git reset --keep [commit]` | Moves the branch while retaining changes outside of the index | `git reset --keep 8d6fe82` |