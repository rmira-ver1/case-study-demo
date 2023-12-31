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
   >   > > Your branch is up to date with 'origin/main'. `note: "origin/<main>"` may vary on which branch you are working on.

## Pushing from local repo to remote repo

1.  Open a terminal and follow the commands:
    > - git status (to view the status of your files in the local repo)
    >   > > `note if the text is red it means that you haven't added that file yet, "it's just like online shopping you need to add to cart the product before buying it."`
    > - git add `<filename>` example **docs/repository_changes.md** you can copy the text after **"modified"** and replace the `<filename>` placeholder.
    >   > > `note: alternatively you could also do "git add ." if you have to add multiple files, this is only applicable if you are creating the file for the first time, "git add ." is not a good practice since some files might have different changes from each other but it varies from situation to situation`
    > - git commit -m "commit message" (replace commit message about what has changed or what happened in that file)
    > - git push (push the changes to the remote repository)
