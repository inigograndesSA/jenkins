# Git Workflow and Best Practices

## Clone Repository
```bash
git clone https://repositorio.git
```

## Access Repository
```bash
cd repositorio
```

## Initial Configuration
```bash
git config --global user.name "nombre"
git config --global user.email "email"
```

## Daily Workflow
1. See state
   ```bash
git status
   ```
2. Add changes
   ```bash
git add testFile.txt  # or use '.' to add all files
   ```
3. Commit
   ```bash
git commit -m "Commit message"
   ```
4. Upload changes to GitHub repository (main is the default branch; change if your branch name differs)
   ```bash
git push origin main
   ```
5. Get remote changes from GitHub repository
   ```bash
git pull origin main
   ```

## Good Practices
1. Show branches
   ```bash
git branch
   ```
2. Create and switch to a new branch
   ```bash
git checkout -b example-branch
   ```
3. Switch to an existing branch (e.g., main)
   ```bash
git checkout main
   ```
4. Merge changes from a branch (e.g., example-branch into current branch)
   ```bash
git merge example-branch
```
