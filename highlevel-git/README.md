# Version Control and Git
## What is Version Control?
At a high level, Version Control (often abreviated as VCS, or "Version Control System") is just a backup system for programming. Imagine writing some code to make a mobile app. You reach a point where everything works stably, so you want to save your progress. Then you add a new feature that introduces some bugs. You can't present your application to your friends now that it has bugs, so you want to revert back to the stable version of your application. But, your new feature is almost bug-free, so you don't want to lose those changes either. Here's where Version Control comes to the rescue. 

## Git
Git is one of many VCS, and is NOT to be confused with GitHub. The difference is simple: 
* Git is the actual version control software
* GitHub is a website/hosting service for Git repositories

So if my team and I are writing code together, we would all "commit" our changes locally and "push" those changes to GitHub. With the project being hosted on GitHub, developers are free to download, or "clone", their projects on whatever computer they want. You can think of GitHub like Google Drive for remotely saving different iterations of code. 

## Core git Concepts
In order to understand how to use git, you need to know a few definitions.

* Repository
* Staging
* Commit
* Index
* Head
* Branch

### Repository
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

The `.git/` folder is what makes a directory a git repository. It contains many helpful things that we will talk about later (including but not limited to): branches, objects, refs, HEAD, index, and config.


