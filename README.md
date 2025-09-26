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



   
