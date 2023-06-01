# Git Commands


Create a new repository on the command line
-------------------------
* git init  
* git add .  
* git commit -m "first commit"   
* git branch -M main  
* git remote add origin https://github.com/имяПользователя/проект.git   
* git push -u origin main  

…or push an existing repository from the command line  
it remote add origin https://github.com/имяПользователя/проект.git  
* git branch -M main  
* git push -u origin main  

Commands
------------------------
* git init
// This command will create a .git repository in your project. A repository or "repo" is a collection of all the changes that have been made since the initialization of the repository. This is the first thing to do for a new project.

* git add filename.extension
// Replace "filename.extension" with whatever file you're trying to commit, such as "index.html". This command will add the file to the "staging area". Think of the staging area as a section in which files are being prepared to be moved into your repository.

* git add .
// If you want to add everything from the project directory to the staging area, then this command will do everything by itself.

* git add *.html
// If you want to add all .html files to the staging area then this command is fine. The extension can be changed depending on preferences.

* git status
// Shows what has already been added to the staging area and what files have been changed and are waiting to be moved to the staging area.

* git reset filename.extension
// Removes the selected file from the staging area. Removes a commit and reverts to changes.

* git rm --cached filename.extension
// Removes the file from the staging area and sets it to be ignored.

* git commit -m "Commit description"
// Takes files from the staging area and "commits" them to your local repository. In quotes, you should insert a brief description of the changes for a particular commit. Try to describe the commit in concise detail, for example: “fixed the problem when changing the username” instead of such messages as “some changes”

* git commit -a -m "Commit description"
// Creates a commit and indexes the state of the repository

* gitlog
// Commit Viewer, lists the commits made to the repository in reverse chronological order

* git show commit name
// Shows what changes happened in the specified commit.

* git checkout “branch or commit name”
// Switches to the specified commit or branch, depending on what you specify. Allows you to switch control over the branch you created and work within it. Here you can make any changes to the code. When you're ready, you can commit the changes and push the changes to GitHub (more on that below), or you can delete the branch if something went wrong or you no longer need the changes made in that branch.

* git rm -- cached -r .
// Removes index file tracking from the Stage Area.

* touch .gitignore
// This command will create a file called .gitignore. You can open this file in a text editor and type in the names of files or directories that you don't want to be tracked (they will be ignored by Git). Changes to ignored files will not show up when doing git status.

* git branch
// Displays all branches in the current repository

* git branch name
// Creates an entity called branch. A branch is an exact copy of your files.

* git branch -m branch name
// Rename the current branch

* git branch -d name
// Deletes the branch, in the name of the branch we indicate which branch we should delete.

* git checkout -b “branch name”
// Creates a new branch and changes to it.

* git merge nameBranches
// While on the master branch, you can use this command to take commits from any of the branches and merge them together. Merging another branch (feature branch) into the main branch (receiving branch).

* git revert
// A safe way to undo the operation without losing the commit history. The command undoes past commits, creating a new one containing all the undone changes. This command is useful when you have already pushed changes to a remote repository, as it keeps the original commit intact.

* git fetch
// Upload commits, files, and links from the remote repository to your local repository. Fetch the data with the fetch command if you want to see what others are working on.

* git remote add origin https://github.com/username/project.git
// This command will determine the "location" of your remote repository. Everything that happened before happened exclusively in the local repository on your computer. You will need to go to your GitHub account and create a new remote repository where you can push changes from your local repository. After you created your remote repository you will be provided with a link and that link is the location you will want to use in the above command.

* git remote -v
// Shows a binding to a remote repository

* git log --oneline --graph
// Displays a visual list of changed branches.

* git diff filename
// Displays the latest changes to the file.

* git remote
// Lists all remote repositories that have been added to your project.

* git remote show -n name
// to view information in a remote repository, use the same command, but with a name. The -n option is used to not establish a connection with the repository itself when executing the command, but to use only locally cached information.

* git push -u origin master
// This command will push the local changes to the remote repository. Thus, this command should be registered only the first time.

* git push
// submits your project with all changes to GitHub

* git push --delete origin branch name
// Deleting the branch we pushed to the remote repository

* git push -all
// Push all branches to the remote repository

* git clone https://github.com/username/project.git
// If you do not have a project on your personal or work computer, then this command will clone/download the entire project into the current directory.

* git-pull
// If you are working on the same project with multiple people, this command will download the latest version from the remote repository and update your local version.

* rm README.txt
// Delete file.

* mkdir directory name
// Creates a new directory

* githelp
// Calls up help

* help command
// Brief help on the command.

Git config
------------------------

* git config --global user.name "Your Name"
* git config --global user.email "yourmail@mail.com"
// These commands will define the information that will be used on each commit. You only need to run them once during your first Git installation.


![picture1.](git.jpg)

