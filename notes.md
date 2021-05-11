# Getting Start with Git

## help command

man git -> full manual (HIGH LEVEL COMMADN, LOWER LEVEL COMMANDS(PLIMBING)

git help config

git help

## git basic command

git status (-s): condensed version of the status 
git add : used to add files or add changes from a file to a stage
git stage : pu files or change in the stage state
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