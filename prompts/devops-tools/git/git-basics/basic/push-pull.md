# Push and Pull

## Purpose
Send local commits to a remote repository and bring remote changes into your branch.

## Commands
- `git push`
  Push the current branch to its tracked remote branch.
  Use after committing local work.
- `git push -u origin <branch>`
  Push a new branch and set upstream tracking.
  Use the first time you publish a branch.
  Example: `git push -u origin feature/login`
- `git pull`
  Fetch remote changes and merge them into the current branch.
  Use to update your branch quickly.
- `git pull --rebase`
  Fetch remote changes and replay your local commits on top.
  Use to keep history linear on feature branches.

## Notes
- Pulling can create merge commits depending on repo settings and local history.
- Avoid `git push --force`; prefer `git push --force-with-lease` only when you intentionally rewrote history.
