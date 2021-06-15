## rename branches
git branch -m old branch_name new branch_name

## deleting branch 
git branch -d branch

## Merging
Target and Source
Target: master
source: solution branch

Fast Forward merge
git checkout<target-branch>
git merge <source branch> 

## how to compare branches 
git diff <branch1> <branch2> 

## git rebase 
git rebase: used to cleanup history
Do not use rebase on a public branch 

cases to use it:
    - clean up your local history before sharing a branch 
    - pull changes from a branch into your branch without performing a merge.

steps for squashing commits with rebase:
git log --oneline    << see the branch history
git merge-base ticket1 master  << show the original base of the "ticket1" branch created from master. aka show common ancestor sha between master and branch
git rebase -i <commit-sha> or get rabase <origainl_branch> << first is for squashing.. second is for rebasing >>
update the text with squash instead of pick
choose the commit message

to see history of the rebase you will see 

git reflog 

# Cherry pick 

Check out a branch and run the command below to copy the commit in other branches to checked out branch
git cherry-pick <<commit hash >>

# Remotes
git fetch: download but don't merge 
git pull: download and merge

git status : give information about the remote and how to resolve conflicts 

to rebase from remote you can do 
git rebase remote/origin
This is a a good way to resolve conflicts with less chance of having to deal with merge conflicts.

git ls-remote: list remote branches
git push -u origin feature4 