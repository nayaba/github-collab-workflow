# **Git Workflow for Beginners**

1. **Keep Your Branch Updated**:  
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
        <details>
           <summary><bold>What If There Are Conflicts?</bold></summary>
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
        </details>

     


2. **Do work on your branch.**
3. **Commit Your Changes**:  
     ```bash
     git add .
     git commit -m "Add login form"
     ```

4. **Push Your Branch**:   
     ```bash
     git push origin name-feature
     ```

5. **Open a Pull Request (PR)**:  
   - On GitHub, go to the repository and open a pull request (PR) from your branch into `main`.  

6. **The Manager reviews and merges the PR into `main`.**  

