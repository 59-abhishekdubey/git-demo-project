
# Git Demo Project

This is a simple project created for the ASD practical.

## Objective
To demonstrate version control using Git and GitHub.
Better know abhishek




A. Configure and initialize

git --version
git config --global user.name "59-abhishekdubey"
git config --global user.email "abhishekdubey112jeem@gmail.com"
mkdir git-demo-project
cd git-demo-project
git init
git status
  


Create index.html and README.md in VS Code, then save them.

B. Stage, commit and inspect history

git add .
git status
git commit -m "Initial commit"
git log --oneline
  



C. Modify a file and create another commit

Edit index.html and save the change first.

git status
git diff
git add .
git commit -m "Update project"
git log --oneline
  



D. Create and merge a feature branch

git switch -c feature
  


Edit index.html again and save a new feature.

git add .
git commit -m "Add feature"
git switch master
git merge feature
git log --oneline --graph --all
  



E. Connect and push to GitHub

First create a new, empty GitHub repository and copy its HTTPS URL.

git remote add origin https://github.com/YOUR-USERNAME/git-demo-project.git
git remote -v
git push -u origin master
  



F. Synchronize with GitHub

git pull origin master
git fetch origin
git log --oneline origin/master
git merge origin/master
git status