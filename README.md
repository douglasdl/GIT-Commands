# GIT
Version control software.


<br>
Install Git
<br>
`sudo apt-get install git-core`

<br>
Install Git
<br>
`sudo useradd git`

<br>
Install Git
<br>
`passwd git`

<br>
Interface gráfica padrão
<br>
<code>
    gitk
</code>
<br>

Usar Saídas do GIT Coloridas
<br>
<code>
    git config color.ui true
</code>
<br>

Exibir Log em Apenas uma Linha por Commit
<br>
<code>
    git config format.pretty oneline
</code>
<br>


# Github
Web service that uses GIT to host files and handle in a friendly interface.

## Concepts
Repository: a folder that contens the files of a project.<br>
Readme: document that explains the details of your project.<br>
Master: main code.<br>
Branch: creates a copy from the master as a parallel sub version.<br>
Fork: create a copy from the master to your account to use independently.<br>
Commit: Save the files.<br>
Push: request to send files request to merge your branch code changes to the master code.<br>
Pull Request: request the files updates from Github to synchonize your local folder.<br>
Working Directory: 
Stage (Index):
History:

## Commands

Check a directory settings
<br>
<code>
    git config --list
</code>
<br>

Set or change the user name
<br>
<code>
    git config --global user.name "username"
</code>
<br>

Set or change the user e-mail
<br>
<code>
    git config --global user.email "email"
</code>
<br>

Set or change the user name (only for current repository)
<br>
<code>
    git config user.name "username"
</code>
<br>

Set or change the user e-mail (only for current repository)
<br>
<code>
    git config user.email "email"
</code>
<br>



Check the history of all changes logs (To quit VIM editor press :q)
<br>
<code>
    git log
</code>
<br>

Check the history of the last 2 changes logs
<br>
<code>
    git log -2
</code>
<br>

Check the staus of your project
<br>
<code>
    git status
</code>
<br>

Clone a local directory to your PC
<br>
<code>
    git clone [address]
</code>
<br>

Clone a remote directory to your PC
<br>
<code>
    git clone user@server:[address]
</code>
<br>





## Create a new Repository
Add a folder from your local folder to Github
<br>
<code>
    git init
</code>
<br>


## Copy files from WORK DIRECTORY to STAGE(INDEX)
Add a new file to be sent to Github
<br>
<code>
    git add [file]
</code>
<br>

Add ALL the new files, directories or changes to be sent to Github
<br>
<code>
    git add .
</code>
<br>

Make interactive inclusions
<br>
<code>
    git add -i
</code>
<br>

## Removing Files and Directories to be Commited
Discard the changes in a working directory to be sent to Github
<br>
<code>
    git restore [file]
</code>
<br>
    
Discard the changes in a working directory to be sent to Github
<br>
<code>
    git rm --cached [file]
</code>
<br>

## Removing Untracked Files and Directories from workspace
Dry run to see which files you’ll delete
`git clean -n -d`

Delete all untracked files and direcories
`git clean -f -d`


## Copy files from STAGE(INDEX) to HISTORY
Send the changes or new files and directories to Github, giving a description about these changes
<br>
<code>
    git commit -m "Initial import"
</code>
<br>

Send all the changes or new files and directories to Github, giving a description about these changes
<br>
<code>
    git commit -a -m "Initial import"
</code>
<br>

Edit the commit message  
`git commit --amend`  




## Sending the Files
Send to files to Github to share
<br>
<code>
    git push
</code>
<br>

Check the name of the remote repository from Github
<br>
<code>
    git remote
</code>
<br>

Check the name of the remote repository from Github with verbose
<br>
<code>
    git remote -v
</code>
<br>

Send to files to Github to share
<br>
<code>
    git push origin
</code>
<br>

Send to files to Github to share
<br>
<code>
    git push origin master
</code>
<br>

Create a new branch
<br>
<code>
    git checkout -b new-branch-name
</code>
<br>

## Copy files from WORKING DIRECTORY directly to HISTORY
Equivalent to running git add on all filenames that existed in the latest commit, and then running git commit.
<br>
<code>
    git commit -a
</code>
<br>


## Receiving the Files
Get files from Github to update your local folder
<br>
<code>
    git pull
</code>
<br>

## Change Branch
Show all the banches
<br>
<code>
    git branch
</code>
<br>

Switch from one branch to another
<br>
<code>
    git checkout [branchname]
</code>
<br>

Switch from one branch to another
<br>
<code>
    git switch [branchname]
</code>
<br>

Switch back to previous branch
<br>
<code>
    git switch -
</code>
<br>

Create a new branch and switch to it
<br>
<code>
    git checkout -b [branchname]
</code>
<br>

Create a new branch and switch to it
<br>
<code>
    git switch -c [branchname]
</code>
<br>


# Merge Branches
Merge the currently selected brance to another branch
<br>
<code>
    git merge [branchname]
</code>
<br>


## Ignore files
Create a .gitignore file to track the files that must be ignored
<br>
LINUX
<br>
<code>
    touch .gitignore
</code>
<br>
WINDOWS
<br>
<code>
    notepad .gitignore
</code>
<br>





# CLASP (GIT tool for Google Apps Script)

## Installation
Installation (Need to install Node.js and NPM before)
<br>
<code>
    npm install @google/clasp -g
</code>
<br>

## Login
Log in to script.google.com to authorize managment of your account
<br>
<code>
    clasp login
</code>
<br>

## Logout
Log out from your Google account
<br>
<code>
    clasp logout
</code>
<br>

## Create
Create a new Google Apps Script project. First you need to authorize the API at https://script.google.com/home/usersettings 
<br>
<code>
    clasp create [scriptTitle]
</code>
<br>

## Clone
Clone an existing project
<br>
<code>
    clasp clone <scriptId>
</code>
<br>
 
## Pull
Download a script project
<br>
<code>
    clasp pull
</code>
<br> 

## Push
Update the remote project (upload all files)
<br>
<code>
    clasp push
</code>
<br>

Update the remote project every time you save a modified file (upload all files)
<br>
<code>
    clasp push -w
</code>
<br>

## Versions
List versions of a script
<br>
<code>
    clasp versions
</code>
<br>

## Deploy
First create an immutable version of the Apps Script project.
<br>
<code>
    clasp version [description]
</code>
<br>

Deploy a project.<br>
Undeploy a deployment of a project
<br>
<code>
    clasp deploy [version] [description]
</code>
<br>
<code>
    clasp undeploy <deploymentId>
</code>
<br>
 
Update an existing deployment with a new version and description
<br>
<code>
    clasp redeploy <deploymentId> <version> <description>
</code>
<br> 

List deployments
<br>
<code>
    clasp deployments
</code>
<br> 

Open the project in the Apps Script editor
<br>
<code>
    clasp open
</code>
<br> 
 
## Other commands
Lists files that will be pushed by clasp
<br>
<code>
    status [options]
</code>
<br> 

List App Scripts projects
<br>
<code>
    list
</code>
<br>

Shows the StackDriver logs
<br>
<code>
    logs [options]
</code>
<br>

Run a function in your Apps Scripts project
<br>
<code>
    run [options] [functionName]
</code>
<br>

List, enable, or disable APIs
<br>
<code>
    apis [options]                              
</code>
<br>
<code>
    list
</code>
<br>
<code>
    enable <api>
</code>
<br>
<code>    
    disable <api>
</code>
<br>

Display help
<br>
<code>
    help
</code>
<br>

<p align="center">Desenvolvido por Douglas Dias Leal</p>
