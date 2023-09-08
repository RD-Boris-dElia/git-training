# Setup a new repo

The objective of this exercise is to sync a local and a remote (github) repository.

In both cases, you will need to create your github repository separately. You can start with that.

### Setup locally

```
cd <working directory>
git init
```

Then we need to link a remote repository to your local one. 

The remote name does not matter but is named "origin" by default whenever you clone a remote instead of adding it manually.

`git remote add <remote name> <repository url>`

### setup on github

 `git clone <your repo url> (your destination path/directory)`

## push your first file

Create a readme.md file with any text in it

```
git add .
git commit -m "my first commit"
git push
```

Note : You can link your current local repo with a specific remote and branch by running `git branch --set-upstream-to <remote-name>/<branch-name>`

## pull changes from repo

Go to your github repo and create another file.

Call it "feature1.md" and write whatever suits you in it.

Then you want to pull that change to your local repo.

