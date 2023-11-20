---
layout: post
title: Management and Collaboration with Git and Github
date: 2023-11-08
tags: general-skills
---

# The Problem

## Problem 1: If something really bad happens to the project, how can you undo errors?

Decent solution: save project backups

- Can quickly take up a lot of file space
- May not be able to undo minor changes between versions

## Problem 2: How do you get a bunch of developers to collaborate on the same project at once?

Bad solution #1: have everyone just edit code at the same time on the same files

- Might overwrite changes
- Half-done code will prevent other code from running
- Messy

Bad solution #2: have everyone make copies to make changes then people add their changes to the master version when everything is ready

- Half-done code will prevent other code from running
- Time consuming
- Messy

# Git

Git is a program used by developers to help manage their code.

## Features

- Very safe
- Lightweight
- Changes done locally
- Freedom in versioning patterns

## How it works

Projects in Git are called **repositories**.

Each change you make to your code in Git is called a **commit**. Commits can be undone in case of a mistake.

All code in a Git repository is stored on a computer called the **origin** server which is normally run by a third party company such as GitHub. Once the server has a repository, any developer given access to the repository can **clone** (copy) it to the local drive of a computer. Copied to a computer, developers can change code without immediately affecting the code that everyone else has access to. This allows multiple people to work on different features at the same time without other code changing around them.

Once an addition is done, developers can add their changes to the server by **pushing** (sending) the changes to update the origin. Other developers may check for changes like these at any time by fetching from the server. If a change is found, that developer may copy it to their computer by **pulling** the changes.

Let’s say two developers want to work on different features at the same time without interfering with the other’s code. To let both developers code in the same repository, Git allows the creation of **branches** that section off a group of changes to the code. This means the changes made on the branch do not go back to the original and changes to the original do not go to the branch. 

Once the changes are ready to be added onto the rest of the code, the branch can be **merged** into the original code. Sometimes changes are made in such a way that Git will not know how to handle them (often from different people changing the same line). This is called a **merge conflict**.

Every repository will have a main or master branch which is like the official version of the code. Well run repositories will make use of several other branches to work on individual features--the best repositories will have nothing done to the main branch directly--though these are normally deleted when the feature is complete.

Think of branches like parallel universes. The main or master branch is like the canonical universe. Branches you make are alternate universes. The actions you take on those branches are your commits. Then, you can merge them together to get the features of both.

It’s generally recommended that different developers should work on different features on a project at a time in different branches. When a developer is done making changes, they will submit a **pull request** which is like a final check before merging.

Systems like Git also enable the creation of open source software--free software with publicly available source code. This software can be edited and improved by anyone who knows how to code, allowing much quicker innovation. Many popular applications were created open source, including Blender, Python, Canvas, Firefox, and many more. If you want to play around with any of these, you can **fork** (make a copy of) the original repository and change the code.

# GitHub

**GitHub** is an online platform which will host your code repositories and allow you to share them with others.

**GitHub Desktop** is a software program which can help simplify using Git and Github.

# Activity

Prerequisite: Install VS Code or some other text editor

## Basic use with GitHub Desktop

1. Set up a GitHub account https://github.com/
2. Install GitHub Desktop https://desktop.github.com/
3. Make a repository in Github
4. Clone the repository to your computer with GitHub Desktop
5. Open the repository in VS Code
6. Make a commit on main
7. Make a new branch
8. Make a commit on the new branch
9. Push your changes
10. Submit a pull request
11. Merge the branch to main

## Using VS Code Git and Git commands

VS Code also supports managing Git repositories.

1. Install git-scm https://git-scm.com/
2. Open the repository from the activity before with VS Code
3. Try making a change to one of the files
4. Go to the sidebar and select the Git icon
5. Try committing and pushing the change

You can also use Git through commands with git-scm. However, command line usage is for a later lesson.
