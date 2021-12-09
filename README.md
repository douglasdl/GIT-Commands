# GIT
Version control software.

# Github
Web service that uses GIT to host files and handle in a friendly interface.

## Concepts  
Repo: same as Repository.
Repository: a folder that contens the files of a project.  
Readme: document that explains the details of your project.  
Master: main code.  
Branch: creates a copy from the master as a parallel sub version.  
Fork: create a copy from the master to your account to use independently.  
Commit: Save the files.<br>
Push: request to send files request to merge your branch code changes to the master code.  
Pull Request: request the files updates from Github to synchonize your local folder.  
Working Directory:  the files that you are currently working on.  
Working Tree: same as Working Directory.  
Index: same as Staging Area.
Staging Area: intermediary area where commits are prepared.  
History: the versions from your project that can be restored.    
Tracked Files: files included in your project to be monitored.  
Untracked Files: files not included in your project to be monitored.  
Ignored Files: files included in your .gitignore file to be ignored from your project and to not be monitored.  
Tree States (Tracked Files) : Modified, Staged, Committed.  

## Commands

Check a directory settings
```sh
    git config --list
```

Set or change the user name
```sh
    git config --global user.name "username"
```

Set or change the user e-mail
```sh
    git config --global user.email "email"
```

Set or change the user name (only for current repository)
```sh
    git config user.name "username"
```

Set or change the user e-mail (only for current repository)
```sh
    git config user.email "email"
```


Check the history of all changes logs (To quit VIM editor press :q)
```sh
    git log
```

Check the history of the last 2 changes logs
```sh
    git log -2
```

Check the staus of your project
```sh
    git status
```

Clone a local directory to your PC
```sh
    git clone [address]
```

Clone a remote directory to your PC
```sh
    git clone user@server:[address]
```


## Create a new Repository
Add a folder from your local folder to Github
```sh
    git init
```

## Create a new Repository (on Server)
Create a new Git Project on Server  
```sh
    git init --bare my-project.git  
```

## Add an existing local repository to an empty repository (on Server)
```sh
git init
git add .
git commit -m "First commit"
git remote add origin user@server:[address]
git push -u origin master
```

## Copy files from WORK DIRECTORY to STAGE(INDEX)
Add a new file to be sent to Github
```sh
    git add [file]
```

Add ALL the new files, directories or changes to be sent to Github
```sh
    git add .
```

Make interactive inclusions
```sh
    git add -i
```

## Removing Files and Directories to be Commited
Discard the changes in a working directory to be sent to Github
```sh
    git restore [file]
```
    
Discard the changes in a working directory to be sent to Github
```sh
    git rm --cached [file]
```

## Removing Untracked Files and Directories from workspace
Dry run to see which files you’ll delete
```sh
    git clean -n -d
```

Delete all untracked files and direcories
```sh
    git clean -f -d
```
  
Cancel changes from working area file
```sh
    git checkout -- <file>
```

## Copy files from STAGE(INDEX) to HISTORY
Send the changes or new files and directories to Github, giving a description about these changes
```sh
    git commit -m "Initial import"
```

Send all the changes or new files and directories to Github, giving a description about these changes
```sh
    git commit -a -m "Initial import"
```

Edit the commit message  
```sh
    git commit --amend
```  

## Sending the Files
Send to files to Github to share
```sh
    git push
```

Check the name of the remote repository from Github
```sh
    git remote
```

Check the name of the remote repository from Github with verbose
```sh
    git remote -v
```

Send to files to Github to share
```sh
    git push origin
```

Send to files to Github to share
```sh
    git push origin master
```

Create a new branch
```sh
    git checkout -b new-branch-name
```

## Copy files from WORKING DIRECTORY directly to HISTORY
Equivalent to running git add on all filenames that existed in the latest commit, and then running git commit.
```sh
    git commit -a
```

## Receiving the Files
Get files from Github to update your local folder
```sh
    git pull
```

## Change Branch
Show all the banches
```sh
    git branch
```

Switch from one branch to another
```sh
    git checkout [branchname]
```

Switch from one branch to another
```sh
    git switch [branchname]
```

Switch back to previous branch
```sh
    git switch -
```

Create a new branch and switch to it
```sh
    git checkout -b [branchname]
```

Create a new branch and switch to it
```sh
    git switch -c [branchname]
```


# Merge Branches
Merge the currently selected brance to another branch
```sh
    git merge [branchname]
```
  
# Delete a Branch  
Delete branch locally  
```sh
    git branch -d [localBranchName]
```

Delete branch remotely  
```sh
    git push origin --delete [remoteBranchName]
```

## Ignore files
Create a .gitignore file (LINUX)
```sh
    touch .gitignore
```
Create a .gitignore file (WINDOWS)
```sh
    notepad .gitignore
```
[gitignore generator](https://www.toptal.com/developers/gitignore)


# CLASP (GIT tool for Google Apps Script)

## Installation
Installation (Need to install Node.js and NPM before)
```sh
    npm install @google/clasp -g
```

## Login
Log in to script.google.com to authorize managment of your account
```sh
    clasp login
```

## Logout
Log out from your Google account
```sh
    clasp logout
```

## Create
Create a new Google Apps Script project. First you need to authorize the API at https://script.google.com/home/usersettings 
```sh
    clasp create [scriptTitle]
```

## Clone
Clone an existing project
```sh
    clasp clone <scriptId>
```
 
## Pull
Download a script project
```sh
    clasp pull
``` 

## Push
Update the remote project (upload all files)
```sh
    clasp push
```

Update the remote project every time you save a modified file (upload all files)
```sh
    clasp push -w
```

## Versions
List versions of a script
```sh
    clasp versions
```

## Deploy
First create an immutable version of the Apps Script project.
```sh
    clasp version [description]
```

Deploy a project.<br>
Undeploy a deployment of a project
```sh
    clasp deploy [version] [description]
```
  
```sh
    clasp undeploy <deploymentId>
```
 
Update an existing deployment with a new version and description
```sh
    clasp redeploy <deploymentId> <version> <description>
``` 

List deployments
```sh
    clasp deployments
``` 

Open the project in the Apps Script editor
```sh
    clasp open
``` 
 
## Other commands
Lists files that will be pushed by clasp
```sh
    status [options]
``` 

List App Scripts projects
```sh
    list
```

Shows the StackDriver logs
```sh
    logs [options]
```

Run a function in your Apps Scripts project
```sh
    run [options] [functionName]
```

List, enable, or disable APIs
```sh
    apis [options]                              
```
```sh
    list
```
```sh
    enable <api>
```
```sh    
    disable <api>
```

Display help  
```sh
    help
```

<p align="center">Desenvolvido por Douglas Dias Leal</p>
