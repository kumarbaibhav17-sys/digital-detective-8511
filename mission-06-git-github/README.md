# Mission 6 — Git and GitHub

## 1. Task / objective
Understand version control, stage and commit changes, create a branch, open a Pull Request and explain the collaboration workflow.

## 2. Work completed

### Task 6.1: Basic Git workflow
I checked the repository status, staged the README, created a commit with a meaningful message and viewed the commit history.

| Git operation | What it does in my own words |
|---|---|
| Check repository status | Shows which files are changed, staged or untracked, and which branch I am on |
| Stage selected changes | Marks chosen changes to be included in the next commit |
| Create a commit | Saves the staged changes as a snapshot in the history with a message |
| View commit history | Lists the past commits, newest first |

Staging chooses which changes will go into the next commit. Committing actually saves them in the history.

### Task 6.2: Branch
I created a branch named `update-about`, added a "My Learning" section to the root README describing what I have learned, committed it and pushed the branch to GitHub.

### Task 6.3: Pull Request
I opened a Pull Request from `update-about` into `master` with a short description of the README change. PR status: [Merged into master].

A branch is a separate line of work, so I can make changes without affecting the main version. A Pull Request asks to merge one branch into another and lets others review the changes first. They are useful when several people work on the same project because each person's work stays separate until it is reviewed.

### Task 6.4: Git glossary

| Operation | One-line explanation |
|---|---|
| Initialise a repository | Turns a folder into a Git repository so changes can be tracked |
| Check status | Shows changed, staged and untracked files |
| Stage changes | Selects changes for the next commit |
| Commit changes | Saves the staged changes as a snapshot with a message |
| View history | Shows the list of past commits |
| Create or list branches | Lists branches or creates a new one |
| Switch branches | Moves to a different branch |
| Publish changes | Uploads my local commits to GitHub |
| Retrieve remote changes | Downloads and merges new changes from GitHub |

## 3. Commands / tools used
- `git status`, `git add`, `git commit`, `git log --oneline`
- `git switch -c update-about` – created and moved to a new branch
- `git push -u origin update-about` – published the branch
- `git switch master`, `git pull` – returned to the main branch and fetched updates
- Tools: VS Code, GitHub
