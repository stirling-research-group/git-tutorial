# Git Demo Script
## Table of content
- [Do Ahead of Time](#do-ahead-of-time)
- [Background](#background)
    - [What's That](#whats-that)
    - [Structure](#structure)
- [Create Repo](#create-repo)
- [Clone Repo](#clone-repo)
- [Make changes](#make-changes)
- [Status](#status)
- [Add](#add)
- [Commit](#commit)
- [Push](#push)
- [Fetch](#fetch)
- [Pull](#pull)
- [Merge](#merge)
- [Conflicts](#conflicts)
- [Branch](#branch)
- [Checkout](#checkout)
- [Merge Branch](#merge-branch)
- [.gitignore](#gitignore)
## Do ahead of time
- Have the lab slack open for sharing link
- Have a GitHub account with SSH Setup
  - [Windows](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=windows)
  - [Mac](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=mac)
  - [Linux](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent?platform=linux)
- Have [git](https://github.com/git-guides/install-git) installed on your computer 
- Have a text editor you like available to modify files.

## Background
### What's that
- **Git** - A way of doing version control for files.
- **Version Control** – A way of tracking changes to files and know what is the most recent.

### Structure
- Can be done totally locally but often uses a central repository (repo) so it is easier to collaborate.
- Each system has its own repository which is a complete history of the changes that have been committed and can synchronize one system’s repo with the central repo.

![An image of the working directory, staging area, and repository.  There is an arrow labeled "checkout the project" pointing from the repository to the working direction, an arrow labeled "stage fixes" pointing from the working directory to the staging area, and an arrow labeled "commit" pointing from the staging area to the repository.](./images/git_local_areas.png)  
from : https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F

#### Working Directory
- This is the area you are working in
- The changes you make here are not in the repository till you commit them
- You can have untracked files 

#### Check Status 
This can be done with the ```git status``` command.

![An image showing a call to "git status".  It shows files not staged and untracked files.](./images/status.png)

#### Staging Area
- This is where you have said what files you are getting ready to commit
- They are still not in the repository
- You just want to add the files relevant to the commit you are making.

#### Move file to the staging area
```git add <filename>```
![An image showing the use of "git add", followed by "git status" showing the added file in green in the staging area.](./images/add.png)

## Create Repo

## Clone Repo

## Make changes

## Status

## Add 

## Commit 

## Push 

## Fetch

## Pull

## Merge

## Conflicts

## Branch

## Checkout

## Merge Branch

## gitignore

