# git-tutorial
### GitHub Cheat Sheet for Developers

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

2. **Clone the Repository**
   - Clone the practice repository:
     ```bash
     git clone git@github.com:urbantech/git-tutorial.git
     ```
   - Change directory into the cloned repository:
     ```bash
     cd git-tutorial
     ```

---

### **Basic Commands**

3. **Check Repository Status**
   - View the status of your repository:
     ```bash
     git status
     ```

4. **Create Your First Git Commit**
   - Create a new file (e.g., `README.md`):
     ```bash
     touch README.md
     ```
   - Open `README.md` in your text editor and add some content (e.g., `# Git Tutorial`).
   - Stage the new file:
     ```bash
     git add README.md
     ```
   - Commit the staged changes with a message:
     ```bash
     git commit -m "Add README.md for Git tutorial"
     ```

---

### **Branching and Merging**

5. **Branching**
   - List all branches:
     ```bash
     git branch
     ```
   - Create a new branch for your feature (e.g., `feature/first-commit`):
     ```bash
     git branch feature/first-commit
     ```
   - Switch to the new branch:
     ```bash
     git checkout feature/first-commit
     ```

6. **Merging**
   - Switch back to the main branch:
     ```bash
     git checkout main
     ```
   - Merge the feature branch into the main branch:
     ```bash
     git merge feature/first-commit
     ```

---

### **Working with Remote Repositories**

7. **Push Changes**
   - Push your changes to the remote repository:
     ```bash
     git push origin main
     ```

8. **Pull Changes**
   - Fetch and merge changes from the remote repository:
     ```bash
     git pull origin main
     ```

---

### **Viewing History and Changes**

9. **Viewing Commit History**
   - View the commit history:
     ```bash
     git log
     ```

10. **Diffing Changes**
    - Show changes not yet staged:
      ```bash
      git diff
      ```

---

### **Undoing Changes**

11. **Undoing Changes**
    - Unstage a staged file:
      ```bash
      git reset README.md
      ```
    - Discard changes in a file (uncommitted changes):
      ```bash
      git checkout -- README.md
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

This cheat sheet provides a structured way for students to practice Git commands using the provided repository.
