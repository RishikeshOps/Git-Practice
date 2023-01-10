# Day 11 Task: Advance Git & GitHub for DevOps Engineers: Part-2

## Git Stash:
Git stash is a command that allows you to temporarily save changes you have made in your working directory, without committing them. This is useful when you need to switch to a different branch to work on something else, but you don't want to commit the changes you've made in your current branch yet.

To use Git stash, you first create a new branch and make some changes to it. Then you can use the command git stash to save those changes. This will remove the changes from your working directory and record them in a new stash. You can apply these changes later. git stash list command shows the list of stashed changes.

You can also use git stash drop to delete a stash and git stash clear to delete all the stashes.

## Git Reset:
Git reset is a command that allows you to undo commits and bring your branch to a previous state. It has two options: --soft and --hard, which determine whether the changes in the commit are kept or discarded.

When you use git reset --soft option, it undoes the last commit, but keeps the changes in the working directory. This allows you to make additional changes, or to create a new commit with the changes included.

On the other hand, when you use git reset --hard option, it undoes the last commit and discards the changes in the working directory. This is a more destructive operation and should be used with caution as it permanently discards changes.

## Git Rebase:
Git rebase is a command that allows you to integrate changes from one branch into another. It works by "moving" the commits on the branch you are rebasing to be based on the tip of the branch you are rebasing onto. This effectively replaces the original commits on the branch you are rebasing with new commits that have the same changes but with different SHA-1 identifiers.

To use Git rebase, you first create a new branch and make some commits to it. Then you create another branch, make some commits to it, and use git rebase <branch_name> to integrate the changes from the first branch into the second. When conflicts occur during the rebase process, you will need to resolve them, you can use the commands git status, git diff, and git add to identify and resolve conflicts.

## Git Merge:
Git merge is a command that allows you to bring changes from one branch into another. When you use git merge <branch_name>, it creates a new commit that has two parents: one for the tip of the branch you are merging in and one for the current commit on the branch you are merging into.

## Cherry-pick:
Git cherry-pick is a command that allows you to select specific commits from one branch and apply them to another. This can be useful when you want to selectively apply changes that were made in one branch to another.

To use git cherry-pick, you first create two new branches and make some commits to them. Then you use git cherry-pick <commit_hash> command to select the specific commits from one branch and apply them to the other.

## Resolving Conflicts:
Conflicts can occur when you merge or rebase branches that have diverged, and you need to manually resolve the conflicts before git can proceed with the merge/rebase.
git status command shows the files that have conflicts, git diff command shows the difference between the conflicting versions and git add command is used to add the resolved files.


# Task-01 


