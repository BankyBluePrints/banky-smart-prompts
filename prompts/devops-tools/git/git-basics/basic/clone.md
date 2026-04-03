# Clone

## Purpose
Copy an existing Git repository to your local machine and optionally set up the default remote.

## Commands
- `git clone <repo-url>`
  Clone a repository into a new local folder.
  Use when starting work on an existing project.
  Example: `git clone https://github.com/example/project.git`
- `git clone <repo-url> <folder-name>`
  Clone a repository into a specific directory name.
  Use when you want a custom local folder name.
  Example: `git clone https://github.com/example/project.git my-project`
- `git clone --branch <branch> --single-branch <repo-url>`
  Clone only one branch instead of all branches.
  Use when you only need a specific branch.
  Example: `git clone --branch release/1.0 --single-branch <repo-url>`

## Notes
- Cloning downloads the repository history and sets `origin` automatically.
