# Branching in github

## Creating a branch

1. go to the main page of the repository [Link to the main page](https://github.com/rmira-ver1/case-study-demo)
   > - under the name of the repo there is a button with the name "main" on it, click the drop down menu and select **"View all branches"**
   > - Click the button **New Branch**
   >   > - give your branch a name ex: **feat-001/branch-policy**
   >   > - select the branch source as **main**
   >   >   > `note: the main branch is the most important branch of all since this will contain the files or codes that will be deployed, never commit changes directly on the main branch do a pull request instead.`

# Pulling remote branch into your local machine

1. Open a terminal and follow the commands:
   > - git branch -a
   >   > you will be greeted by this console log:
   >   > `* main` > > `remotes/origin/HEAD -> origin/main` > > ` remotes/origin/main**`
   >   > as you can see it only points to the main branch, it means that your local machine is only seeing the main branch
   > - Now execute the command **git fetch** which checks if there are changes within out repository/project. then it will return this text:
   >   > From github.com:skynet6969/case-study
   >   > `* [new branch]      feat-001/branch-policy -> origin/feat-001/branch-policy`
   >   > this means that the branch that we have created is now visible to our machine and is now tracking it, and if you'll do another **git branch -a** > > `* main` > > `remotes/origin/HEAD -> origin/main` > > `remotes/origin/feat-001/branch-policy` > > `remotes/origin/main`
   >   > we can see that **remotes/origin/feat-001/branch-policy** has been added and is being tracked by our local machine.
   > - to jump into this branch just do git checkout **feat-001/branch-policy**
   >   > you will be greeted by this message:
   >   > `Switched to a new branch 'feat-001/branch-policy'` > > `branch 'feat-001/branch-policy' set up to track 'origin/feat-001/branch-policy'`
   >   > it means that you have successfully transferred to the branch that you have created also in visual studio code there is an indicator on the bottom left that tells you which branch you are currently in if it says `main*` then it means that you are currently in the main branch.
