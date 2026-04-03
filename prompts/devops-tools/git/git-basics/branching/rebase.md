# Rebase

## Purpose
Replay commits on top of another branch to keep history cleaner and more linear.

## Commands
- `git rebase <base-branch>`
  Reapply the current branch commits on top of another branch.
  Use when updating a feature branch from `main`.
  Example: `git rebase main`
- `git rebase -i HEAD~<n>`
  Interactively edit, squash, or reorder recent commits.
  Use before sharing or merging a branch.
  Example: `git rebase -i HEAD~3`
- `git rebase --continue`
  Continue a rebase after resolving conflicts.
  Use during conflict resolution.
- `git rebase --abort`
  Cancel the rebase and restore the branch to its previous state.
  Use when the rebase should not proceed.

## Notes
- Do not rebase shared public history unless your team expects it.
- A rebase followed by push may require `git push --force-with-lease`.
