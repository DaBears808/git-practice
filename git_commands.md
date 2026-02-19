# Git Beginner Cheat Sheet

A simple, beginner-friendly guide to the most common Git commands and how to use them.

---

## 📌 What Is Git?

Git is a **version control system**.

It helps you:

- Track changes in your code  
- Save versions of your project  
- Go back to older versions  
- Work with other developers  
- Manage different versions of your project safely  

---

# 1️⃣ First-Time Setup (Only Do This Once)

These commands set up your identity in Git.

```bash
git config --global user.name "Your Name"
Sets your name for commits.

git config --global user.email "you@example.com"
Sets your email for commits.

git config --list
Shows your current Git configuration.

2️⃣ Starting a Project
Create a new Git repository
git init
Creates a new Git repository in your current folder.

Clone an existing repository
git clone <repository-url>
Downloads an existing repository from the internet.

Example:

git clone https://github.com/user/project.git
3️⃣ Basic Workflow (Most Important Section)
This is the core Git workflow you will use every day.

Check project status
git status
Shows:

Changed files

Staged files

Untracked files

Add files to staging
git add <file>
Adds a specific file to staging.

git add .
Adds all changed files to staging.

Commit changes
git commit -m "Your message"
Creates a snapshot of staged files with a message describing what changed.

git commit -am "Message"
Adds and commits tracked files in one step.

4️⃣ Branches (Working Safely)
Branches let you work on new features without breaking your main project.

View branches
git branch
Shows all branches.

Create a new branch
git branch <branch-name>
Creates a new branch.

Switch branches
git checkout <branch-name>
Switches to another branch.

git checkout -b <branch-name>
Creates and switches to a new branch.

Merge branches
git merge <branch-name>
Merges another branch into your current branch.

5️⃣ Pushing & Pulling (Working with GitHub)
These commands are used when working with remote repositories.

Check connected remote repositories
git remote -v
Shows connected remote repositories.

Push changes to remote
git push
Uploads your commits to the remote repository.

git push -u origin main
Pushes your branch and connects it to the remote repository.

Pull latest changes
git pull
Downloads and merges latest changes from the remote repository.

git fetch
Downloads changes but does not merge them.

6️⃣ Viewing History
View commit history
git log
Shows full commit history.

git log --oneline
Shows a shorter version of commit history.

See changes
git diff
Shows what has changed but not yet committed.

git show <commit-id>
Shows details of a specific commit.

7️⃣ Undoing Mistakes
⚠️ Be careful with some of these commands.

Discard changes in a file
git restore <file>
Remove file from staging
git reset <file>
Delete all uncommitted changes (Dangerous)
git reset --hard HEAD
Undo a commit safely
git revert <commit-id>
Creates a new commit that reverses a previous commit.

✅ Step-by-Step: How to Commit Your Code
Here is the full beginner workflow from start to finish:

# 1. Go to your project folder
cd your-project-folder

# 2. Start Git (only first time)
git init
#DONT NEED TO DO THIS

# 3. Check what changed
git status

# 4. Add files to staging
git add .

# 5. Commit your changes
git commit -m "Initial commit"

# 6. (Optional) Connect to GitHub
git remote add origin https://github.com/username/repository.git
# DONT NEED TO DO THIS

# 7. Push to GitHub
git push -u origin main
#ONLY NEED TO DO GIT PUSH
⭐ The 3 Most Important Commands to Remember
If you only remember three commands, remember these:

git status
git add .
git commit -m "message"
If you understand those three, you understand the core of Git.

# 67

