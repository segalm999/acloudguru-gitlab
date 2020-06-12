# Practice repository to start learning Git

##Commands used

- git init: Create a repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Set or get configuration
- git log: Show history of projects commits
- git branch: list branches
- git checkout -b: Create branch, then check it out

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
