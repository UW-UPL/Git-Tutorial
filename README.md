# Git/Github Handbook
Created by the UPL

## Before We 'Git' Started
Git has a very, very steep learning curve. There's a lot of jargon that flies around, and can feel overwhelming. Don't feel like you're dumb or not supposed to be a CS major if you don't get this right away. It takes time, and lots of practice. To help get you wrap your head around Git, we're going to use an analogy throughout this tutorial. We're going to make a coloring book (literally, we're going to have doodles) to demonstrate the logic of Git, because we're all familiar with the concept of a coloring book. This coloring book has one slight difference though - it's really more of a journal. Our book is initially empty, and we'll be adding pages to it instead of filling in existing lines with color. 

## What is Git and what is Github, and why do we need this?
According to [Git's website](https://git-scm.com/), "Git is a free and open source *distributed version control system* designed to handle everything from small to very large projects with speed and efficiency." The two main parts to that description are distributed, and version control system. Let's talk about what a version control system, or VCS, is. 
### VCS
A VCS, at a high level, is very intuitive. Here's an example of what a VCS does.

Let's say we have a picture in our coloring book, and one day we make the background red and save that to our VCS. Then we decide to add some Bucky Badger heads and save that to the VCS. Next we add a Motion W, and heck why not one of those silly Gopher M's. After that we add some text at the bottom like 'Go Bucky!'. 

If we didn't save our picture to a VCS, then one of two things would happen. Either we'd only have one file that represents one version, the latest version, or we would have a cluttered directory because we saved each iteration to a different file name.

If we saved only one file, we would have no concept of how the picture was made, in what order the elements were added, and no way to restore the picture to a previous state. 

Our working directory would look something like this
```
bucky.psd
```
Here are the pros and cons of working like this.
* Pro
  * Clean working directory
* Con
  * No way to rollback changes

Now let's look at the alternative: we save files at each step. Our working directory would look something like below. 
```
red_background.psd
red_with_bucky.psd
red_with_bucky_with_motion_w.psd
...
...
...
```
Here are the pros and cons to working like this.
* Pro
  * We have a way of versioning our picture
* Con 
  * Our working directory is a mess
  
How do we combine the pros and eliminate the cons of each? VCS! A VCS will allow us to version a file so that we can track changes throughout it's lifespan. We don't need to create new copies of the file, we just need to save to the VCS so that it can track the changes. 



### Distributed


## Table of Contents  
1. [Version Control and Git](https://github.com/UW-UPL/Git-Tutorial/blob/master/highlevel-git/README.md#version-control-and-git)  
    1. [What is Version Control?](https://github.com/UW-UPL/Git-Tutorial/blob/master/highlevel-git/README.md#what-is-version-control)
    2. [Git](https://github.com/UW-UPL/Git-Tutorial/blob/master/highlevel-git/README.md#git)
    3. [Git Core Concepts](https://github.com/UW-UPL/Git-Tutorial/blob/master/highlevel-git/README.md#core-git-concepts)
    4. [Repository](https://github.com/UW-UPL/Git-Tutorial/blob/master/highlevel-git/README.md#repository)

## Contributors
[Evan Kivolowitz](https://github.com/ekivolowitz)  
[Aaron Levin](https://github.com/awlevin)  
[Christian Borst](https://github.com/ChristianBorst)  
