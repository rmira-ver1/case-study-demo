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

# Switching from branch to branch

1. In your terminal follow these commands:
   > - git branch -a (view all local branches)
   >   > if you can see more that one local branch you can switch to which branch you want to switch with.
   >   > `feat-001/branch-policy` > > `* main` > > `remotes/origin/HEAD -> origin/main` > > `remotes/origin/feat-001/branch-policy` > > `remotes/origin/main`
   >   > if the text is green and has an asterisk on the left side of the name, it signifies that you are currently on that branch
   > - to switch branches execute the command **git checkout feat-001/branch-policy** in this case we are switching into feat-001/branch-policy which is above main and does not have any color.
   >   after executing the command it shows this message:
   >   > `Switched to branch 'feat-001/branch-policy'` (this message tells you that you have successfully switched from one branch to another in our case it is from main to feat-001/branch-policy)
   >   > `Your branch is up to date with 'origin/feat-001/branch-policy'.` (this tells you if the local branch is updated and is not behind the online repo in github.com)
   >   > note: **you can switch to any branch you like as long as it has been tracked by your local machine**
   > - to switch back to the main branch execute git **checkout main** > `note: the red text that starts with remotes/origin talks about the branches that are found in the remote repo in github.com in this case it is the project "case-study-demo"`
