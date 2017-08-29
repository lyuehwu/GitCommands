# Git Commands

### Creating repository online for the <b>first time</b>!

``` sh
$ touch README.md
$ git init
$ git add README.md
$ git add -u # when you have deleted a local file you want to remove
$ git commit -m "first commit"
$ git remote add origin https://github.com/lyuehwu/GitCommands.git
$ git push -u origin master
#put in username  & password
```

### When adding on tto your repository online with changes
``` sh
$ git add .
$ git commit -m 'what has changed'
$ git push
#put in username  & password
```
### No more username & password input for every push

```sh
$ NEED TO SET SSH KEY FIRST!!!
$ git remote set-url origin git@github.com:lyuehwu/GitCommands.git
$                           git@github.com:lyuehwu/GitCommands.git

```

### Working together from perspective of person that doesn't have the main rrepo

```sh

#fork repo you want to work on
$git clone https://github.com/lyuehwuFACK/GitCommands.git
```

### WAnt to remove a file from online github repo but keep it locally

```sh
$ git rm --cached localFileName
$ add localFileName to .gitignore file and then commit these changes
```

### Commands for fixing problems

```sh
# undo multiple commits
$ git reset --hard commitSHA###... = changes staging index and local folder to match online repository commit

```
# removing 3 commits from online github repo
```sh
$ git push -f origin HEAD^^^:branchNameToUndoLast3Pushs
```
### Branch Commands
```sh
# creating a new branch
$ git branch #list all branches in working folder
$ git branch newBranchName
$ git checkout newBranchName # adds new branch newBranchName
$ git push origin newBranchName #adds new branch to github repo
# push commits

# mergin new branch to old branch
$ git checkout oldBranchName
$ git merge newBranchName #
$ git branch -d branchName ToDelete #delete branch while you are on a different branch
```




