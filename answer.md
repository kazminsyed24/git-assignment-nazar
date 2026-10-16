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

## Answer: .gitignore file is a text file that lists files or folders to be ignored by Git and not included in a version control history, such as passwords, large folders or temporary files. This is the .gitignore file that excludes node_modules and any type of .env file node_modules/*.env.
