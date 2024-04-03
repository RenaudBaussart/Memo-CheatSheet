## Basic Commands:
`git init`Initialize a Repository  
`git clone <repository_url>` Clone a Repository  
`git add <file(s)>` Add Changes  
`git commit -m "Commit message"` Commit Changes  
`git push <remote> <branch_name>` Push Changes to Remote Repository  
`git pull <remote> <branch_name>` Pull Changes from Remote Repository  
`git status` Check Repository Status  
## Branching and Merging:
`git branch` list all the branch in the local Repository  
`git branch <branch_name>` Create a New Branch  
`git switch <branch_name>` Switch to a Branch  
`git switch -b <branch_name>` Create a New Branch and Switch to it  
`git merge <branch_name>` Merge Branches into the current branch  
`git branch -d <branch_name>` Delete a Branch  
### Logging and History:
`git log` View Commit History  
`git show <commit_id>` View Changes Made in a Commit  
`git diff <branch1> <branch2>`View Differences Between Branches  
### Remote Repositories:
`git remote add <name> <repository_url>` Add a Remote Repository  
`git remote -v` List Remote Repositories  
`git remote remove <name>` Remove a Remote Repository  
### Undoing Changes:
`git reset HEAD~1` Undo Last Commit (Keep Changes)  
`git checkout -- <file(s)>` Discard Changes in Working Directory  
`git reset --hard HEAD~1` Undo Last Commit and Changes 
### Miscellaneous:
to Ignore Files Create a `.gitignore` file and list files/directories to be ignored.  
`git config --list` View Git Configuration  
`git diff > patch_name.patch`  
`git apply patch_name.patch` Create and Apply Patch  
`git stash` Stash Changes  
`git stash apply` Apply Stashed Changes  