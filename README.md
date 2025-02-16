### Lesson Plan: Collaborating on GitHub Repositories

**Objective:**  
By the end of this lesson, students will be able to:  
1. Create and collaborate on a shared GitHub repository.  
2. Follow a simple Git workflow for group projects.  
3. Understand roles and responsibilities within the team.  

---

### 1. **Setting Up the Collaborative Repository**
1. **Choose a Repository Manager**:  
   - One person (the "Manager") creates the repository on GitHub.  
   - The Manager shares the repository link with the team.  

2. **Clone the Repository**:  
   - Everyone on the team clones the repository to their local computer using:
     ```bash
     git clone <repository-url>
     ```

3. **Branching Rules**:  
   - Everyone creates their own branch to work on.  
   - Name the branch as `name-feature`, for example, `nabila-index` or `ali-update-form`.  
   - Use this command to create and switch to your branch:  
     ```bash
     git checkout -b name-feature
     ```

---

### 2. **Git Workflow for Beginners**
1. **Always Work on Your Branch**:  
   - Never make changes directly to the `main` branch.  

2. **Keep Your Branch Updated**:  
   - Regularly pull updates from the `main` branch to keep your branch up-to-date:  
     ```bash
     git pull origin main
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
