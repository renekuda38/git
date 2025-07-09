## Creating git repo locally and pushing it to GitHub
``` bash
mkdir testDir; cd testDir
touch queries.sql
git init
git add queries.sql
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/renekuda38/<repository-name>.git
git push -u origin main # main or master - check it with "git branch"
# use above command if it's first push after creation of repository
# or after switching the branch
# if it's not first time or after branch switching -> git push
```
### Github Login Prompt after `git push`
``` bash
Username for 'https://github.com': renekuda38
Password for 'https://renekuda38@github.com': <generate a token from https://github.com/settings/tokens>
```
## Having repository on GitHub and want to pull it locally
### 1. Clone GitHub repository locally (to folder of your sake on your machine)
``` bash 
git clone https://github.com/user/<repository-name>.git
```
![Screenshot 2025-07-05 at 08 24 44](https://github.com/user-attachments/assets/c25c41ed-83e8-465e-99e3-247268c14200)
### 2.1 After changes made locally, you want to commit it back to GitHub
``` bash
git add .
git commit -m "new commit"
git push # can be prompted to input GitHub credentials
```
### 2.2 After changes made on Github, pull the updated files locally
``` bash
git pull origin master # or main
```
