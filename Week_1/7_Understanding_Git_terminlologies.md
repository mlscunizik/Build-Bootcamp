# :flags: Understanding Git terminlologies

## :star: Tutor | Course overview and learning outcomes 

Tutors: [Nehemiah Onyekachukwu Emmanuel](https://github.com/devgenix) and [Nworie Kingsley](https://github.com/nworiekingslee) <br>
The goal of this course is help you understand commonly used Git terminologies. 🚀

### Git init

```git init``` is used to initialize a repository. It is what tells Git to start tracking files in that repository. When you run the command, your project folder becomes a repository and you can now use the full features of Git in your repo. 

### The three git states
Growing up, my mum gave me a job. She would always give some money to me to save in a piggybank (Kolo, as we locally call it) almost everyday as she returns from work. On Friday I would take the kolo into a bank, round up the money and deposit it. Git states works in a similar way.

#### Modified
This means there's new file(s) or new changes that is not tracked by git. It is that straight forward. Using my analogy, think of my mum as a developer and I as git except instead of tracking and managing code, it's money. When my mum comes back from work, whether or not she has some change to save, I wouldn't know unless she calls me and tell me so. Same goes for git, git won't track your changes until you tell it to do so.

##### Staging
This is also called index. This means git is now aware of the new changes and can now track the file(s). You can take your code to the staging area by runing `git add file1`. This means that file1 is now tracked and it's changes is ready to be commited. Back to my analogy again. This stage is where my mum delivers the money into my hands after work, now I am aware of the new input and I can record it.

#### Committed
This takes the current state of the code, the person who made the change, the time, commit message and store it in the git repository like a snapshot with a unique commit ID. This help us track project history and prepare the code to be pushed to the remote. Based on the analogy, committed is related to the money that has made it into the Kolo (piggybank) ready to visit the bank on Friday.

### Git Status
The ```git status``` command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information. Mostly, it is used to display the state between Git Add and Git commit command.

# Week 1 Wrap up
This is the end of Week 1. You should now take your [assessment](https://forms.gle/KTEkixQDzessvcsP9).
Please note that you can only take your assessment once, as such please go through all learning materials and take your assessment confidently. Once you submit it, you cannot edit it or submit another.

## Next Step :arrow_right:
To find content for Week 2, Go to [Home](../../../)
