# Practice repository to start learning Git

##Commands used

- git init: Create a new git repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show a history (aka "logo") of projects commits
- git show: Show a singl commits
- git diff: Show the difference between commits, the working directory, and the staging areas
- git checkout: Checkout out branch (update HEAD and apply changes to working directory)
- git checkout -b: Create branch, then check it out
- git branch -c: Create a branch
- git branch: list branches
- git merge: Merge changes from different branches
- git stash: Stash changes from working directory
- git stash list: List stashes
- git stash pop: Apply stashed changes to working directory
- git remote add <remote> <url>: ADd a new <remote> at <url>
- git remote -v: List remote repositories
- git push -u <remote> <branch>: Push <branch> to <remote>, and set default upstream for <branch>
- git fetch: Fetch changes from remote repository
- git pull: Fetch and then Merge

## What's a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we're "on" that branch.
 When we make a commit while we're on a branch, 
the branch is updated to ref(er) to the new commit. Git commands like 'status', 'log', and 'branch' use HEAD. '

## What's HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit...mre on that later). 
Git commands like 'status', 'log', and 'branch' use HEAD. 'git checkout' updates HEAD to ref(er) to a different branch.

## Commit messages

Default editor is vim (this can be changed)
	- 'i' to enter *insert* mode
	- Type commit messages
	- 'Esc' -> ':wq' -> 'Enter' to write message and quit
Or use 'git commit -m "<message>"'

- First line should be clear, accurate, and concise
- Use proper spelling, grammar, and punctuation
- Don't end with a '.'

For more advice, see: https://chris.beams.io/posts/git-commit/

## Merging

Merging means to bring the changes from one branch into another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.


## What's a remote?

A remote repo is one hosted somewhere other than our local machine. We can add remotes with 'git remote add', and set up *tracking branches* to track differences between our local and remote repostirories.

We push to remotes with 'git push', and fetch from them with 'git fetch'. WE can also fetch and merge in one set with 'git pull'.