## Gist Stash with Gary
Whenever someone submits a pull request, every team member should stop and go
review the pull request.

But wait! I'm in the middle of coding! I don't want to commit  or lose my work!

GIT STASH TO THE RESCUE!

1. `git stash` - This saves all the un-committed code in a 'stash'
1. `git stash list` - This lists all the stashes you can retrieve
1. `git stash apply STASH_NAME` - applies the named stash
1. `git stash pop` - applies the most recently stashed stash and deletes it
1. `git stash branch BRANCH_NAME` - Creates a branch from your stash
1. `git stash --help` - tells you how git stash works

