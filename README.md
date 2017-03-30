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
