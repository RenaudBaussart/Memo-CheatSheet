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
`git diff`show the exact diff between active directory and the staging area  
    - `--staged` same as diff but for staging and last commit
### Remote Repositories:
`git remote add <name> <repository_url>` Add a Remote Repository  
`git remote -v` List Remote Repositories  
`git remote remove <name>` Remove a Remote Repository  
### Undoing Changes:
`git reset HEAD~1` Undo Last Commit (Keep Changes)  
`git checkout -- <file(s)>` Discard Changes in Working Directory  
`git reset --hard HEAD~1` Undo Last Commit and Changes 
`git commit -- amend` change the message on the last commit  
`git revert [commit number]` this will revert all modif ater this commit
### Miscellaneous:
to Ignore Files Create a `.gitignore` file and list files/directories to be ignored.  
`git config --list` View Git Configuration  
`git diff > patch_name.patch`  
`git apply patch_name.patch` Create and Apply Patch  
`git stash` Stash Changes  
`git stash apply` Apply Stashed Changes  

****what to do to when we did sometiong wrong****
```
git reflog
# you will see a list of every thing you've
# done in git, across all branches!
# each one has an index HEAD@{index}
# find the one before you broke everything
git reset HEAD@{index}
# magic time machine
```