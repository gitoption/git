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

## Force to push your code if you think it's ok but it is refusing to push 

`git push -f origin master`
