# :flags: Understanding Github terminlologies

## :star: Tutor | Course overview and learning outcomes 

Tutor: [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix) and [Nworie Kingsley](https://github.com/nworiekingslee)<br>
The goal of this course is help you understand commonly used terms about Github. 🚀

### Repository

At the heart of Github is repositories. It's the basics for all other actions in Git and Github. A repository is your project folder that is git enabled. By this, I mean your project folder or codebase is not a repository untill you have enabled Git in it. To do that you musthave Git installed on your laptop and either use the Command prompt for Windows Os or Terminal for Linux/Mac OS users to initialize Git in your Project folder/codebase. If you use Viscual Studio Code, you can use the in-editor terminal. For an In-depth guide on how to do that, go [here](./set_up.md). When you initialize Git in your Projecct folder or Codebase, Git creates a hidden folder in the Project Folder now called a repository. The repository tracks all changes to build a history over time. All this changes are tracked and stored locally in your machine. If there are a number of people working on one Codebase, each of them would have a local copy of the Repository on their Computer and all of them would use the Remote Repository (explained below) as a source of truth or Central repository to keep track of the project and what the other is doing.

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQaZXkMudffpVLQ5NdoeZRDkSYQviFRrv7SXg&usqp=CAU" />

### Remote
This is also known as "Remote Repository". It is a git repository hosted on the internet. After using git to initialize a repository to track project changes on your local machine, you can equally create a repository on Github hosted on the internet. Git enables us to link the repository present in our local machine to the repository hosted on the internet allowing `push` and `pull` actions with the remote project.

This has alot of advantages, one major advantage is that it stores your project on the internet, now you can access and make changes to your project with or without the computer you used to start the project. 

### Branching
Branching is how git enables multiple developers to collaborate and work on a project by modifying the working codebase. When you create a branch, git creates a different codebase where you can make changes and modify files without affecting the main codebase which is usually on the main branch. A branch can be created using the terminal by running `git branch <new_branch_name>`.A branch can be created to fix a bug, work on a new feature, test out a way of doing something or whatever. After work is done on the branch, it is then merged (explained below) into the main branch and can either be deleted or continued to be used by the developer.

<img src="https://miro.medium.com/max/1400/1*JbVkbGtNh08HreFuEk_n4w.png" />
<img src="https://coderefinery.github.io/git-intro-stockholm/img/octopus.jpeg" />

### Merging
Once you’ve completed work on your branch, you can decide to merge it with the main branch. Merging simply means updating the main branch with changes from another branch in the same repository. When the `git merge <branch_name>` command is run, git scans through your branch for changes and updates the main (main branch) with found changes. 

<img src="https://www.w3docs.com/uploads/media/default/0001/03/e0f0e9e14db945c07e1fc0f3b2460ac19e0f738f.png" />

### Merge Conflicts
Sometimes merging a branch to the main isn't as straight forward as writing a single command on the terminal. In a scenerio where two developers are working on the same file in a project from different branches, the first merge from the first branch might have no conflict but when you try to merge the second branch, there will be a merge conflict especially when both branches modified the same file. Reason for the conflict is that git doesn't know which version of the file to keep. Everytime there's a merge conflict, git shows you every line of code that has a conflict and you'll have to manually decide which part of the code stays and which goes. While resolving merge conflict on the terminal, it is important that you delete the merge markers along side the unwanted code.

<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTG6sl8C5TrHmqhJ7TQ95cjKD0P2usVmvwfsw&usqp=CAU" />
<img src="http://www.cs.utsa.edu/~cs3443/git/merge-conflict.png" />

### Issues
GitHub Issues is a lightweight issue-tracking system that is available in all GitHub repositories. It is a simple tool that allows you to track your progress, keep a task list, collect feedback, and report bugs for your GitHub hosted project.
<img src="https://learn-the-web.algonquindesign.ca/topics/github-issues/issues-tab.jpg" alt="github issues" />

* Creating an Issue.<br>
  To create an Isuue, go to the issues tab and click on ```New Issue```
  <img src="https://learn-the-web.algonquindesign.ca/topics/github-issues/new-issue.jpg" />
  
  Then in the Write section, describe in detail what the problem is about. Once you are done, click on ```Submit new Issue```
  
  <img src="https://learn-the-web.algonquindesign.ca/topics/github-issues/write-issue.jpg" />
  
  You can tag people in Issues or assign them so that they are aware you are requesting help, add labels to keep issues organised, assign Issues to Projects, add links, make refereneces to file, to a line or lines of code and even add images. Issues support Markdown, which is what makes all of these possible. (Markdown is what this file is written in and what everything in this learning material for the Bootcamp is written in, so you can see that it's powerful.)

### Cloning

Git Clone is a feature which is used to target an existing repository and create a clone, or copy of the target repository. In the command line or Terminal, the command is ```git clone``` followed by the link to the repository which can be found on Github. 

<img src="https://static.javatpoint.com/tutorial/git/images/git-clone.png" />

To copy a git repository link, go to the repo on Github and click on green button that says ```Code```
In the dropdown box that appears, make sure ```https``` is selected, then click the icon next to the link to copy it. Note that it must end in **.git**

<img src="https://itknowledgeexchange.techtarget.com/coffee-talk/files/2020/11/find-github-url.png" />

Once that is done, open Terminal or command line and enter ```git clone``` followed by the link to the repo as this ```https://github.com/mlscunizik/Build-Bootcamp.git``` Such that you now have ```git clone https://github.com/mlscunizik/Build-Bootcamp.git``` 

  * Cloning on terinal
    <img src="https://images.ctfassets.net/nrgyaltdicpt/31ufabXrxuY0a0msQYWOUo/d8dc045fd128630eb0bfac07c8069884/Screen_Shot_2018-12-06_at_19.50.43.png" />

### Pull

### Fork

### Pull Requests


## Resources

[A video explaining Github Issues](https://www.youtube.com/watch?v=yAPSbIHcDTw)

### Next Step :arrow_right:
Go to [Understanding Git terminologies](./7_Understanding_Git_terminlologies.md)
