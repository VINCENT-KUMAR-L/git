## Learning the Git and GitHub

## This is the main Branch
## This is Bug Branch
## This is new bug branch created from bug

Got it — I’ll clean up the text, fix grammar and clarity issues, and format it properly as a **README.md** file. Here’s the polished version you can upload directly to GitHub:

```markdown
# Git & GitHub Guide

## What is Git?
Git is a version control system that tracks file changes and versions. It enables functionalities such as commits, merges, and pull requests.

## What is GitHub?
GitHub is a cloud-based platform for hosting Git repositories and collaborating with others.

---

## Configuration

Set global configuration:
```bash
git config --global user.name "YourName"
git config --global user.email "YourEmail"
```

Verify configuration:
```bash
git config user.name
git config user.email
```

---

## Initialization

Set default branch and initialize repository:
```bash
git config --global init.defaultBranch main
git init
```

---

## Common Commands

- `git status` → Shows status of files (staged, unstaged, untracked).
- `git add filename` or `git add .` → Moves changes from working directory to staging area.
- `git commit -m "message"` → Records staged changes into repository history.
- `git log` → Displays commit history.
- `git checkout branchName` or `git checkout commitID` → Switches to branch or commit.
- `git checkout main` → Switches to main branch.
- `git checkout -f main` → Discards uncommitted changes and switches to main branch.

---

## Linking Local and Remote Repository

1. Create a new repository on GitHub.
2. Copy the repository link and add it locally:
   ```bash
   git remote add origin https://github.com/username/repo.git
   ```
3. Rename branch to `main`:
   ```bash
   git branch -M main
   ```
4. Push changes:
   ```bash
   git push -u origin main
   ```

---

## Branch Management

| Command | Action | Notes |
|---------|--------|-------|
| `git branch new-feature` | Creates a new branch | Does not switch to it |
| `git checkout -b new-feature` | Creates and switches to new branch | Older method |
| `git switch -c new-feature` | Creates and switches to new branch | Modern, clearer syntax |

Other branch-related commands:
- `git checkout new-branch source-branch` → Creates branch from source.
- `git push -u origin branch-name` → Push branch to remote (first time).
- `git fetch` → Retrieves remote branches.
- `git pull` → Gets latest changes from remote.
- `git stash` → Temporarily saves uncommitted changes.
- `git stash list` → Lists stashed changes.
- `git stash apply stashID` → Applies stashed changes.

---

## Reset & Revert

- `git reset commitID` → Moves to specific commit (unstaged).
- `git reset --soft commitID` → Moves to commit (staged).
- `git reset --hard commitID` → Moves to commit (discard changes).
- `git revert commitID` → Creates a new commit that undoes changes (keeps history).

---

## Notes
- Use **reset** when you want to discard history.
- Use **revert** when you want to undo changes but keep history intact.
- Prefer `git switch` over `git checkout` for clarity when working with branches.
```

---

✅ This version is corrected, concise, and properly formatted for a **README.md** file.  

Would you like me to also add a **step-by-step practice workflow section** (like creating a repo, branching, committing, pushing, and merging) so your README doubles as a hands-on guide?