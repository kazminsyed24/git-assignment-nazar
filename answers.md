# Git Assignment — Answers
# Part 1 - Concepts & Theory

## Q1.1. What is a terminal? How is it different from clicking through folders in a file explorer?

## ANSWER: a terminal is a text-based window used to input commands to instruct the computer's processing. A file explorer is a graphical application for exploring files, which means you use the mouse to click on folders and icons. The terminal is more efficient for repetitive tasks and can be scripted, the file explorer is easier to use for novice users, but slower.

## Q1.2. Write the terminal command to: (a) list all files including hidden ones, (b) create a folder called project , (c) move into that folder?

## ANSWER: the command ls a displays all the files, hidden or not (b) the command mkdir project makes a folder called project and (c) the command cd project changes the directory to project.

## Q1.3 What does the cd .. command do? What about cd ~?

## ANSWER: cd ~ takes you to the home folder, from anywhere.cd .. moves to the parent folder or ex folder above the one from which you are issuing the command.

## Q2.4.Explain what version control is in your own words. Give one real-world analogy (not Google Docs — pick your own)

## ANSWER: version control is a tool that allows you to keep track of any changes made to the files you save, which you can later access to return to an older version, view what has been changed, It's similar to a photo album of a building on the go each photo depicts the building at a specific point in time, so you have the option to look at any stage if something isn't going your way.

## Q2.5. What is the difference between Git and GitHub? Can you use Git without GitHub?

## ANSWER: git is a free application that you can install on your computer that will be used to monitor changes in your code. GitHub is a web based platform for hosting repositories which are shared and collaboratively developed. you can use Git without GitHub Git works fully on your own computer.

## Q2.6. Name three features GitHub provides that Git alone does not?

## ANSWER: you get online storage for your repositories ability to submit pull requests for code review by team members identify bugs and schedule tasks. It also provides GitHub actions for automation and project boards.

## Q2.7 What is a repository? What is the difference between a local repository and a remote repository?

## ANSWER: a repo is a project folder that contains all project files and complete history of changes. It is available as a local repository and can be used without the internet. A remote repository is a repository that is hosted on a server like GitHub or GitLab and is used for backup and for sharing with others.

## Q3.8. Explain what HEAD means in Git. What happens to HEAD when you switch branches?

## ANSWER: HEAD is a pointer that indicates where you are currently in the repository upon branch switching HEAD points to the new branch and your files are updated to reflect the new HEAD's latest commit in that branch.

## Q3.9. What is a .gitignore file? Write a .gitignore that ignores: all called node_modules/ , and any file ending in .env .?

## Answer: A `.gitignore` file tells Git which untracked files and folders to ignore. For example, it can exclude log files, installed dependencies, and environment configuration files.
## *.log
## node_modules/
## *.env
## Exercise 2.2
## Q2.6. 
## Answer: we did this to keep them organized. This make commit easier to find mistakes, undo changes and easier to understand. when changes have seperate purpose we should split commits. 

## What would happen if you made a local commit first WITHOUT pulling? What command helps you check?

## ANSWER: if local commit before pull, local branch and github branch may have different commits. because when i try to push it will reject because i dont have it locally. git status will help and git log --online to check  commit history.

## Exercise 3.1(9)
##
## since feature branch is created. fast forward merge happens when the main branch has no new commits. Git simply moves the main branch forward without creating a new merge commit. when both branch have different new commits a merge commit happens. Git join the branches.

## 3.2(15)

## ANSWER: 1. the conflic happen when both branches changed same line in same file. 

## 2. No, Git can normally marge changes made to different line automatically.

## 3. no, usually there would not be a  conflict.


## Exercise 4.1 — Feature branch workflow

## 1. What is the purpose of a pull request? Why not just merge directly?

## a pull request let other to review changes before they add to main branch. it helps to find mistakes.
## 2. Name two things a reviewer should check in a pull request.

## check for code works correctly 
## correct for erros bus

## 3. What is the difference between a merge commit and a fast-forward merge?

## a merge commit joins two branch histories by creating a new commit a fastforward merge moves the main branch pointer forward when there are no separate new commits on main that need to be joined.

## PART 5 - MERGE CONFLICT SCENARIOS
### Scenario A
## no conflict ahmed changed line 10 and sara changed line 1 they are distinct branches and Git can automatically merge both changes.

### Scenario B
## no conflict Ali made modifications to style.css and Fatima made modifications to app.js. they are two different files so git cant conflict.

### Scenario C
## yes there will be a conflict but it will be resolved. both developers changed the same line line 5 of the same file to different value so Git cannot choose one the file would contain the following
### Scenario C
## <<<<<<< HEAD
##  DEBUG = True
##    =======
##    DEBUG = False
##    >>>>>>> dev-b-branch
### Scenario C
## there will be conflict Both developers modified line 5 of config.py to other values, and this makes it impossible to select one from Git. The file would look like this:

  ##   <<<<<<< HEAD
  ##   DEBUG = True
  ##  =======
  ##  DEBUG = False
   ## >>>>>>> dev-b-branch

## The part between <<<<<<< and ======= is the current branch HEAD. The branch to be merged in is indicated between >>>>>>> and =======

### Scenario D
## git status – displays the list of files with conflicting changes. 2. Open index.html in VS Code and find the markers <<<<<<<, ======= and >>>>>>>
## In this step retain the proper code (or both codes) and remove all of the marker lines.
## 4. Save the file
## 5. git add index.html
## 6. git commit -m "fix: resolve merge conflict in index.html"
## 7. git checkout master

### Scenario E
## it is a good practice. you get your teammates latest work before you start. If you skip it you may work on old code your push can get rejected and you are at a higher risk of merge conflicts later.
