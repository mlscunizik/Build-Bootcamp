# :flags: Saving changes

## :star: Tutor | Course overview and learning outcomes 

Tutor: [Akeem Qudus](https://github.com/holytech) and [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix)<br>
The goal of this course is to introduce you to get started using git and github comfortably to work effectively.🚀

## Periquisities
If you followed from week 1, then you know what a repository is and why it's necessary to use git and github. <br>
The guide in the module uses git commands and not the Github Desktop GUI. If you use the Windows OS, please use Git Bash (or Power Shell) and not Command Prompt. Git Bash is installed alongside when you install Git, if you don't have Git installed yet, download it for Windows from [here](https://git-scm.com/download/win). <br>
If you use Linux or Mac, use the Terminal. First make sure Git is installed by running the command ```git --version```. if you get an output like below, <br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20version.png?raw=true"><br>

then you have git installed. Otherwise if you get an error like ```-bash: git: command not found```, then install git with the command ```sudo apt install git```<br>

For a further guide on how to install Git on Windows, Mac or Linux; check [here](https://www.linode.com/docs/guides/how-to-install-git-on-linux-mac-and-windows/)<br><br>
With that out of the way, let's get started.

## Course Ouline
We'll go cover the following:
- Git init
- Git clone
- Git Config

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


## 📚  Resources 
* [A bullet summary of everything here by Akeem Qudus](https://docs.google.com/presentation/d/1K_Fj9X1VdctS1RVYVdldnx0yh1n5YaPpYCPgiFDuZCg/edit?usp=sharing) 

### Next Step :arrow_right:
Go to [Saving Changes](./2_Saving_changes.md)
