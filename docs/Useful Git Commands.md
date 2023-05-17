---
sidebar_position: 1
---
----
# 1. Useful Git Commands
----

Here's the formatted text:

### 2. How to check your Git configuration:   
```
git config -l  
```

### 3. How to setup your Git username:
```  
git config --global user.name "CosmosCloud"
```

### 4. How to setup your Git user email:
```
git config --global user.email "admin@cosmoscloud.wiki"
```

### 5. How to cache your login credentials in Git:
```
git config --global credential.helper cache
```

### 6. How to initialize a Git repo:
```
git init
```

### 7. How to add a file to the staging area in Git:    
```
git add filename_here
```

### 8. How to add only certain files to the staging area in Git
```     
git add fil*
```   

### 9. How to check a repository's status in Git:
```
git status
```

### 10. How to commit changes in the editor in Git:     
```   
git commit
```

### 11. How to commit changes with a message in Git:
```
git commit -m "your commit message here"

```

### 12. How to commit changes (and skip the staging area) in Git:
```
git commit -a -m "your commit message here"
```

### 13. How to see your commit history in Git:
```
git log
```
### 14. How to see your commit history including changes in Git:
```
git log -p
```

### 15. How to see a specific commit in Git:
```
git show commit-id
```

### 16. How to see log stats in Git:
```
git log --stat
```

### 17. How to see changes made before committing them using "diff" in Git:
```
git diff  
git diff all_checks.py
git diff --staged
```

### 18. How to see changes using "git add -p":
```
git add -p
```

### 19. How to remove tracked files from the current working tree in Git:
```
git rm filename
```

### 20. How to rename files in Git:
```
git mv oldfile newfile
```

### 21. How to revert unstaged changes in Git:
```
git checkout filename
```

### 22. How to amend the most recent commit in Git:
```
git commit --amend
```

### 23. How to rollback the last commit in Git:
```
git revert HEAD
```

### 24. How to rollback an old commit in Git:
```
git revert comit_id_here
```

### 25. How to create a new branch in Git:
```
git branch branch_name
```

### 26. How to switch to a newly created branch in Git:
```
git checkout branch_name
```

### 27. How to list branches in Git:
```
git branch
```
### 28. How to create a branch in Git and switch to it immediately:

```
git checkout -b branch_name
```

### 29. How to delete a branch in Git:
```
git branch -d branch_name
```

### 29. How to merge two branches in Git:
```
git merge branch_name
```

### 30. How to show the commit log as a graph in Git:
```
git log --graph --oneline
```

### 31. How to show the commit log as a graph of all branches in Git:
```
git log --graph --oneline --all
```

### 33. How to abort a conflicting merge in Git:
```
git merge --abort
```

### 34. How to add a remote repository in Git
```
git add remote https://repo_here
```

### 35. How to see remote URLs in Git:
```
git remote -v
```

### 36. How to push changes to a remote repo in Git:
```
git push
```

### 37. How to get more info about a remote repo in Git:
```
git remote show origin
```

### 38. How to push changes to a remote repo in Git:
```
git push
```

### 39. How to pull changes from a remote repo in Git:
```
git pull
```

### 40. How to check remote branches that Git is tracking:

```
git branch -r
```

### 41. How to fetch remote repo changes in Git:
```
git fetch
```

### 42. How to check the current commits log of a remote repo in Git
```
git log origin/main
```

### 43. How to merge a remote repo with your local repo in Git:
```
git merge origin/main
```

### 44. How to get the contents of remote branches in Git without automatically merging:
```
git remote update
```

### 45. How to push a new branch to a remote repo in Git:
```
git push -u origin branch_name
```

### 46. How to remove a remote branch in Git:
```
git push --delete origin branch_name_here
```

### 47. How to use Git rebase:
```
git rebase branch_name_here
```

### 48. How to run rebase interactively in Git:
```
git rebase -i master
# p, pick = use commit
# r, reword = use commit, but edit the commit message
# e, edit = use commit, but stop for amending
# s, squash = use commit, but meld into previous commit
# f, fixup = like "squash", but discard this commit's log message
# x, exec = run command (the rest of the line) using shell
# d, drop = remove commit
```

### 49. How to force a push request in Git:
```
git push -f
```
