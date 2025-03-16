# 📘 Git & GitHub Complete Notes

## 📑 Table of Contents
- [Introduction](#introduction)
- [Git Basics](#git-basics)
- [Git Commands](#git-commands)
- [GitHub Basics](#github-basics)
- [GitHub Commands](#github-commands)
- [Working with Remote Repositories](#working-with-remote-repositories)
- [Branching and Merging](#branching-and-merging)
- [Common Errors and Fixes](#common-errors-and-fixes)
- [Useful Tips](#useful-tips)

---

## 🔰 Introduction

- **Git** is a **version control system** for tracking changes in source code.
- **GitHub** is a **cloud-based hosting platform** for Git repositories to collaborate and share code.

---

## 🔵 Git Basics

- Tracks changes in source code.
- Used for collaboration on coding projects.
- Local operations, distributed system.

---

## 💻 Git Commands

### ✅ Basic Git Setup
```bash
git --version                    # Check Git version
git config --global user.name "Your Name"    # Set Git username
git config --global user.email "you@example.com" # Set Git email
```

### ✅ Initialize Repository
```bash
git init                         # Initialize a local Git repository
```

### ✅ Basic Workflow
```bash
git status                       # Check status
git add <filename>               # Stage file
git add .                        # Stage all files
git commit -m "Commit message"   # Commit changes
```

### ✅ View Logs & History
```bash
git log                          # Show commit logs
git log --oneline                # One-line log format
```

### ✅ File Operations
```bash
git rm <file>                    # Remove file
git mv <old> <new>               # Rename file
```

---

## 🟣 GitHub Basics

- Online platform to store repositories.
- Offers collaboration tools like Pull Requests, Issues, Wiki, Actions.
- Remote storage for Git repositories.

---

## 🟢 GitHub Commands

### ✅ Connecting Local Repo to GitHub
```bash
git remote add origin https://github.com/username/repo.git  # Add remote repo
git remote -v                      # Verify remote URL
```

### ✅ Pushing and Pulling
```bash
git push -u origin main             # Push initial commit to GitHub
git pull origin main               # Pull updates from GitHub
git push                           # Push changes
```

---

## 🌐 Working with Remote Repositories

### ✅ Clone Repositories
```bash
git clone https://github.com/username/repo.git  # Clone repo
```

### ✅ Fetch & Merge Changes
```bash
git fetch                           # Download changes
git merge origin/main               # Merge fetched changes
git pull                            # Fetch + merge in one command
```

---

## 🌿 Branching and Merging

### ✅ Branch Operations
```bash
git branch                          # List branches
git branch <branch-name>            # Create branch
git checkout <branch-name>          # Switch to branch
git checkout -b <branch-name>       # Create & switch to branch
```

### ✅ Merging Branches
```bash
git merge <branch-name>             # Merge branch into current
```

### ✅ Delete Branch
```bash
git branch -d <branch-name>         # Delete branch locally
```

---

## ⚠️ Common Errors and Fixes

| Error                                                                 | Fix Command                                                      |
|----------------------------------------------------------------------|------------------------------------------------------------------|
| `Updates were rejected because the remote contains work...`           | `git pull --rebase origin main`                                   |
| `fatal: refusing to merge unrelated histories`                       | `git pull origin main --allow-unrelated-histories`                |
| `error: failed to push some refs to 'url'`                           | `git pull --rebase origin main` or fix conflicts, then `git push` |
| Mistaken commit message                                              | `git commit --amend`                                              |
| Push to wrong branch                                                 | `git push origin <correct-branch>`                                |

---

## 💡 Useful Tips

- **Check Configurations**
```bash
git config --list                   # List all configurations
```

- **Undo Last Commit (Keep Changes)**
```bash
git reset --soft HEAD~1
```

- **Undo Last Commit (Remove Changes)**
```bash
git reset --hard HEAD~1
```

- **Create .gitignore file** to ignore specific files/folders.

---

## 🚀 Example Workflow

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main
```

---

## 🌟 **Useful Links**
- [Git Official Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/en)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

---

## 📬 Contact
> Made with ❤️ by [Selvaneyas](https://github.com/selvaneyas)

---