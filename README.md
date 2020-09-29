# git
# Git documents

## this project name is `git` and the username is `gitoption`

***

## Clone a project from the github

`git clone https://github.com/githubusername/projectname.git`

Example clone of the this project:

`git clone https://github.com/gitoption/git.git`

## Add remote url from local machine
`git remote add origin https://github.com/githubusername/projectname.git`

Example add of this project url

`git remote add origin https://github.com/gitoption/git.git`

## Remove remote url from the local machine

`git remote remove origin`

If you want to add another remote url, at first you need to remove the current remote url then to add new url

## Add any changes including files, folders and codes
`git add --all`

## Commit all changes 
`git commit -m 'your commit message here'`

## Push your source code to the github
`git push` (This will push the source codes on the current branch)

`git push origin master` (This will push the source codes to the master branch)

also `git push -u origin master`

## Reset saved but uncommitted code 
First save unsaved work or close and reopen the file, then use this command

`git reset --hard` 

Then use `git pull`

## Restore your currently changed files

`git restore`

## Force to push your code if you think it's ok but it is refusing

`git push -f origin master`

## Create a new branch
`git branch your_new_branch_name`

## Go / switch to a branch
`git checkout your_target_branch_name`

`git switch your_target_branch_name`

## Create a new branch and switch to that branch

`git checkout -b your_new_branch_name`

## Check the changes status
`git status`

## Create an orphan branch 
An ophan branch is completely a new branch without any git history or git commit. You need to commit add all the files to this branch before making a commit

```
git checkout --orphan yourNewBranchNameHere
git add -A
git commit -m 'commitMessageHere'
```

## Remove git commit history from your repo
```
git checkout --orphan newbranch
git add -A
git commit -m 'firstcommit'
git branch -D master
git branch -m master
git remote remove origin
git init
git remote add origin https://github.com/yourUsername/yourGithubRepoName.git
git push -f origin master
git gc --aggressive --prune=all
```
