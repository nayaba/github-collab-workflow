# **Git Workflow for Beginners**

1. **Always Work on Your Branch**:  
   - Never make changes directly to the `main` branch.  

2. **Keep Your Branch Updated**:  
   - Pull updates from the `main` branch:  
     ```bash
     git pull origin main
     ```
   - **Steps to Pull and Merge `main` into Your Feature Branch:**
        1. **Make sure you're on your feature branch**:
           ```bash
           git checkout name-feature
           ```
        
        2. **Merge `main` into your feature branch**:
           ```bash
           git merge main
           ```
        
        3. **What If There Are Conflicts?**
        If there are conflicts during the merge:
        1. Look for ❗️ symbol in your file tree.
        2. Open the files with ❗️.  You'll see something like this
        ```bash
        <<<<<<< HEAD
        Your changes here
        =======
        Changes from main branch
        >>>>>>> main
        ```
        3. If you want to keep the changes from the main branch, click `"Accept Incoming Change."`
        4. After resolving conflicts:
           ```bash
           git add .
           git commit -m "Resolve merge conflicts with main"
           ```

3. **Commit Your Changes**:  
   - Use clear and simple commit messages to explain your changes:
     ```bash
     git add .
     git commit -m "Add login form"
     ```

4. **Push Your Branch**:  
   - Push your changes to GitHub:  
     ```bash
     git push origin name-feature
     ```

5. **Open a Pull Request (PR)**:  
   - On GitHub, go to the repository and open a pull request (PR) from your branch into `main`.  
   - Add a short description of what you did in the PR.

6. **Wait for Review and Approval**:  
   - The Manager reviews and merges the PR into `main`.  
   - The Manager ensures there are no conflicts before merging.  

---

### 3. **Best Practices**
1. **Clear Roles**:  
   - The Manager is responsible for merging pull requests and resolving conflicts.  

2. **Small and Focused Changes**:  
   - Work on one feature at a time and avoid doing unrelated work in the same branch.  

3. **Communicate**:  
   - Let the team know what feature you're working on to avoid duplicate work.  

4. **Pull Frequently**:  
   - Always pull the latest changes from the `main` branch before starting new work.  

5. **Resolve Conflicts Locally**:  
   - If there are conflicts, fix them locally before pushing updates.

---

### 4. **Cheat Sheet**
- **Clone Repository**:  
  ```bash
  git clone <repository-url>
  ```

- **Create and Switch to a New Branch**:  
  ```bash
  git checkout -b name-feature
  ```

- **Check Your Current Branch**:  
  ```bash
  git branch
  ```

- **Stage Changes**:  
  ```bash
  git add .
  ```

- **Commit Changes**:  
  ```bash
  git commit -m "Brief description of the changes"
  ```

- **Push Branch to GitHub**:  
  ```bash
  git push origin name-feature
  ```

- **Pull Updates from Main**:  
  ```bash
  git pull origin main
  ```

- **Merge a Pull Request**:  
  - The Manager handles this through the GitHub interface.  

