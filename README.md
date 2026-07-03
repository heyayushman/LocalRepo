# Learning Git Basic
### Git Configuration :
git config --global user.name "My Name"
<br>
git config --global user.email "My email"

### To check git setup:
git config --list

## Clone: Cloning or copying a repo from github to our local system
git clone <-link of github repo->
<br>

cd - change directory, go inside to another directory : cd folder name
<br>

### To view all the files in a folder : ls

## status : view the status of the code : git status

* There are four types of status
1. untracked : new files that git does not yet track
2. modified : files which are changed
3. staged : files are ready to be committed
4. unmodified : unchanged files

### after creating modification, we need to add files to the stage, we need to add before committing any repo : git add <-link->

#### git add . : used to add all files

## commit : it is the record of changes made in repository
git commit -m "some meaningful message"

### Example:
1. Create a new folder : git add <-new file name->
2. check : git status
3. <-new file added-> (staged)
4. git commit -m "new folder created"

### push : used to upload local repo content to remote repo
git push origin main


## Create new folder in local system and initialize the git into it, so that it can be viewed in github

### Init command : Used to initialize git to a new folder, created in local computer

git init

### Let's create a new folder and initialize git into this

file name : GitRepo

PS C:\ LocalSystem > mkdir GitRepo

#### mkdir : make directory, command to create new folder ==> mkdir folder name

After creating new folder, run <-git init-> to initialize git into the new folder (run this two time)

PS C:\LocalSystem\GitRepo > git init

* Now, come to github and create a new repository with same name or any name, then copy the repo link
* Again, in the terminal run > git remote add origin <-link->
* make sure your're on the correct directory by running <- git remote -v ->
* check in which branch we are in > git branch > it will show *master
* change it to *main > git branch -M main
* Branch name will be changed

### Now, we can push code into github

* git push origin main
* Also, we can use > git push -u origin main (it will always push the code to origin main, no need to do it manually)

* git push > all the code, changes made in code will be pushed to git





