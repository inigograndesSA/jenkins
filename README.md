# Docker&Git Workflow and Best Practices
I have created this repository for future developments to make more simple and easy escalable projects, which developers could use with a guided way taking the best practices to have a Docker environment running Jenkins (on our case) on a Linux based Host.

## Docker Workflow and Best Practices

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






