# Collaborating on GitHub Repositories

### Set Up the Local Repos
1. Clone your [Auth Frontend](https://github.com/nayaba/react-jwt-auth-template-seb-2-pt) and [Auth Backend](https://github.com/zeemohamed7/seb-pt-2-express-api-jwt-auth) Templates
2. Remove git tracking and initialize a new git repo
   ```bash
   rm -rf .git
   git init
   git add .
   git commit -m "Initial Commit"
   ```
3. Link your local repo to the github.com repo you just created
   ```bash
   git remote add origin <github-repo-link>
   git push origin main
   ```

### Set Up the Collab Repos
1. **Choose a Repo Manager**:  
   - One person (Manager) creates the repository on GitHub.  
   - The Manager shares the repository link with the team.  

### Follow the Picture Below to Add Your Group Members to the Repo
<img width="1508" alt="repo-settings" src="https://github.com/user-attachments/assets/929dc6df-5b74-408f-9a92-4192bc0721d7" />
<img width="1506" alt="repo-settings-2-collaborators" src="https://github.com/user-attachments/assets/31ad2d91-df09-452e-bac7-f6c219e611a0" />
<img width="1503" alt="repo-3-collaborators" src="https://github.com/user-attachments/assets/69489fb2-fa02-4884-87a2-9dcd42c40d53" />
<img width="1505" alt="repo-04-collaborators-search-results" src="https://github.com/user-attachments/assets/d099080c-ef52-4c1f-9257-10e57aca87a7" />
<img width="1984" alt="repo-05-view-invite" src="https://github.com/user-attachments/assets/ce7964ca-2f81-4b81-8143-48c70d4333d3" />
<img width="1467" alt="repo-6-collaboration-invite-github" src="https://github.com/user-attachments/assets/c5c69460-d0e0-4f40-a894-35261e0daf87" />


2. **Clone the Repo & Finish Setup**:  
   - Everyone clones the repo to their computer using:
     ```bash
     git clone <repo-url>
     ```
   - Run install command and create `.env` file:
     ```bash
     npm i
     touch .env
     ```
   - Add info to the right .env file:
     Backend:
     ```bash
      MONGODB_URI=mongodb+srv://<username>:<password>@sei-w0kys.azure.mongodb.net/hoot?retryWrites=true
      JWT_SECRET=your_secure_random_string_here
     ```
     Frontend:
     ```bash
      VITE_BACK_END_SERVER_URL=http://localhost:3000
     ```

3. **Branching Rules**:  
   - Everyone creates their own branch to work on.  
   - Name the branch `name-feature`, for example, `nabila-index` or `ali-update-form`.  
   - Use this command to create your branch:  
     ```bash
     git checkout -b name-feature
     ```


🖥️ [Workflow for Coding](workflow.md)

