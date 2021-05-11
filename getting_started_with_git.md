# Getting Start with Git

## help command

man git -> full manual (HIGH LEVEL COMMADN, LOWER LEVEL COMMANDS(PLIMBING)

git help config

git help

## git basic command

git status (-s): condensed version of the status 
git add : used to add files or add changes from a file to a stage
git stage : put files or change in the stage state
git diff --staged: compares staged version versus committed version (locally)
git diff --staged --no-renames: to tell get to ignore the hash for empty files so it doesn't think you are modifying the same file (e69de29)
git diff : different between staged and working directory (locally)

To skip staging and go straight to committing:
git commit -a -m
-m is for commit message
-a commit all changed files

## Extended Command of Everyday Git

git push origin-1 master:

git log: show commit history

git log -1
git log --oneline
git log --stats : extra details
git log --patch : this will provide the full diff

git rm: remove a file 
git rm --cached : to untrack a file 
git mv old-file new-file-name

git merge (to-branch: if ommited it will be check out branch) (from branch)
git reset: allows to move commit from history to working or staging area
    git reset --soft:  will move the committed to staging area
    git reset --mixed: default, move from the committed changes to working directory. git reset --mixed hash
    git reset --hard: will take the committed change to trash (gone)

you can use 'git reset 'to regroup commits from different branches into a single commit 


