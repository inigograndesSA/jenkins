# GITHUB+JENKINS
### GITHUB
1. Clone repository
	git clone https://repositorio.git
2. Access to repositoy
	cd repositorio
3. Initial configuration
	git config --global user.name "nombre"
	git config --global user.email "email"
4. Dailyl work flow
	4.1. See state
		git status
	4.2. Add changes
		git add testFile.txt (. everything)
	4.3. Commit
		git commit -m "Commit message" 
	4.4. Upload changes to github repository
		git push origin main (main is my principal branch, it has to be changed if your branch name is other)
	4.5. Get remote changes from github repository
		git pull origin main
5. Good practices
	5.1. Show branches
		git branch
	5.2. Create and change branch
		git checkout -b example-branch
	5.3. Change branch
		git checkout main
	5.4. Merge changes
		git merge example-branch




