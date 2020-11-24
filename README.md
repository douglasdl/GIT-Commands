# GIT
Version control software.

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

//
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




<p align="center">Desenvolvido por Douglas Dias Leal</p>
