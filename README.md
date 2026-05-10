# Git & GitHub Assessment

## NAME: SHIWANSHU KUMAR JHA
## MOBILE_NUMBER : 7979756698
## EMAIL_ID : shiwanshukumarjha7@gmail.com
## GIT_REPO : https://github.com/shiwanshu97/GIT_Assessment.git

---

# Question 1: Project Initialisation & First Push

## Objective
Set up a new Git project and push it to a remote repository.

## Tasks

### 1. Create a new folder for your project
Created a new project folder named **Git_Assessment** to store all project files.

```bash
mkdir Git_Assessment
cd Git_Assessment
```

---

### 2. Initialise a Git repository
Initialised Git inside the project folder so Git can start tracking project changes.

```bash
git init
```

---

### 3. Create a file named app.py and add some Python code
Created the main Python file for the project and added basic Python code.

```bash
touch app.py
```

---

### 4. Check the current Git status
Checked the repository status to see untracked, modified, or staged files.

```bash
git status
```

---

### 5. Stage the file
Added `app.py` to the staging area so it can be included in the next commit.

```bash
git add app.py
```

---

### 6. Commit with a meaningful message
Created the first commit to save the current project state with a clear message.

```bash
git commit -m "Initial commit with app.py"
```

---

### 7. Create a remote repository (GitHub or similar)
Created a remote repository on GitHub to store and manage the project online.

```text
Repository Name : GIT_Assessment
```

---

### 8. Add the remote (origin) to your local repo
Connected the local repository with the GitHub repository using the remote URL.

```bash
git remote add origin https://github.com/shiwanshu97/GIT_Assessment.git
```

---

### 9. Verify the remote configuration
Verified that the remote repository was added successfully.

```bash
git remote -v
```

---

### 10. Push your code to the remote repository
Uploaded the local project files and commit history to GitHub.

```bash
git push -u origin main
```

OR

```bash
git push -u origin master
```

---

# Question 2: Working with Changes & History

## Objective
Track code changes and manage commit history properly.

## Tasks

### 1. Modify app.py by adding new functionality
Updated the existing Python file by adding new functionality or logic.

---

### 2. Check what changes are made before staging
Checked which files were modified before adding them to staging.

```bash
git status
```

---

### 3. View differences in the file
View the line-by-line changes made inside the file before committing.

```bash
git diff
```

---

### 4. Stage only specific changes (if possible)
Used patch mode to stage selected changes instead of the entire file.

```bash
git add -p
```

OR

```bash
git add app.py
```

---

### 5. Commit with a clear message
Saved the new changes with a meaningful commit message.

```bash
git commit -m "Added new functionality"
```

---

### 6. Make another change in app.py
Modified the file again to continue development and improvements.

---

### 7. Stage all changes
Added all modified files to the staging area at once.

```bash
git add .
```

---

### 8. Commit again
Created another commit to save the latest project updates.

```bash
git commit -m "Updated app.py with additional changes"
```

---

### 9. View full commit history
Displayed the complete commit history with detailed information.

```bash
git log
```

---

### 10. View compact (one-line) history
Displayed commit history in a short one-line format.

```bash
git log --oneline
```

---

# Question 3: Branching & Feature Development

## Objective
Work with branches and manage feature development.

## Tasks

### 1. Create a new branch (e.g., feature-update)
Created a separate branch to work on new features safely.

```bash
git branch feature-update
```

---

### 2. Switch to the new branch
Moved from the main branch to the feature branch for development.

```bash
git checkout feature-update
```

OR

```bash
git switch feature-update
```

---

### 3. Modify app.py with new feature logic
Added new feature-related updates inside the Python file.

---

### 4. Stage and commit the changes
Saved the feature branch changes using staging and commit commands.

```bash
git add app.py
git commit -m "Added new feature update"
```

---

### 5. Switch back to the main branch
Returned to the main branch after completing feature development.

```bash
git checkout main
```

OR

```bash
git switch main
```

---

### 6. Merge the feature branch into main
Merged all feature branch updates into the main branch.

```bash
git merge feature-update
```

---

### 7. Verify changes are merged
Checked commit history to confirm the merge was successful.

```bash
git log --oneline
```

---

### 8. Delete the branch safely
Deleted the feature branch after merging it successfully.

```bash
git branch -d feature-update
```

---

### 9. Try force deleting a branch (create a dummy branch for this)
Created a dummy branch and force deleted it using the `-D` option.

Create dummy branch:

```bash
git branch dummy-branch
```

Force delete dummy branch:

```bash
git branch -D dummy-branch
```

---

# Question 4: Handling Errors (Stash, Reset, Revert)

## Objective
Learn how to manage mistakes and unfinished work.

## Tasks

### 1. Make changes to app.py, but do NOT commit
Modified the file temporarily without creating a commit.

---

### 2. Stash the changes (include untracked files)
Temporarily saved all changes, including untracked files, using stash.

```bash
git stash -u
```

---

### 3. Check the stash list
Viewed all saved stashes available in the repository.

```bash
git stash list
```

---

### 4. Apply the stashed changes back
Restored the stashed changes back into the working directory.

```bash
git stash apply
```

---

### 5. Commit the changes
Committed the restored changes after reviewing them.

```bash
git add .
git commit -m "Committed stashed changes"
```

---

### 6. Make another commit with incorrect code
Created a commit intentionally containing incorrect changes for practice.

```bash
git add .
git commit -m "Added incorrect code"
```

---

### 7. Undo the last commit using reset
Used reset to remove the latest commit from the commit history.

Soft reset:

```bash
git reset --soft HEAD~1
```

OR Hard reset:

```bash
git reset --hard HEAD~1
```

---

### 8. Make another commit
Created a new commit after fixing previous mistakes.

```bash
git add .
git commit -m "Fixed previous mistakes"
```

---

### 9. Undo a commit using revert (create a new reversing commit)
Used revert to safely undo changes by creating a reverse commit.

```bash
git revert HEAD
```

---

### 10. Verify the commit history
Checked the final commit history after reset and revert operations.

```bash
git log
```

OR

```bash
git log --oneline
```

---

# Conclusion

Successfully completed all Git & GitHub assessment tasks, including:

- Repository initialisation
- Working with commits and history
- Branching and merging
- Stashing changes
- Resetting commits
- Reverting commits
- Pushing code to the GitHub repository
