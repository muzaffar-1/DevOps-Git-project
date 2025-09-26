# DevOps-Git-project
# DevOps Project with Git

## Objective
This project demonstrates **version-controlled DevOps practices** using Git and GitHub.  
It follows best practices including feature branching, pull requests, `.gitignore`, and tagging for releases.

---

## Tools Used
- Git
- GitHub
- Docker

---

## Branching Strategy
- **main** → Production-ready code (stable releases)  
- **dev** → Development / integration branch  
- **feature/* ** → Individual features or tasks  

**Example feature branches:**  
- `feature/setup-docker` → Added Dockerfile  
- `feature/add-gitignore` → Added comprehensive `.gitignore`  

---

## Workflow
1. **Initialize Repo**  
   - `git init`  
   - Added `README.md`  
   - Pushed to GitHub

2. **Feature Development**  
   - Create a feature branch:  
     ```bash
     git checkout -b feature/setup-docker
     ```
   - Make changes, commit, and push:  
     ```bash
     git add .
     git commit -m "Added Dockerfile"
     git push origin feature/setup-docker
     ```
   - Raise Pull Request → Merge into `dev`  

3. **Integration & Testing**  
   - Test all changes in `dev` branch  
   - Once verified, raise Pull Request → Merge `dev` → `main`  

4. **.gitignore**  
   - Added `.gitignore` to ignore system files, logs, Docker, Terraform, Node, Python caches, and IDE files.

5. **Tagging Versions**  
   - Tag releases for stable code:  
     ```bash
     git tag -a v1.0 -m "First stable release"
     git push origin v1.0

6. ## screenshot##
   https://github.com/user-attachments/assets/64fc28f5-01e3-4320-bc68-74222096a5bd

   https://github.com/user-attachments/assets/20c82d0b-8f3c-4e23-ae93-674e02d685cd
  { To view the image please copy and paste the url on browser.}

        



   
