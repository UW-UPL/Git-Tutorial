# Using GitHub

## Two Approaches
There are two main approaches to getting a repository up-and-running with GitHub. In short, they are:

1. GitHub-First
2. Local-First

These imply where the repositories are first instantiated. These two approaches are slightly different (the first is marginally easier to setup, but is only viable if you haven't actually started your project yet). Thus, it is up to you, the programmer, to be prepared to handle either scenario!


### Approach #1 (GitHub first, project not yet started)
Head over to GitHub.com and navigate to the "repositories" tab of your profile. You should see a "New" button that looks like this:

![new-repo-button](new-repo-button.png)

Click the button and fill out the details of your repo. We recommend leaving out the README and .gitignore for the sake of simplicity. 

![create-new-repo](create-new-repo.png)

When your empty repository has been created, you should arrive at a screen like this:

![empty-repo](empty-repo.png)

Copy the HTTPS URL from the "Quick setup" box and head over to terminal. Type `git clone <insert-URL-here>` and press enter. Your computer will download the "empty" repository, and then you're ready to use it to start creating files, staging them, and committing them under version control!

Quick side note: why did we put "empty" in quotations? Take a second to think about it.


...
1 second later...
...


It's because there's a hidden `.git/` folder in your repository, even though it looks like it's empty! Remember, this folder stores all of the version history for your project!

### Approach #2 (local first, project probably already started)
The second approach is to create a Git repo locally, before pushing it to GitHub. In any folder on your computer (empty or not), type `git init` to create a hidden `.git/` folder that will maintain all of your version history! 

Congrats! You're now perfectly capable of using Git to make commits, branches, etc. But, your project doesn't exist on GitHub yet, so you'll only be able to work on it by yourself, and `git push` won't do much of anything. Sad!

Let's link this baby to GitHub. Head over to GitHub and create your new repository. Copy the HTTPS URL of your new project, and head back to your local repository via the commandline. Simply type `git remote add origin <URL>`, press enter, and you're ready to `git push` your commits to GitHub! Go ahead, stage something (`git add <file>`), commit it (`git commit -m "<commit message>"`) and `git push` it to GitHub!

Next, we'll talk about some common problems that arise when working with teammates, and how you can resolve them as easily as possible!
