# Git Commands

## `git clone`
This command is used to create a full copy of a remote repository on the local machine. The cloned repository contains all the project files, complete history, and branches.

## `git fetch`
This command fetches updates from the remote repository that are not yet in the local repository. It retrieves the updates but does not merge and change the state of your local repository, leaving the current work intact.

## `git pull`
This command fetches updates from the remote repository and merges them into the current local working branch. Essentially, it's a combination of `git fetch` followed by `git merge`.

## `git config --global user.email “xyz@gmail.com”`
This command sets the global configuration for my Git user email to "xyz@gmail.com". This email is attached to all the commits I make on any local repositories, identifying me as the author.

## `git config --global user.name “Dylon-Chan”`
This command sets the global configuration for my Git username to "Dylon-Chan". Similar to the user email, this name is attached to all the commits I make on any local repositories.

## `git add .`
This command stages all the modified, new (untracked) and deleted files in the current directory and its subdirectories, preparing them to be included in my next commit.

## `git commit -m “Update README.md”`
The `git commit` command commits the staged changes (save the changes) to the local repository. Committing is the process of taking a snapshot of the changes. The `-m` flag allows a user to include a message with the commit. This message, `Update README.md` in this case, provides context about the changes. Note that this commit only affects the local repository and does not change the remote repository.

## `git push origin main`
The `git push` command is used to upload the local repository content to a remote repository after the local commits were made. `origin` is the default name Git gives to the server where the repository was cloned from. `main` refers to the branch that the changes are pushed to on the remote repository. `main` is the default main branch but it could be named something else depends on the branch that the user created or worked on.

## `git branch feature3`
This command creates a new branch named `feature3` in the local repository. This is useful for working on new features or bug fixes without affecting the main branch.

## `git checkout feature3`
This command switches the active branch to the branch which was named `feature3`. All the changes made will now be on this branch.

## `git checkout -b feature4`
`git checkout` command is primarily used to switch from one branch to another and the option `-b` tells the Git to create a new branch with the name `feature4`. Essentially, this command is a shortcut for doing a `git branch` followed by a `git checkout` which creates a new branch named “feature4” and immediately switches the active branch to it.

## `git push --set-upstream origin feature3`
The `git push` is used to upload local repository content to a remote repository. `--set-upstream` is the flag that sets the upstream (tracking) reference for the current branch which so that Git will know where to push the commits. `origin` is the name of the remote repository and `feature3` is the name of the branch on the remote repository where user want to push the changes. This command combination is saying: “I want to push the changes from my current local branch to the “feature3” branch on the “origin” remote repository, and I want to set the “feature3” branch on the “origin” repository as the default remote branch for my current local branch”.