# Git Commands - DevOps Training Documentation

This document outlines key Git commands learned during AWS & DevOps training. It is structured in the correct order for someone starting from scratch and working toward collaborating with remote repositories.

---

##  Initial Setup

| Command | Purpose |
|--------|---------|
| `git --version` | Check if Git is installed |
| `git config --global user.name "Your Name"` | Set your Git username |
| `git config --global user.email "you@example.com"` | Set your Git email ID |

---

##  Cloning a Repository

| Command | Purpose |
|--------|---------|
| `git clone https://github.com/user/repo.git` | Clone a remote repository to your local machine |

---

##  Working with Branches

| Command | Purpose |
|--------|---------|
| `git branch` | List all local branches |
| `git branch new-branch` | Create a new branch |
| `git checkout branch-name` | Switch to an existing branch |
| `git checkout -b new-branch` | Create and switch to a new branch |

---

##  Managing Remotes

| Command | Purpose |
|--------|---------|
| `git remote -v` | View connected remote repositories |
| `git remote add origin https://github.com/user/repo.git` | Add a new remote repository |
| `git remote set-url origin git@github.com:user/repo.git` | Change remote URL to SSH |

---

##  Staging and Committing Changes

| Command | Purpose |
|--------|---------|
| `git add filename.txt` | Stage a specific file |
| `git add .` | Stage all modified files |
| `git commit -m "message"` | Commit staged changes with a message |

---

##  Modifying the Last Commit

| Command | Purpose |
|--------|---------|
| `git commit --amend -m "New message"` | Modify the last commit message or add forgotten files |
| `git commit --amend -f -m "Forced new message"` | Force amend the last commit (use with caution) |

📌 *Use `--amend -f` only when you fully understand the effect. Avoid on pushed commits unless necessary.*

---

##  Pushing Changes to Remote (SSH)

| Command | Purpose |
|--------|---------|
| `git push origin branch-name` | Push changes to the remote branch |
| `git push origin main` | Push to the main branch |

---

##  Checking Status and Logs

| Command | Purpose |
|--------|---------|
| `git status` | Show the current state of working directory and staging area |
| `git log` | Display full commit history |
| `git log --oneline` | Display concise commit history |

---

##  Merging Branches

| Command | Purpose |
|--------|---------|
| `git merge feature-branch` | Merge a branch into the current branch |

📌 *Always pull the latest changes before merging.*

---

##  Pulling Changes

| Command | Purpose |
|--------|---------|
| `git pull origin main` | Fetch and merge changes from remote to your current branch |

---

##  Fetching Changes (without Merging)

| Command | Purpose |
|--------|---------|
| `git fetch origin` | Download changes from remote without merging |

---

## ✅ Best Practices

- Commit often with clear messages.
- Use branches for each feature or fix.
- Always `pull` before starting new work.
- Use `status` frequently to track changes.
- Avoid using `--amend -f` unless you're sure.
- Prefer SSH over HTTPS for better security.

---

###  Author: [Sai Manikanta]

*Prepared as part of AWS & DevOps Git Training Assignment.*
