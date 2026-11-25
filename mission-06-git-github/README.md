# Mission 6 — Git and GitHub

## 1. Task / objective

Understand the basic Git workflow, create and use a branch, document Pull Request use and build a Git command glossary.

## 2. Work completed

### Basic Git workflow

| Git operation | What it does |
|---|---|
| Check repository status | `git status` shows the active branch, tracked changes and untracked files. |
| Stage selected changes | `git add <file>` adds selected changes to the staging area for the next commit. |
| Create a commit | `git commit -m "message"` records a snapshot of staged changes and its message in local history. |
| View commit history | `git log --oneline` displays recent commit IDs and summary messages. |

Staging prepares selected changes for a commit. Committing records that snapshot in repository history. Changes may be unstaged and modified before a commit, while committed history remains recorded.

### Branch and Pull Request activity

The local branch `update-about` was created for the README learning update. A branch is an independent line of repository history for a focused change. A Pull Request asks maintainers to review and merge one branch into another.

The project overview includes the learning summary. This mission's own content and Git glossary are committed independently in `mission-06-git-github/`.

No GitHub remote or authenticated GitHub publishing tool is configured. Publishing the branch and creating a live Pull Request therefore remain external steps.

### Git command glossary

| Operation | One-line explanation |
|---|---|
| Initialise a repository | `git init` creates a local Git repository and starts local version history. |
| Check status | `git status` reports the branch and the state of changed or untracked files. |
| Stage changes | `git add` selects file changes for inclusion in the next commit. |
| Commit changes | `git commit` saves staged changes as a recorded snapshot. |
| View history | `git log` lists commits and their identifying details. |
| Create or list branches | `git branch` creates a branch or lists existing branches. |
| Switch branches | `git switch <branch>` changes the working tree to another branch. |
| Publish changes | `git push` sends local commits and branches to a remote. |
| Retrieve remote changes | `git pull` fetches and integrates remote changes; `git fetch` retrieves them for review before integration. |

## 3. Commands / tools used

- `git status`, `git add`, `git commit`, `git log --oneline`
- `git branch update-about` or `git switch -c update-about`
- `git switch main`
- VS Code — editing project documentation

## 4. My understanding

Git separates working files, the staging area and committed history. Branches keep focused updates independent until review is complete. A remote repository allows a team to share branches and commits, and a Pull Request is the review and merge point for GitHub collaboration.

## 5. Difficulties faced

No GitHub remote or authenticated GitHub publishing tool was available.

## 6. How I resolved them

I completed the local Git workflow and documented the unavailable external publishing step rather than claiming that a live Pull Request was created.

## 7. Evidence / files

- Git glossary and branch / Pull Request explanation in this README
- Local `update-about` branch

## 8. Commit details

- Commit message: `Complete Git and GitHub collaboration mission`
- This commit contains only the `mission-06-git-github/` folder.