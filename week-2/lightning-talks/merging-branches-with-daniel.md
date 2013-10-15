# Merging Branches with Daniel

How to keep your master perfect all the time:

1. We were each working on features in different branches
1. We both had divered from master quite a bit.
1. First merge went fine. Could be merged automatically
1. Second pull request conflicted, so it couldn't be merged automatically.
1. So we fixed it:
  * `git checkout master`
  * `git pull master`
  * `git checkout our-branch`
  * `git merge master`
  * resolved merge conflicts
  * `git add each-file-that-had-a-merge-conflict`
  * `git commit`
  * `git push origin our-branch`
  * the pull request is automatically updated
