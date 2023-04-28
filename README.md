# Git Command And Error Fixing :
In this repository,I  have solve some common problem on git and GitHub. New users face this types of problem , when they use this version control system tecchnology.
## Git Command :
## LINKS : 
- [For checking your Current status ](#for-checking-your-current-status)
- [Checking process is git is install in your pc or not](#checking-process-is-git-is-install-in-your-pc-or-not)
- [For checking your Current status](#for-checking-your-current-status)
- [For cloning remote repository to your local folder](#for-cloning-remote-repository-to-your-local-folder)
- [For adding new branch](#for-adding-new-branch)
- [For initializing git folder](#for-initializing-git-folder)
- [For Adding File](#for-adding-file)
- [For adding Folder ](#for-adding-folder)
- [For adding all files and Folder](#for-adding-all-files-and-folder)
- [For Commiting ](#For-commiting )
- [For adding remote origin ](#for-adding-remote-origin )
- [Push local to remote](#push-local-to-remote)
- [Swtching one branch to another branch](#swtching-one-branch-to-another-branch)
- [Showing how many number of branch in your local repository](#showing-how-many-number-of-branch-in-your-local-repository)
- [Deleting a branch locally ](#deleting-a-branch-locally )
- [ Deleting a branch remotely ](#deleting-a-branch-remotely )
- [ For viewing commit ](#for-viewing-commit)
- [For swtching your current branch ](#for-swtching-your-current-branch)
- [Error 1 way 1](#error-1-way-1)
- [Error 1 way 2](#error-1-way-2)
- [ Error 2 checkout swtching doesnt work ](#error-2-checkout-swtching-doesnt-work)
- [Error 3 pushing shows some error ](#error-3-pushing-shows-some-error)
- [Error 4 origin does not appear to be a git repository](#error-4-origin-does-not-appear-to-be-a-git-repository)

## !!First you haveto download git in your PC!!
### Checking process is git is install in your pc or not

```sh
Command : git --version
#If the terminal shows this types of result such as (git version 2.34.1) that means git is installed in your PC .
```

### For checking your Current status 

```sh
Command : git status
```

### For cloning remote repository to your local folder 
```sh
Command : git clone URL
Command : git clone https://github.com/RlM100always/Git_Error_Fix.git
```

### For initializing git folder 
```sh
Command : git init
```

### For Adding File 
```sh
#If File name = Test.txt
git add File name
Command : git add Test.txt
```

### For adding Folder 
```sh
#If Folder name = DSA
Command : git add DSA/
```

### For adding all files and Folder 
```sh
Command : git add . 
```

### For Commiting 
```sh
Command : git commit -m "Anything as your wish"

```

### For adding new branch 
```sh
git branch <branch name>
#If branchname = master
Command : git branch master
```

### For adding remote origin 
```sh
Command : git remote add origin https://github.com/RlM100always/Test1.git
```
Note : If you face (//fatal: remote origin already exists) this types of problem when you add origin , you have to be Fixed this Error

### Error 1 way 1
#### Error name : //fatal: remote origin already exists 
#### Lets fix it :
```sh
Command : git remote remove origin
Command : git remote -v
Command : git remote add origin [url].git
#Now fix this issue .
```

### Error 1 way 2
#### //fatal: remote origin already exists 
```sh
Command : git remote rename origin dev
Command : git remote -v
#It is the another way to fix this same problem .
```

###  Push local to remote
```sh
Command : git push -u origin <branch name>
#If branchname = master
Command : git push -u origin master
```

### Swtching one branch to another branch 
```sh
Command : git checkout <branch name>
```
if branch name = (main) and you want to go on branch (master).
You have to check it first which is your current branch.
```sh
Command : git branch
```
(It shows your current branch name) <br>
if branch name = (main) and you want to go on branch (master).
```sh
Command : git checkout master
```
Now your branch will be chanced from main to master.

### For creating Branch 
```sh
Command : git branch <branch name>
```

### Showing how many number of branch in your local repository 
```sh
Command : git branch
```

### Deleting a branch locally 
```sh
Command : git branch -d <branch>
```

### Deleting a branch remotely
```sh
Command : git push <remote> --delete <branch>
Command : git push origin --delete fix/authentication
```

### You can also use this shorter command to delete a branch remotely 
```sh
Command : git push <remote> :<branch>
```

###  **Try to synchronize your branch list using:
The -p flag means "prune". After fetching, branches which no longer exist on the remote will be deleted.
```sh
Command : git fetch -p
```

### Error 2 checkout swtching doesnt work 
#### Stash Changes :
Use git stash to store your changes until you are ready to commit. Git stash will conserve your changes, but not associate them with any commit or branch until you are ready.
```sh
Command : git stash push  
Command : git checkout <previous-branch>
Command : git stash pop 
```
### For viewing commit 
```sh
Command : git log
Command : git log --oneline
```
### Error 3 pushing shows some error

! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/RlM100always/Git_Error_Fix.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
#### Lets fix it : 
```sh
Command : command : git push -f origin branchname
```
### Error 4 origin does not appear to be a git repository

fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

```sh
Command : git remote -v
# If there is no remote repo called origin
# Lets try following code
Command : git remote add origin <remote_URL>
Command : git push -f origin <branch name>
```

### For swtching your current branch 
```sh
Command : git switch -c newbranchname
```









