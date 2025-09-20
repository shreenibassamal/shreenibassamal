# 1\. Git 🌀

## 1.1 What is Git? 📂

Git is a **distributed version control system**. It’s mainly used to:

* Track changes in code 📝
    
* Manage different versions of a project 🔀
    
* Allow multiple people to work on the same codebase at the same time without conflicts 👥
    

## 1.2 GitHub 🌐

GitHub is a **cloud-based platform** built on top of Git. It allows us to:

* Store repositories online ☁️
    
* Collaborate with team members 🤝
    
* Review code through pull requests 🔍
    
* Manage issues or tasks 📌
    

👉 **In short**: Git = Version Control ⚡ | GitHub = Collaboration Platform 🚀

---

## 1.3 My Project Experience 💼

In my projects, we used Git with GitHub:

* Created **branches** for new features or bug fixes 🌱
    
* Merged them into **main branch** via pull requests 🔄
    
* Handled **conflicts** when multiple people worked on the same files ⚔️
    
* Git helped us to **rollback changes**, **track history**, and improve collaboration ✅
    

---

## 1.4 Git Branching and Merging Workflow 🌳

| Step | Command / Action | Description |
| --- | --- | --- |
| 1 | `git init` | Initialize empty Git repository ⚡ |
| 2 | `git checkout -b b1` | Create and switch to branch `b1` 🌱 |
| 3 | Create `b1.txt` in Notepad ✍️ | Write one line in the file and save |
| 4 | `git add b1.txt` | Stage the file for commit 📦 |
| 5 | `git commit -m "Added b1.txt"` | Commit the file to `b1` branch ✅ |
| 6 | `git checkout -b b2` | Create and switch to branch `b2` 🌱 |
| 7 | Create `b2.txt` in Notepad ✍️ | Write one line in the file and save |
| 8 | `git add b2.txt` | Stage the file 📦 |
| 9 | `git commit -m "Added b2.txt"` | Commit the file to `b2` branch ✅ |
| 10 | `git checkout -b b3` | Create and switch to branch `b3` 🌱 |
| 11 | Create `b3.txt` in Notepad ✍️ | Write one line in the file and save |
| 12 | `git add b3.txt` | Stage the file 📦 |
| 13 | `git commit -m "Added b3.txt"` | Commit the file to `b3` branch ✅ |
| 14 | `git checkout master` | Switch back to master branch ⬅️ |
| 15 | `git merge b1` | Merge `b1` into master 🔀 |
| 16 | `git merge b2` | Merge `b2` into master 🔀 |
| 17 | `git merge b3` | Merge `b3` into master 🔀 |
| 18 | `git branch -d b1` | Delete branch `b1` 🧹 |
| 19 | `git branch -d b2` | Delete branch `b2` 🧹 |
| 20 | `git branch -d b3` | Delete branch `b3` 🧹 |
| 21 | `ls` / `cat b1.txt b2.txt b3.txt` | Verify all files are present in master 👀 |

---

## 1.5 Common Git Commands 🛠️

### 🔹 Repo Setup

| Command | Description |
| --- | --- |
| `git init` ⚡ | Initialize a new Git repository |
| `git clone <repo_url>` 🔗 | Clone an existing repository |

### 🔹 Configuration ⚙️

| Command | Description |
| --- | --- |
| `git config --global` [`user.name`](http://user.name) `"Name"` | Set username for all repos |
| `git config --global` [`user.email`](http://user.email) `"Email"` | Set email for all repos |

### 🔹 Status & Info 📋

| Command | Description |
| --- | --- |
| `git status` | Show working directory status |
| `git log` 📜 | Show commit history |
| `git log --oneline --graph --all` 🌳 | Compact history in tree format |
| `git diff` | Show unstaged changes |

### 🔹 Staging & Commit ✅

| Command | Description |
| --- | --- |
| `git add <file>` 📦 | Add file(s) to staging area |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Commit staged changes |
| `git commit --amend` ✏️ | Edit last commit or add forgotten changes |

### 🔹 Branching 🌱

| Command | Description |
| --- | --- |
| `git branch` | List all branches |
| `git branch <name>` | Create a new branch |
| `git checkout <branch>` 🔄 | Switch to a branch |
| `git checkout -b <branch>` | Create and switch to new branch |
| `git switch <branch>` | Switch to a branch (new syntax) |
| `git switch -c <branch>` | Create & switch to new branch |

### 🔹 Merging 🔀

| Command | Description |
| --- | --- |
| `git merge <branch>` | Merge branch into current one |
| `git rebase <branch>` | Reapply commits on top of another branch |

### 🔹 Remote 🌍

| Command | Description |
| --- | --- |
| `git remote -v` | Show remote repositories |
| `git remote add origin <url>` | Add remote repo |
| `git push origin <branch>` 🚀 | Push branch to remote |
| `git push -u origin <branch>` | Push branch & set upstream |
| `git pull` ⬇️ | Fetch & merge from remote |
| `git fetch` | Download changes without merging |

### 🔹 Undo / Reset 🔄

| Command | Description |
| --- | --- |
| `git reset <file>` | Unstage a staged file |
| `git reset --hard <commit>` ⚠️ | Reset repo to specific commit |
| `git restore <file>` | Restore file from last commit |
| `git revert <commit>` | Create a commit that undoes changes |

### 🔹 Tagging 🏷️

| Command | Description |
| --- | --- |
| `git tag <name>` | Create a tag |
| `git tag` | List tags |
| `git push origin <tag>` | Push tag to remote |

### 🔹 Stash 📦

| Command | Description |
| --- | --- |
| `git stash` | Save changes temporarily |
| `git stash pop` | Reapply stashed changes |
| `git stash list` | Show stashed changes |

### 🔹 Clean Up 🧹

| Command | Description |
| --- | --- |
| `git branch -d <branch>` | Delete branch (safe) |
| `git branch -D <branch>` ❌ | Force delete branch |

---

✨ With Git + GitHub, collaboration becomes smooth, trackable, and efficient 🚀
