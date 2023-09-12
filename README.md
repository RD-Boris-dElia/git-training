# git-training

Welcome to this git hands-on training !

Everything can be done either through your IDE, your cmd-line interface, git bash, git GUI, or whichever solution you want to try.

It doesn't matter what method you use, I just hope it helps your understand how to properly use git and gain proficiency.

## Exercises

### 1. [setup](./exercises/setup.md)

### 2. [branches](./exercises/branches.md)

## Helpful commands

Here is the [official documentation](https://git-scm.com/docs) for all commands. 

#### list remotes

```console
$ git remote -v
github  https://github.com/RD-Boris-dElia/git-training (fetch)
github  https://github.com/RD-Boris-dElia/git-training (push)
```

#### [git log](https://git-scm.com/docs/git-log) and [git diff](https://git-scm.com/docs/git-diff)

You can list commits that happened on the repository with the `git log` command. It's always in descending order based on timestamp.

But you can also filter based on your needs :

- Everything that happened for a branch `git log <branch name>`
- Search in commit messages :`git log --grep="search string"`
- Search in code :`git log -S"search string"`
- Search in code (Regexp) :`git log -G"regexp"`

And much more. Here's a cheatsheet of most useful commands : https://devhints.io/git-log

Git log is useful to find specific commits but you won't know what did this commit introduce in the code.
For that, `git diff <commit>` is the right command to use. By default, it diffs the code against your HEAD.

Commits are identified by a unique sha or hash (ex :431df8fddd622ecb1b31f0b669952060c129b5c3)

- diff a commit's change only : `git diff <commit>^!`
- diff local changes against a remote current state `git diff origin/main` or `git diff <remote>/<branch>`
