# Changes in repository

## Pulling from remote to local repo

1. Open a terminal and follow the commands
   > - `git fetch` (checks if there are changes in the remote repository)
   > - `git status` (execute to see the status of your repo to determine if it is ahead or behind a few several commits)
   >   > > read the console and you will find this message:
   >   > > "Your branch is behind 'origin/main' by 1 commit, and can be fast-forwarded.
   > - `git pull` (pull the changes from the remote repository to your local repo)
   > - run `git status` again to see if the pull wass successful.
   >   > > read the console and you will find this message:
   >   > > Your branch is up to date with 'origin/main'. `note: "origin/<main>"` may vary on which branch you are woirking on.
