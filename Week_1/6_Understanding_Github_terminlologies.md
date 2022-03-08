# :flags: Understanding Github terminlologies

## :star: Tutor | Course overview and learning outcomes 

Tutor: [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix) <br>
The goal of this course is help you understand commonly used terms about Github. 🚀

## Repository
A git repository is a hidden directory created in our project directory. It is the `.git/` folder inside your project directory. The repository tracks all changes to build a history over time. All this changes are tracked and stored locally in your machine.
It is important to note that this .git/ folder known as the repository doesn't appear untill it is initialized using git. There's a number of ways to initialize a git repository. One way is by using the terminal. To initialized a git repository using the terminal, simply run `git init`.

## Remote
This is also known as "Remote Repository". It is a git repository hosted on the internet. After using git to initialize a repository to track project changes on your local machine, you can equally create a repository on Github hosted on the internet. Git enables us to link the repository present in our local machine to the repository hosted on the internet allowing `push` and `pull` actions with the remote project.

This has alot of advantages, one major advantage is that it stores your project on the internet, now you can access and make changes to your project with or without the computer you used to start the project. 

## Branching
Branching is how git enable multiple developers to collaborate and work on a project by modifying the working codebase. When you create a branch, git creates a different codebase where you can make changes and modify files without affecting the main codebase which is usually on the main branch. A branch can be created using the terminal by running `git branch <new_branch_name>`.

## Merging
Once you’ve completed work on your branch, you can decide to merge it with the main branch. Merging simply means updating the main branch with changes from another branch in the same repository. When the `git merge <branch_name>` command is run, git scans through your branch for changes and updates the main (main branch) with found changes. 

## Merge Conflicts
Sometimes merging a branch to the main isn't as straight forward as writing a single command on the terminal. In a scenerio where two developers are working on the same file in a project from different branches, the first merge from the first branch might have no conflict but when you try to merge the second branch, there will be a merge conflict especially when both branches modified the same file. Reason for the conflict is that git doesn't know which version of the file to keep. Everytime there's a merge conflict, git shows you every line of code that has a conflict and you'll have to manually decide which part of the code stays and which goes. While resolving merge conflict on the terminal, it is important that you delete the merge markers along side the unwanted code.

## Issues

## Cloning

## Fork

### Next Step :arrow_right:
Go to [Understanding Git terminologies](./7_Understanding_Git_terminlologies.md)
