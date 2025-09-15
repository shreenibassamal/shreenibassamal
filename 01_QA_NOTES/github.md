# **Git Basic Commands Cheat Sheet**

---

## **1\. Setup & Configuration**

```xml
git --version                # Check Git version
git config --global user.name "Your Name"       # Set username
git config --global user.email "your@email.com" # Set email
git config --list            # List all config
```

---

## **2\. Create or Clone Repository**

```xml
git init                     # Initialize new local repo
git clone <url>              # Clone repo from remote
git clone <url> myproject    # Clone into folder "myproject"
```

---

## **3\. Basic Snapshotting**

```xml
git status                   # Show status of changes
git add <file>               # Stage single file
git add .                    # Stage all changes
git reset <file>             # Unstage file
git reset                    # Unstage all files
git diff                     # Show unstaged changes
git diff --staged            # Show staged changes
git commit -m "message"      # Commit staged changes
git commit -am "message"     # Stage & commit tracked files
```

---

## **4\. Branching & Merging**

```xml
git branch                   # List branches
git branch <name>            # Create new branch
git checkout <name>          # Switch branch
git checkout -b <name>       # Create + switch branch
git merge <branch>           # Merge branch into current
git branch -d <name>         # Delete branch
```

---

## **5\. Remote Repositories**

```xml
git remote -v                # Show remotes
git remote add origin <url>  # Add remote repo
git push origin <branch>     # Push branch to remote
git push -u origin <branch>  # Push & set upstream
git fetch origin             # Fetch updates from remote
git pull origin <branch>     # Fetch + merge remote branch
git push                     # Push committed changes
```

---

## **6\. Undoing Changes**

```xml
git checkout -- <file>       # Discard changes in file
git reset --hard             # Reset working directory
git revert <commit>          # Undo commit (safe, new commit)
git reset <commit>           # Reset to commit (keeps changes unstaged)
git reset --hard <commit>    # Reset to commit (discard changes)
```

---

## **7\. Viewing History**

```xml
git log                      # Commit history
git log --oneline            # Condensed history
git log --graph --oneline    # Visual branch history
git show <commit>            # Show details of commit
git blame <file>             # Show who changed each line
```

---

## **8\. Stashing (Temporary Save)**

```xml
git stash                    # Save changes temporarily
git stash list               # List stashes
git stash apply              # Apply latest stash
git stash pop                # Apply + remove latest stash
git stash drop               # Delete latest stash
```

---

## **9\. Tagging**

```xml
git tag                      # List tags
git tag v1.0                 # Create lightweight tag
git tag -a v1.0 -m "msg"     # Create annotated tag
git show v1.0                # Show tag details
git push origin v1.0         # Push tag to remote
```

---

## **10\. Collaboration & Conflicts**

```xml
git fetch origin             # Fetch latest changes
git pull                     # Pull + merge
git push                     # Push changes
# Conflict handling:
# Edit conflicting files
git add <file>               # Mark resolved
git commit                   # Commit resolution
```

---

## **11\. Helpful Shortcuts**

```xml
git status -s                # Short status
git log --since="1 week ago" # Commits in last week
git diff HEAD~1 HEAD         # Difference between last commit & current
```

---

✅ **Key Flow for Practice (Daily Git Workflow):**

1. `git init` or `git clone <url>`
    
2. Modify files
    
3. `git add .`
    
4. `git commit -m "message"`
    
5. `git push origin main`
    
6. `git pull origin main` (before pushing next time)
    

---

Would you like me to create a **step-by-step Git practice exercise** (like a hands-on lab: init repo → add → commit → branch → merge → push → resolve conflict), so you can practice all these commands in order?
