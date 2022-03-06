# :flags: What is Git? 

## :star: Tutor | Course overview and learning outcomes 

Tutor is [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix) <br>
The goal of this course is to introduce you to Git. We’ll also provide you with materials for further learning. 🚀

## :octocat: Git

**Git is a fast, versatile, highly scalable, free, Open Source Distributed Version Control System. Its primary author is Linus Torvalds, the creator of Linux.** That's a lot of grammar especially if you are just getting started with this whole thing about Git.

Let's backup and examine a scenario to help you understand. <br>
Let's say you just got started programming and you decide to build a Blog website with your two of friends who also just got started programming too. After planning with your friends what the website would look like and what features to implement, you get down to writing code. But then since you realize that there is need for the three of you to keep track of what the other is doing. You also realize that you may want to undo certain changes that you cannot undo after days or weeks, or you may want to have a backup of your project somewhere should anything happen to your computer. You realize that there is need for all these things to happen without hindering your workflow. 

Then enters Git. :relieved:

![Git entrance](https://media.giphy.com/media/dqiwnLsJJmkWMNNUpj/giphy.gif)

Back to the definition, Git is a Version Control System, not just any VCS but a Distributed Version Control System. It may seem like I'm repeating words but I'm doing that to help you understand.
There have been earlier instances of VCSes, such as CVS, Subversion (SVN), and Perforce. These VCSes used a centralized server to store a project's history. This centralization meant that the one server was also potentially a single point of failure.
Git is distributed, which means that a project's complete history is stored both on the client(the developer in this case) and on the server. You can edit files without a network connection, check them in locally, and sync with the server when a connection becomes available. If a server goes down, you still have a local copy of the project. Technically, you don't even have to have a server. Changes could be passed around in e-mail or shared by using removable media, but no one uses Git this way in practice.

In relation to the example scenario above,real life projects generally have multiple developers working in parallel. So a version control system like Git is needed to ensure there are no code conflicts between the developers.
Additionally, the requirements in such projects change often. So a version control system allows developers to revert and go back to an older version of the code.
Finally, sometimes several projects which are being run in parallel involve the same codebase. In such a case, the concept of branching in Git is very important.

A version control system (VCS) is a program or set of programs that tracks changes to a collection of files. One goal of a VCS is to easily recall earlier versions of individual files or of the entire project. Another goal is to allow several team members to work on a project, even on the same files, at the same time without affecting each other's work.

Another name for a VCS is a software configuration management (SCM) system. The two terms often are used interchangeably—in fact, Git's official documentation is located at git-scm.com. Technically, version control is just one of the practices involved in SCM. A VCS can be used for projects other than software, including books and online tutorials.

With a VCS as Git, you can:

  * See all the changes made to your project, when the changes were made, and who made them
  * Include a message with each change to explain the reasoning behind it.
  * Retrieve past versions of the entire project or of individual files.
  * Create branches, where changes can be made experimentally. This feature allows several different sets of changes (for example, features or bug fixes) to be worked on at the same time, possibly by different people, without affecting the main branch. Later, you can merge the changes you want to keep back into the main branch
  * Attach a tag to a version—for example, to mark a new release.

## Summary
Git, created by Linus Torvalds, the creator of Linux, is a **distributed Version Control System (VCS)**, which means it is a useful tool for easily tracking changes to your code, collaborating, and sharing. With Git you can track the changes you make to your project so you always have a record of what you’ve worked on and can easily revert back to an older version if need be. It also makes working with others easier—groups of people can work together on the same project and merge their changes into one final source!

## 📚  Resources 
* [A short video explaining what GitHub is](https://www.youtube.com/watch?v=w3jLJU7DT5E&feature=youtu.be) 

### Next Step :arrow_right:
Go to [What is Github?](./3_what_is_github.md)
