# :flags: Understanding Git terminlologies

## :star: Tutor | Course overview and learning outcomes 

Tutors: [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix) and [Nworie Kingsley](https://github.com/nworiekingslee) <br>
The goal of this course is help you understand commonly used Git terminologies. 🚀

---
### Git States
Growing up, my mum gave me a job. She would always give some money to me to save in a piggybank (Kolo, as we locally call it) almost everyday as she returns from work. On Friday I would take the kolo into a bank, round up the money and deposit it. Git states works in a similar way.

#### Modified
This means there's new file(s) or new changes that is not tracked by git. It is that straight forward. Using my analogy, think of my mum as a developer and I as git except instead of tracking and managing code, it's money. When my mum comes back from work, whether or not she has some change to save, I wouldn't know unless she calls me and tell me so. Same goes for git, git won't track your changes until you tell it to do so.

#### Staging
This is also called index. This means git is now aware of the new changes and can now track the file(s). You can take your code to the staging area by runing `git add file1`. This means that file1 is now tracked and it's changes is ready to be commited. Back to my analogy again. This stage is where my mum delivers the money into my hands after work, now I am aware of the new input and I can record it.

#### Committed
This takes the current state of the code, the person who made the change, the time, commit message and store it in the git repository like a snapshot with a unique commit ID. This help us track project history and prepare the code to be pushed to the remote. Based on the analogy, committed is related to the money that has made it into the Kolo (piggybank) ready to visit the bank on Friday.

---
### Git init

```git init``` is used to initialize a repository. It is what tells Git to start tracking files in that repository. When you run the command, your project folder becomes a repository and you can now use the full features of Git in your repo. 

---
### Git add
```git add``` adds new or changed files in your working directory to the Git staging area. git add is an important command - without it, no ```git commit``` would ever do anything. 
Git add selects a files or files, and moves it to the staging area, marking it for inclusion in the next commit. You can select all files, a directory, specific files, or even specific parts of a file for staging and commit. ```git add``` and ```git commit``` go together hand in hand. They don't work when they aren't used together. And, they both work best when used thinking of their joint functionality.

 - To add a specific like a README.md, you use ```git add README.md``` 
 - To add all files, you use ```git add .``` The period asks git to store all files and directories in the repository.
 - To add a specofic folder like images, you use ```git add /images```

---
### Git commit
Commits are the building blocks of "save points" within Git's version control. <br>
```git commit``` creates a commit, which is like a snapshot of your repository. These commits are snapshots of your entire repository at specific times. You should make new commits often, based around logical units of change. Over time, commits should tell a story of the history of your repository and how it came to be the way that it currently is. Commits include lots of metadata in addition to the contents and message, like the author, timestamp, and more.

 - git commit: This starts the commit process, but since it doesn't include a -m flag for the message, your default text editor will be opened for you to create the commit message. If you haven't configured anything, there's a good chance this will be VI or Vim.
 - git commit -m "descriptive commit message": This starts the commit process, and allows you to include the commit message at the same time.
 - git commit -am "descriptive commit message": In addition to including the commit message, this option allows you to skip the staging phase. The addition of -a will automatically stage any files that are already being tracked by Git (changes to files that you've committed before).
 - git commit --amend: Replaces the most recent commit with a new commit. (More on this later!)

---
### Git Push
```git push``` uploads all local branch commits to the corresponding remote branch. <br>
git push updates the remote branch with local commits. It is one of the four commands in Git that prompts interaction with the remote repository. You can also think of git push as update or publish. <br>

By default, git push only updates the corresponding branch on the remote. So, if you are checked out to the main branch when you execute git push, then only the main branch will be updated. It's always a good idea to use git status to see what branch you are on before pushing to the remote. If you are in a different branch that has not yet been created on the remote repository, you can create it when you push by doing ```git push -u origin [branchname]```
Also, if you setup your repository with ```git init``` and not by cloning, when pushing for the first time you have to use ```git push -u origin main``` assuming that the name of the branch is **main** ( which is the default branch name when you create a new repository ) 

As best practice, it's important to run the git pull command before you push any new changes to the remote branch. This will update your local branch with any new changes that may have been pushed to the remote from other contributors. Pulling before you push can reduce the amount of merge conflicts you create on GitHub - allowing you to resolve them locally before pushing your changes to the remote branch.

 - git push -f: Force a push that would otherwise be blocked, usually because it will delete or overwrite existing commits (Use with caution!)
 - git push -u origin [branchname]: Useful when pushing a new branch, this creates a branch with that name on the remote repository with a lasting relationship to that local branch, so that next time you only have to do ```git push [branchname]``` or just ```git push``` from that branch.
 - git push --all: Push all branches
 - git push --tags: Publish tags that aren't yet in the remote repository
See all options of using ```git push``` in the [documentation](https://git-scm.com/docs/git-push)

---
### Git Pull
The ```git pull``` command is used to fetch and download content from a remote repository and immediately update the local repository with that content. Merging remote upstream changes into your local repository is a common task in Git-based collaboration work flows. The git pull command is actually a combination of two other commands, git fetch followed by git merge. In the first stage of operation git pull will execute a git fetch to get content from the remote repository to the local repository. Once the content is downloaded, git pull will enter a merge workflow where it will merge the updated content with the local content on your local repository.

It's a good idea to run git pull regularly on the branches you are working on locally.
Without git pull, (or the effect of it,) your local branch wouldn't have any of the updates that are present on the remote.

---
### Git Clone

Git Clone is a feature which is used to target an existing repository and create a clone, or copy of the target repository. In the command line or Terminal, the command is ```git clone``` followed by the link to the repository which can be found on Github. 

<img src="https://static.javatpoint.com/tutorial/git/images/git-clone.png" />

To copy a git repository link, go to the repo on Github and click on green button that says ```Code```
In the dropdown box that appears, make sure ```https``` is selected, then click the icon next to the link to copy it. Note that it must end in **.git**

<img src="https://itknowledgeexchange.techtarget.com/coffee-talk/files/2020/11/find-github-url.png" />

Once that is done, open Terminal or command line and enter ```git clone``` followed by the link to the repo as this ```https://github.com/mlscunizik/Build-Bootcamp.git``` Such that you now have ```git clone https://github.com/mlscunizik/Build-Bootcamp.git``` 

  - git clone [url]: Clone (download) a repository that already exists on GitHub, including all of the files, branches, and commits.

  * Cloning on terinal
    <img src="https://images.ctfassets.net/nrgyaltdicpt/31ufabXrxuY0a0msQYWOUo/d8dc045fd128630eb0bfac07c8069884/Screen_Shot_2018-12-06_at_19.50.43.png" />

---
### Git Status

The ```git status``` command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information. Mostly, it is used to display the state between Git Add and Git commit command.

  - Here's a snapshot when you have done noting or when you have commited all files.
    <img src="https://static.javatpoint.com/tutorial/git/images/git-status.png" />
    
  - Status when there are changes. When we create a file in the repository, the state of the repository changes. Here's a snapshot.
    <img src="https://static.javatpoint.com/tutorial/git/images/git-status2.png" />
    
  - As we can see from the above output, the status is showing as "nothing added to commit but untracked files present (use "git add" to track)". The status           command also displays the suggestions. As in the above output, it is suggesting to use the add command to track the file.

    Let's track the file and will see the status after adding a file to the repository. To track the file, run the add command. Now see the output:
    <img src="https://static.javatpoint.com/tutorial/git/images/git-status3.png" />
    
   - From the above output, we can see that the status after staging the file is showing as "changes to be committed".
  
     Before committing blindly, we can check the status. This command will help us to avoid the changes that we don't want to commit. Let's commit it and then          check the status. Consider the below output:
     <img src="https://static.javatpoint.com/tutorial/git/images/git-status4.png" />

---
### Git Log
The advantage of a version control system is that it records changes. These records allow us to retrieve the data like commits, figuring out bugs, updates. But, all of this history will be useless if we cannot navigate it. At this point, we need the git log command. <br>
In an example Repo, typing the command ```git log``` gives this output:

<img src="https://static.javatpoint.com/tutorial/git/images/git-log.png" />

The above command is listing all the recent commits. Each commit contains some unique sha-id, which is generated by the SHA algorithm. It also includes the date, time, author, and some additional details.

Generally, the git log is a record of commits. A git log contains the following data:
 - **A commit hash**, which is a 40 character checksum data generated by SHA (Secure Hash Algorithm) algorithm. It is a unique number.
 - **Commit Author metadata:** The information of authors such as author name and email.
 - **Commit Date metadata:** It's a date timestamp for the time of the commit.
 - **Commit title/message:** It is the overview of the commit given in the commit message.
     
## Resources 
* [Git status](https://www.javatpoint.com/git-status)
* [Git Cheat Sheet](https://www.javatpoint.com/git-cheat-sheet)
* [Github's Documentation](https://git-scm.com/docs/git-commit)
* [Git Guides](https://github.com/git-guides/)
* [Git log](https://www.javatpoint.com/git-log)

# Week 1 Wrap up
This is the end of Week 1. You should now take your [assessment](https://forms.gle/KTEkixQDzessvcsP9).
Please note that you can only take your assessment once, as such please go through all learning materials and take your assessment confidently. Once you submit it, you cannot edit it or submit another.

## Next Step :arrow_right:
To find content for Week 2, Go to [Home](../../../)
