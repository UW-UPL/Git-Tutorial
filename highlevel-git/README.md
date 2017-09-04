# Core git Concepts
In order to understand how to use git, you need to know a few definitions.

* Repository
* Staging
* Commit
* Index
* Head
* Branch

## Repository
A git repository is the collection of a bunch of files tracked by git for a project. Think of this as your working directory for your project.

If you were on your desktop and ran the following code, you would create a git repository called MyFirstRepository. Simply having a folder named `MyFirstRepository` does not it a git repository. What makes a folder a git repository is the `git init` command. Before you run the `git init` command, there is nothing but an empty folder when we viewed the directory with `ls -a`. Ater running `git init` and another `ls -a`, we'll see that there is a `.git/` folder. (Side Note: You need the `-a` flag with the `ls` command because that will specify to the `ls` command that it should include  hidden files and folders. Any hidden file or folder will begin with a '.'.)
```
cd ~/Desktop/
mkdir MyFirstRepository
cd MyFirstRepository
ls -a
git init
ls -a
```

The `.git/` folder is what makes a directory a git repository. It contains many helpful things that we will talk about later: branches, objects, refs, HEAD, index, and config.


