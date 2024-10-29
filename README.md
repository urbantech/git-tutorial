# git-tutorial
### GitHub Cheat Sheet for Developers
Here's a detailed GitHub tutorial cheat sheet covering the most commonly used Git commands that developers on your team can reference. This guide includes commands for setting up a repository, managing branches, making commits, and collaborating with others.

### **Getting Started**

1. **Set Up Git**
   - Install Git (if not already installed):
     ```bash
     brew install git
     ```
   - Configure your Git identity:
     ```bash
     git config --global user.name "Your Name"
     git config --global user.email "you@example.com"
     ```
   - Check your configuration:
     ```bash
     git config --list
     ```

2. **Create a New Repository**
   - Create a new local repository:
     ```bash
     git init <repository-name>
     ```
   - Clone an existing repository:
     ```bash
     git clone <repository-url>
     ```

---

### **Basic Commands**

3. **Navigating and Managing Repositories**
   - Change directory into your project:
     ```bash
     cd <repository-name>
     ```
   - View the status of your repository:
     ```bash
     git status
     ```

4. **Staging Changes**
   - Stage a specific file:
     ```bash
     git add <file-name>
     ```
   - Stage all changes:
     ```bash
     git add .
     ```

5. **Committing Changes**
   - Commit staged changes with a message:
     ```bash
     git commit -m "Your commit message"
     ```

---

### **Branching and Merging**

6. **Branching**
   - List all branches:
     ```bash
     git branch
     ```
   - Create a new branch:
     ```bash
     git branch <branch-name>
     ```
   - Switch to a different branch:
     ```bash
     git checkout <branch-name>
     ```
   - Create and switch to a new branch:
     ```bash
     git checkout -b <branch-name>
     ```

7. **Merging**
   - Merge another branch into the current branch:
     ```bash
     git merge <branch-name>
     ```
   - Resolve merge conflicts manually, then stage and commit the resolved files:
     ```bash
     git add <resolved-file>
     git commit -m "Resolved merge conflict"
     ```

---

### **Working with Remote Repositories**

8. **Connecting to Remote Repositories**
   - Add a remote repository:
     ```bash
     git remote add origin <repository-url>
     ```
   - List remote repositories:
     ```bash
     git remote -v
     ```

9. **Pushing Changes**
   - Push changes to a remote branch:
     ```bash
     git push origin <branch-name>
     ```
   - Push all branches:
     ```bash
     git push --all
     ```

10. **Pulling Changes**
    - Fetch and merge changes from the remote repository:
      ```bash
      git pull origin <branch-name>
      ```

---

### **Viewing History and Changes**

11. **Viewing Commit History**
    - View the commit history:
      ```bash
      git log
      ```
    - View a one-line summary of the commit history:
      ```bash
      git log --oneline
      ```
    - View changes made in the last commit:
      ```bash
      git show
      ```

12. **Diffing Changes**
    - Show changes not yet staged:
      ```bash
      git diff
      ```
    - Show changes between the working directory and the last commit:
      ```bash
      git diff HEAD
      ```

---

### **Undoing Changes**

13. **Undoing Changes**
    - Unstage a staged file:
      ```bash
      git reset <file-name>
      ```
    - Discard changes in a file (uncommitted changes):
      ```bash
      git checkout -- <file-name>
      ```
    - Revert a commit by creating a new commit:
      ```bash
      git revert <commit-id>
      ```

---

### **Tagging**

14. **Tagging**
    - Create a new tag:
      ```bash
      git tag <tag-name>
      ```
    - Push tags to the remote repository:
      ```bash
      git push origin --tags
      ```

---

### **Best Practices**

- **Commit Often**: Make frequent commits with descriptive messages to track changes effectively.
- **Branch for Features**: Create a new branch for each new feature or bug fix to keep the main branch clean.
- **Pull Before Push**: Always pull the latest changes before pushing to avoid conflicts.
- **Use `.gitignore`**: Create a `.gitignore` file to specify files and directories that should not be tracked by Git (e.g., `node_modules`, `.env`).

---

### **Helpful Resources**
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Git Cheat Sheet PDF](https://education.github.com/git-cheat-sheet-education.pdf)
