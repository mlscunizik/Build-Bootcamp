# :flags: Setting up Git

## :star: Tutor | Course overview and learning outcomes 

Tutor: [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix)<br>
The goal of this course is to help you understand how to set up git on your computer.🚀

## Git Config
If you followed from week 1, then you know what a repository is and why it's necessary to use git and github. <br>
The guide in the module uses git commands and not the Github Desktop GUI. If you use the Windows OS, please use Git Bash (or Power Shell) and not Command Prompt. Git Bash is installed alongside when you install Git, if you don't have Git installed yet, download it for Windows from [here](https://git-scm.com/download/win). <br>
If you use Linux or Mac, use the Terminal. First make sure Git is installed by running the command ```git --version```. if you get an output like below, <br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20version.png?raw=true"><br>

then you have git installed. Otherwise if you get an error like ```-bash: git: command not found```, then install git with the command ```sudo apt install git```<br>

For a further guide on how to install Git on Windows, Mac or Linux; check [here](https://www.linode.com/docs/guides/how-to-install-git-on-linux-mac-and-windows/)<br><br>
<hr>

**The first thing you should do after installing Git on your system is to configure your git username and email address.** Git associate your identity with every commit you make. In order to perform git operations, Git needs to know which user is making those operations. For example, you cannot push to a private repository belonging to someones else if Git doesn't know that you have permissions to access that repository. 

Git allows you to set a global and per-project username and email address. You can set or change your git identity using the git config command. Changes only affect future commits. The name and email associated with the commits you made prior to the change are not affected.

### Setting Global Git Username and Email
The global git username and email address are associated with commits on all repositories on your system that don’t have repository-specific values. This means that for every repository you work with on your laptop the global user identity you set is what is used to store information about commits, unless otherwise specified in a specific repository.<br>

To set your global commit name and email address run the ```git config``` command with the ```--global``` option:<br>
```
git config --global user.name "Your Name"
git config --global user.email "youremail@yourdomain.com"
```

Do this without the quotes.<br><br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20config%20name.png?raw=true" /><br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20config%20email.png?raw=true" /><br><br>

Once done, you can confirm that the information is set by running:
```
git config --list
```

Which should give the output;<br>
<img src="https://github.com/devgenix/Photo-Backup/blob/main/Build%20Bootcamp/git%20config%20list.png?raw=true" />
```
user.email=emmanueln644@gmail.com
user.name=devgenix
```
<hr>
### Setting Git Username and Email for a Single Repository
If you want to use a different username or email address for a specific repository, run the git config command without the ```--global``` option from within the repository directory or use ```--local``` instead.<br><br>

First,navigate to that repository and open it in Git Bash or Terminal then type the commands; <br>
```
git config user.email "Your Name"
git config user.email "youremail@yourdomain.com"
```

replacing the quotes and its contents with your name and email respectively.<br><br>

With that out of the way, let's get started.

## 📚  Resources 
* [A Video explaining how to set up Git](https://www.youtube.com/watch?v=jUlT-zQ-mbk) 

### Next Steps :arrow_right:
Go to your [Setting up a repository](./2_Setting_up_a_Repository.md)<br>
