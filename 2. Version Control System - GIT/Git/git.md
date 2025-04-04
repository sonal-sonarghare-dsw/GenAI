
## 🔧 What is Git?

Git is a **distributed version control system (DVCS)** that helps teams:
- **Track changes** in source code during development.
- **Collaborate** by managing different versions of code (branches).
- **Experiment safely** with code before merging into the main codebase.
- Work with **local repositories** and sync with **remote repositories** (like GitHub, GitLab).

---

## 🛠️ Step 1: Git Setup (One-Time Only)

Configure Git globally (runs once per machine):

```bash
git config --global user.name "Username"
git config --global user.email "Email"
git config --global color.ui auto
```

To check config:
```bash
git config --list
```

---

## 📁 Step 2: Create or Clone a Git Repository

### A. Initialize a New Repository

```bash
mkdir my-project
cd my-project
git init   # Starts a new Git repo
dir /a      # Shows hidden `.git` directory
```

### B. Clone a Remote Repository

```bash
git clone https://github.com/username/repo.git
cd repo
```

---

## 🔄 Step 3: Git Workflow

Git tracks your files through 3 **main states**:

| State     | Description                                   |
|-----------|-----------------------------------------------|
| Modified  | File has been changed but not staged yet.     |
| Staged    | File is added to the staging area.            |
| Committed | Changes are saved in the Git repository.      |

---

### 🔧 Workflow Example

```bash
# Check current status
git status

# Add files to staging
git add file1.txt file2.txt  # Specific files
git add .                    # Everything
git add *.txt                # All .txt files

# Again Check current status
git status

# Commit staged changes
git commit -m "Initial commit"
```

---

## 🌿 Step 4: Branching & Merging

### Create and Work with Branches

```bash
git branch                  # List branches (* = current)
git branch feature-x        # Create a new branch
git checkout feature-x      # Switch to the branch

# Shortcut to create + switch
git checkout -b feature-x
```

### Merge Branches

```bash
git checkout main           # Switch to main branch
git merge feature-x         # Merge feature-x into main
```
### Push Branch to Remote
```bash
git push origin <branch-name>
```
###  Delete a Branch

```bash
git branch -d feature-x
```

---

## 🌐 Step 5: Work with Remote Repositories

### 🔗 Add a Remote Repo (if not added)

```bash
git remote add origin https://github.com/username/repo.git   # It connects your local Git repository to a remote GitHub repository.
```

### 📤 Push Changes to Remote

```bash
git push origin main            # Push to main branch
git push origin feature-x       # Push a specific branch
```

### 📥 Pull Updates from Remote

```bash
git pull origin main            # Pull latest from main
```

---

## 🔍 Step 6: Inspect and Troubleshoot

### View Commit History

```bash
git log                        # Full commit log
git log --oneline              # Short version
```

### View Changes (Diff)

```bash
git diff                       # Show unstaged changes
git diff --staged              # Show staged vs last commit
```

---

## 🚫 Step 7: Undo & Clean

### Unstage Files

```bash
git reset HEAD <file>
```

### Discard File Changes

```bash
git restore <file>
```

### Remove Git from Folder

```bash
rm -rf .git
```

---

## 🧾 Bonus: .gitignore File

Create a `.gitignore` to prevent tracking sensitive or unnecessary files:

```plaintext
node_modules/
*.log
.env
.DS_Store
*.pyc
```

---

## ✅ Summary Table of Commands

| Task                            | Command                               |
|----------------------------------|----------------------------------------|
| Initialize repo                  | `git init`                             |
| Clone repo                       | `git clone <URL>`                      |
| Check status                     | `git status`                           |
| Stage file(s)                    | `git add <file>` / `git add .`         |
| Commit changes                   | `git commit -m "msg"`                  |
| Create branch                    | `git branch <branch>`                  |
| Switch branch                    | `git checkout <branch>`                |
| Create + switch branch           | `git checkout -b <branch>`             |
| Merge branches                   | `git merge <branch>`                   |
| View log                         | `git log` / `git log --oneline`        |
| Push to remote                   | `git push origin <branch>`             |
| Pull from remote                 | `git pull origin <branch>`             |
| Remove Git from folder           | `rm -rf .git`                          |

---
