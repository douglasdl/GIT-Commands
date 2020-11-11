# GIT
Version control software.

# Github
Web service that uses GIT to host files and handle in a friendly interface.

## Concepts
Repository: a folder that contens the files of a project.<br>
Readme: document that explains the details of your project.<br>
Master: main code.<br>
Branch: creates a copy from the master as a parallel sub version.<br>
Fork: create a copy from the master to your account to use independently.<br>
Commit: Save the files.<br>
Push: <br>
Pull Request: request to send files request to merge your branch code changes to the master code.<br>

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
    git config --global user.name "Douglas Dias Leal"
</code>
<br>

Set or change the user e-mail
<br>
<code>
    git config --global user.email "douglas_san@hotmail.com"
</code>
<br>

//
<br>
<code>
    git log
</code>
<br>

//
<br>
<code>
    git status
</code>
<br>

Clone a directory to your PC
<br>
<code>
    git clone <address>
</code>
<br>

## Adding Files and Directories to be Commited
Add a new file to be sent to Github
<br>
<code>
    git add <file>
</code>
<br>

Add ALL the new files, directories or changes to be sent to Github
<br>
<code>
    git add .
</code>
<br>

## Removing Files and Directories to be Commited
Discard the changes in a working directory to be sent to Github
<br>
<code>
    git restore <file>
</code>
<br>

## Commiting the Files
Send the changes or new files and directories to Github, giving a description about these changes
<br>
<code>
    git commit -m "Initial import"
</code>
<br>

## Sending the Files
Send to files to Github to share
<br>
<code>
    git push
</code>
<br>

Create e new branch
<br>
<code>
    git checkout -b new-branch-name
</code>
<br>


<p align="center">Desenvolvido por Douglas Dias Leal</p>
