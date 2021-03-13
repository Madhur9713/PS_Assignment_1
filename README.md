# Week 1|Batch 5 |NIT Bhopal| Madhur Gupta

## Git commands

### i) Setup a Local Repository:
    - cd /path/to/folder
    - git init
    // Create any file name File.txt
    - git status
    - git add .
    - echo "First_Assignment" >> README.md
    - git add .
    - git commit -m "First ever import to Github from local through main branch”

### ii) Setup a remote Repository:
    - git branch -M main
    - git remote add origin https://github.com/Madhur9713/PS_Assignment_1.git
    - git push -u origin main

### iii) Create local Branch (feature_branch, qa_branch, dev_branch, delivery_branch):
    - git branch feature_branch
    - git branch qa_branch
    - git branch dev_branch
    - git branch delivery_branch

### iv) Create remote branches:
    - git push origin –all

### v) Add files, Make changes to existing files , Add folders, Remove folders, remove files :
    - echo "Adding new file">>File.txt
    - echo "Adding another file">>File2.txt
    - git add .
    - git commit -m "Adding files for operation like add, delete"
    - git push -u origin main
    - git rm -f File2.txt
    - mkdir Folder_new1
    - git add .
    - git commit -m "Created Folder and removed File2.txt"
    - git push -u origin main
    - cd Folder_new1
    - echo "inside Folder_new1">>file_1_v1.txt
    - git add .
    - git commit -m "New Folder with new file"
    - git push -u origin main

### vi) Check-in, Stage, Commit, Push files into feature_branch:
    - git checkout feature_branch
    - echo "Code in Feature Branch">>feature.txt
    - git add .
    - git commit -m "File is commited to feature branch"
    - git push origin feature_branch

### vii) Promote code from feature branch to dev branch pull via pull requests:
    - git checkout dev_branch
    - git pull origin feature_branch
    - git add .
    - do changes in feature.txt using any text editor
    - git commit -m "checked feature file by dev"
    - git push origin dev_branch

### viii) Check-out the latest code from remote branch to local branch:
    - git pull origin feature_branch

### ix) Explore the difference between Checkout vs Pull”:
    - Checkout:	 git checkout branch_name
		It helps us to update the code the through specified branch and we can easily see the history and manage the changes else it gives merge conflict.
  
    - Pull:		git pull branch_name
		It downloads the repo to local pc and brings changes from the remote repository.

### x) Get two people to make Change to the same file, check in & handle merge conflicts:
    - Since both the feature_branch and dev_branch tried to changed the code inside feature.txt then but then we finally resolved the merge conflicts.

### xi) Ensure the code is in Sync with the latest changes across all branches:
    - Code was then pulled across all branches using git pull branch_name

### Basic usage using the GUI Client (GitHub Client):
    - In this I have used the GUI of GitHub do all the changes which are done earlier using cmd

### Basic usage using the GUI Client (GitHub Client):
    - In this I have used the GUI of GitHub do all the changes which are done earlier using cmd

### On the ground day to day scenarios
    - Reset/ revert:  $ git revert HEAD

    - Stash:  $ git stash

    - Rebasing: $ git rebase branch_name

    - Git log, status & reflog: $ git reflog







