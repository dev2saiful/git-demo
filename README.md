🚀 Git & GitHub Command Guide

Reference for managing projects and publishing files on GitHub.

📌 1. Install & Setup
git --version # check if Git is installed

git config --global user.name "Saiful Islam Ronak" // set your name
git config --global user.email "your-email@example.com" // set your email

git config --list // verify configuration

📌 2. Create Local Repository
mkdir project-name // create a project folder
cd project-name // enter project folder
git init // initialize Git tracking

📌 3. Basic Workflow (Most Important)
git status // check file status

git add index.html // stage specific file
git add . // stage all files

git commit -m "Initial commit" // save snapshot with message

git log // view commit history

📌 4. Connect Local Project to GitHub
git remote add origin https://github.com/username/repo-name.git // connect to GitHub repo

git branch -M main // set default branch name
git push -u origin main // upload project to GitHub

After first push, use:

git push // push updates

📌 5. Clone Existing Repository
git clone https://github.com/username/repo-name.git // download project from GitHub
cd repo-name // enter downloaded project

Use this when working from another computer.

📌 6. Portfolio Website Repo (Your Use Case)

Repository name must be:

username.github.io

Example commands:

mkdir ronakdev.github.io // create portfolio project
cd ronakdev.github.io
git init // initialize Git

Add files:

git add . // add portfolio files
git commit -m "Portfolio setup"
git push -u origin main // publish website

Upload certificate:

mkdir certificates // create certificate folder
git add certificates/ml-course.pdf // add PDF certificate
git commit -m "Add ML certificate"
git push

Your certificate link will be:

https://username.github.io/certificates/ml-course.pdf

📌 7. Pull & Update Workflow
git pull origin main // get latest changes from GitHub

git add . // stage changes
git commit -m "Update project" // commit changes
git push // upload updates

Standard workflow:

Pull → Edit → Add → Commit → Push

📌 8. Branching (Feature Development)
git branch feature-widget // create new branch

git checkout feature-widget // switch to branch

git checkout -b feature-widget // create + switch branch

git branch // list branches

Merge branch:

git checkout main // switch to main branch
git merge feature-widget // merge feature into main

📌 9. Undo Mistakes
git reset file.txt // unstage file

git checkout -- file.txt // restore file to last commit

git reset --soft HEAD~1 // undo last commit (keep changes)

📌 10. Ignore Unnecessary Files

Create .gitignore file.

Example for WordPress development:

node_modules/ // ignore node packages
vendor/ // ignore composer packages
wp-config.php // ignore config file
\*.log // ignore log files

📌 11. Remove File from Git
git rm file.txt // remove file from project
git commit -m "Remove file"
git push

📌 12. Tag Versions (Release Management)
git tag v1.0 // create version tag
git push origin v1.0 // upload tag

📌 13. Advanced Remote Management
git remote -v // view connected remote repo

git remote remove origin // remove remote connection

git remote add origin repo-url // reconnect repository

📌 14. Professional Workflow for Your Portfolio

For your real development path:

git clone your-portfolio-repo // download portfolio
git pull origin main // sync latest version
git add new-project/ // add WordPress project showcase
git commit -m "Add Elementor widget project"
git push // publish update

Upload certificates exactly the same way.

📌 15. Quick Cheat Sheet
git init // start repository
git add . // stage all changes
git commit -m "message" // save changes
git push // upload to GitHub
git pull // download updates
git clone repo-url // copy repo locally
git branch // view branches
git checkout -b name // create branch
git merge name // merge branch

📌 16. File & Directory Navigation Commands
pwd // show current directory path

ls // list files and folders
ls -l // list with details (permissions, size, date)
ls -a // show hidden files (like .git)
ls -la // detailed list including hidden files

cd folder-name // go inside a folder
cd .. // go back one directory
cd ../.. // go back two directories
cd ~ // go to home directory
cd / // go to root directory

tree // show folder structure as tree (if installed)

mkdir new-folder // create new folder
touch file.txt // create new empty file

cp file.txt backup.txt // copy file
cp -r folder1 folder2 // copy folder recursively

mv oldname.txt newname.txt // rename file
mv file.txt folder/ // move file to folder

rm file.txt // delete file
rm -r folder-name // delete folder and contents

clear // clear terminal screen

history // show command history
