# Docker&Git Workflow for Jenkins CI/CD
This repository has been created for future developments to make more simple and easy escalable projects, which developers could use with a guided way taking the best practices to have Jenkins running on Docker environment (on our case) on a Linux based Host.

## Docker Workflow for Jenkins CI/CD
This is going to be Docker+Jenkins guide to configure as **Code**.
1. Jenkins infrastructure (docker, servers, agents, plugins, ...)
2. Jenkins job configuration (stages, builds, triggers, ...)
3. Jenkins system configuration (credentials, LDAP, ...)

### GUIDE (from structure to deploy)
#### STRUCTURE FOR JENKINS FOLDER
This main folder (jenkins2) could be created on any directory of the Host, but for this example, I am going to use "/opt" which is the directory where third party software is installed on this distribution.
![[Pasted image 20260618131950.png]]
**jenkins2:** the main folder where all the files will be stored
**certs:** kings... is the certification of our DC
**config:** folder where are all the files required for the build of the image will be stored
**casc.yaml** (configuration as code): file to configure the configuration of Jenkins globally
**Dockerfile:** it is like the recipient for a meal, these are the steps to make the image
**plugins.txt:** file to add all the plugins needed for Jenkins
**docker-compose.yml:** in our case, this file is responsible for launching and starting the container


## Git Workflow for diary rutine
### Clone Repository
```bash
git clone https://repositorio.git
```

### Access Repository
```bash
cd repositorio
```

### Initial Configuration
```bash
git config --global user.name "nombre"
git config --global user.email "email"
```

### Daily Workflow
See state
   ```bash
git status
   ```
Add changes
   ```bash
git add testFile.txt  # or use '.' to add all files
   ```
Commit
   ```bash
git commit -m "Commit message"
   ```
Upload changes to GitHub repository (main is the default branch; change if your branch name differs)
   ```bash
git push origin main
   ```
Get remote changes from GitHub repository
   ```bash
git pull origin main
   ```

### Good Practices
Show branches
   ```bash
git branch
   ```
Create and switch to a new branch
   ```bash
git checkout -b example-branch
   ```
Switch to an existing branch (e.g., main)
   ```bash
git checkout main
   ```
Merge changes from a branch (e.g., example-branch into current branch)
   ```bash
git merge example-branch
```






