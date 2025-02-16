# **Git Workflow for Beginners**

1. **Keep Your Branch Updated**:  
   - Pull updates from the `main` branch:  
     ```bash
     git checkout main
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
           <summary><strong>❗️ What If There Are Conflicts? </strong></summary>
           <ol>
          <li>Look for ❗️ symbol in your file tree.</li>
          <li>
            Open the files with ❗️. You'll see something like this:
            <pre><code>
            <<<<<<< HEAD
            Your changes here
            =======
            Changes from main branch
            >>>>>> main
            </code></pre>
          </li>
          <li>If you want to keep the changes from the main branch, click <strong>"Accept Incoming Change."</strong></li>
          <li>
            After resolving conflicts:
            <pre><code>
            git add .
            git commit -m "Resolve merge conflicts with main"
            </code></pre>
          </li>
        </ol>
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

