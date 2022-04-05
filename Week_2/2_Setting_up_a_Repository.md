# :flags: Setting up a repository

## :star: Tutor | Course overview and learning outcomes 

Tutor: [Akeem Qudus](https://github.com/holytech) and [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix)<br>
The goal of this course is to introduce you to get started using git and github comfortably to work effectively.🚀

## Course Ouline
We'll go cover the following:
- Git init
- Git clone

## Git Init
To create a new repo, you'll use the ```git init``` command. Git init is a one-time command you use during the initial setup of a new repo. Executing this command will create a new .git subdirectory in your current working directory and makes it possible to start recording revisions of the project. This will also create a new main branch. Git init is used when you want to create a repository from scratch, in an empty project folder or an existing project folder. To create a repository with git init; <br><br>
• Open the project directory in
your file explorer (Windows) or finder
(Mac)
• Right click on the folder on inside the folder in an empty space, click “git bash
here” (Windows) or “open terminal here” (Mac or Linux)<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2013-20-31.png?raw=true" /><br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/folder%20empty.png?raw=true" /><br>

• Type “git init” and hit enter.<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2013-22-05.png?raw=true" /><br>

If you get a response like;<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2013-22-13.png?raw=true" />
```
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint: 	git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint: 	git branch -m <name>
Initialized empty Git repository in /home/devgenix/Documents/Build Bootcamp/.git/
``` 
then you've successfully created a repository.<br>
If you have enabled the option to see hidden files, you would see an otherwise hidden .git subdirectory created in that project folder.<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2013-22-33.png?raw=true" /><br>
This is the same thing you would do whether you are creating the repository in an empty project folder or in an already existing project.<br><br>

## Git Clone.
Git clone is used to create a copy or clone of remote repositories. If a project has already been set up in a central repository that is on Github, the git clone command is the most common way for users to obtain a local development clone to work with. Like git init, cloning is generally a one-time operation. Once a developer has obtained a working copy, all version control operations are then managed through their local repository. To clone a repository, type ```git clone``` and pass a repository URL. So that you now have;<br>
```
git clone <repository link>
```

When you do that, remove the braces ( ```<``` and ```>``` ).<br>
There are two ways to clone a repository, Https and SSH. In this example, we'll be using the Https method.<br><br>

First, go to that repository on Github;
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20clone%201.png?raw=true" /><br><br>

Click on the green button that says "Code"<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20clone%202.png?raw=true" /><br><br>

Make sure that "HTTPS" is underlined, then click on the icon next to the link. Once the icon changes to a check mark and you see a tooltip that says "Copied", you've successfully copied the repository link. <br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20clone%204.png?raw=true" /><br><br>

Links copied like this ends in ".git".<br>
Now to clone this repository, you would navigate to a directory(or a folder) where you want to put the repository, open that directory or folder in Git Bash or in terminal and type ```git clone``` then paste the link. To paste in Terminal, use Ctrl+Shift+V keys. As such you would now have;
```
git clone https://github.com/mlscunizik/Build-Bootcamp.git
```
Hit enter to clone the repository. If this is your first time setting up Git on your computer, there are a few things to configure. Read about it [here](./1_setting_up_git.md). <br>
If you are cloning a private repository, you'll be asked to enter your github username and password because Git needs to know if you have access to that repository. On Windows, if you are using Git Bash, you'll be prompted to open your browser and login. Git Bash would then save your credentials for further use. <br>
That brings us to the next thing, continuing **Git Config**<br>

## Git Config - Continued

Before going ahead to enter your github username and password, know that Github depreceated plain text passwords for tokens as a means of authentication since August 13, 2021, at 09:00 PST. You'll need to generate your token and store it safely because once generated on the Githubs' website you can't access it to copy it again. This is a security measure.<br>
These tokens are long and it's not adviced you store it carelessly, Git has something called Github Credentials helper that can store your authentication information for further use, so that you don't have to put in your username and token each time you pull/clone/push.<br><br>

To generate your token, Go to https://github.com and click on your profile picture at the top right corner of the page. <br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-28-51.png?raw=true" /><br><br>

Next, click on ```Settings```<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-28-57.png?raw=true" /><br><br>

You'll be presented with your settings page, scroll down and click on ```Developer Settings```<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-29-33.png?raw=true" /><br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-29-41.png?raw=true" /><br><br>

Click on ```Personal Access Tokens```<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-30-22.png?raw=true" /><br><br>

Click on ```Generate new token```<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-30-34.png?raw=true" /><br><br>

If you are asked to confirm your password, enter your password.<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/Screenshot%20from%202022-04-05%2011-30-40.png?raw=true" /><br><br>




## 📚  Resources 
* [A bullet summary of everything here by Akeem Qudus](https://docs.google.com/presentation/d/1K_Fj9X1VdctS1RVYVdldnx0yh1n5YaPpYCPgiFDuZCg/edit?usp=sharing) 

### Next Step :arrow_right:
Go to [Saving Changes](./2_Saving_changes.md)
