# GitHub Beginners Cheat Sheet — VS Code

---

## Setup

| Task | How |
|------|-----|
| Install Git | [git-scm.com/downloads](https://git-scm.com/downloads) |
| Install VS Code | [code.visualstudio.com](https://code.visualstudio.com) |
| Set your name | `git config --global user.name "Your Name"` |
| Set your email | `git config --global user.email "you@example.com"` |
| Check config | `git config --list` |

---

## VS Code Git Panel

Open the **Source Control** panel with `Ctrl+Shift+G` (Mac: `Cmd+Shift+G`)

| Icon / Action | What it does |
|---------------|--------------|
| Source Control icon (branch icon) | Opens Git panel |
| `+` next to a file | Stages the file (git add) |
| `✓` checkmark (top) | Commits staged changes |
| `...` menu | Access push, pull, branch, stash, and more |
| Inline diff view | Click any changed file to see what changed |

---

## Core Git Commands (Terminal in VS Code)

Open the terminal with `` Ctrl+` `` (backtick)

### Starting Out

```bash
git init                    # Initialize a new repo in current folder
git clone <url>             # Copy a remote repo to your machine
```

### Daily Workflow

```bash
git status                  # See what files changed
git add <file>              # Stage a specific file
git add .                   # Stage all changed files
git commit -m "message"     # Save staged changes with a message
git push                    # Upload commits to GitHub
git pull                    # Download latest changes from GitHub
```

### Branches

```bash
git branch                  # List all branches
git branch <name>           # Create a new branch
git checkout <name>         # Switch to a branch
git checkout -b <name>      # Create AND switch in one step
git merge <branch>          # Merge a branch into current branch
git branch -d <name>        # Delete a branch (safe)
```

### Viewing History

```bash
git log                     # Full commit history
git log --oneline           # Compact one-line history
git diff                    # See unstaged changes
git diff --staged           # See staged changes
```

---

## GitHub Workflow (Fork → Clone → PR)

```
1. Fork the repo on GitHub (click "Fork" button)
2. Clone your fork locally:
   git clone https://github.com/YOUR-USERNAME/REPO.git

3. Create a branch for your changes:
   git checkout -b my-feature

4. Make changes, then stage and commit:
   git add .
   git commit -m "Add my feature"

5. Push your branch to GitHub:
   git push origin my-feature

6. Open a Pull Request on GitHub
   → Go to the original repo → "Compare & pull request"
```

---

## VS Code Extensions (Recommended)

| Extension | Why it helps |
|-----------|--------------|
| **GitLens** | See who changed each line, rich history |
| **GitHub Pull Requests** | Manage PRs directly in VS Code |
| **Git Graph** | Visual branch/commit tree |

Install via `Ctrl+Shift+X` → search extension name

---

## Common Mistakes & Fixes

| Problem | Fix |
|---------|-----|
| Committed to wrong branch | `git checkout correct-branch` then `git cherry-pick <commit-hash>` |
| Want to undo last commit (keep changes) | `git reset --soft HEAD~1` |
| Want to discard all local changes | `git checkout -- .` |
| Merge conflict in VS Code | Open conflicting file → click "Accept Current/Incoming/Both" in the editor |
| Forgot to pull before pushing | `git pull --rebase` then `git push` |

---

## Key Vocabulary

| Term | Meaning |
|------|---------|
| **Repository (repo)** | A project folder tracked by Git |
| **Commit** | A saved snapshot of your changes |
| **Branch** | An independent line of development |
| **Main / Master** | The default primary branch |
| **Fork** | Your personal copy of someone else's repo |
| **Clone** | Download a repo to your local machine |
| **Push** | Upload your local commits to GitHub |
| **Pull** | Download remote commits to your machine |
| **Pull Request (PR)** | A request to merge your branch into another |
| **Merge** | Combine changes from two branches |
| **Staging Area** | Where you prepare changes before committing |

---

## Quick Reference — VS Code Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+Shift+G` | Open Source Control panel |
| `` Ctrl+` `` | Open terminal |
| `Ctrl+Shift+P` | Command Palette (run any command) |
| `Ctrl+Shift+X` | Extensions marketplace |
| `F1` → "Git: Clone" | Clone a repo via command palette |

> Mac users: replace `Ctrl` with `Cmd`

---

*Happy coding!*
