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

### 
---
## Background
### What's that
- **Git** - A way of doing version control for files.
- **Version Control** – A way of tracking changes to files and know what is the most recent.

---
## Structure
- Can be done totally locally but often uses a central repository (repo) so it is easier to collaborate.
- Each system has its own repository which is a complete history of the changes that have been committed and can synchronize one system’s repo with the central repo.

![An image of the working directory, staging area, and repository.  There is an arrow labeled "checkout the project" pointing from the repository to the working direction, an arrow labeled "stage fixes" pointing from the working directory to the staging area, and an arrow labeled "commit" pointing from the staging area to the repository.](./images/git_local_areas.png)  

from: https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F

---
### Working Directory
- This is the area you are working in
- The changes you make here are not in the repository till you commit them
- You can have untracked files 

#### Check Status 
This can be done with the ```git status``` command.

![An image showing a call to "git status".  It shows files not staged and untracked files.](./images/status.png)

---
### Staging Area
- This is where you have said what files you are getting ready to commit
- They are still not in the repository
- You just want to add the files relevant to the commit you are making.

#### Move file to the staging area
```git add <filename>```

![An image showing the use of "git add", followed by "git status" showing the added file in green in the staging area.](./images/add.png)

---
### Local Repository
- This is the place where all the versions of the code are stored
- It has a complete history of all the versions that have been added

#### Commit Files 
```git commit -m ‘<commit message>’```

**Takes the staged files and moves (commits) them to the local repository**
- Do it often and only stage files that are relevant.
- Give descriptive messages about what was done.
- Make commits only for code that is working, or note the issue.

![An image showing the use of "git commit"](./images/commit.png)

#### Repository Structure
Each version has a full copy of the repository at that point

![An image showing that when a file is changed and committed, those changes are tracked but a full copy of each file is created.](./images/versions.png)

From: https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F

####  Files not to use git for
- *Jupyter Notebooks* - Each time you run a section again it records it so you could not change anything about the file and it creates new versions, and then you and your collaborator would have conflicting versions that need to be resolved.
- *CAD Files* - These can be large and every version has a complete copy of all the files, so even if you aren’t changing it makes the repo huge.
- *Data Files*
- *Really any Large Files*

---
### Remote Repository
This is a central place where the repository can be stored for multiple people to access
It has the same repository (when everyone is updated), as the remote repositories

![An image showing the working directory, staging area, committed files (local repository), and remote repository.  There are is an arrow labeled "git add" pointing from the working directory to the staging area, an arrow labeled "git commit" pointing from the staging area to the local repository, an arrow labeled "git push" pointing from the local repository to the remote repository, an arrow labeled "git fetch" pointing from the remote repository to the local repository, and two arrows pointing from the local repository to the working directory labeled "git checkout" and "git merge".](./images/remote.png)

from: https://phoenixnap.com/kb/how-git-works

#### Send update to the remote
```git push```
- Many commits can be done prior to pushing

TODO: add image

#### Update the Local Repo Based on the Remote Repo
```git fetch```

TODO: add image

Update

#### Update the Working Directory from the Local Repository
```git merge```

TODO: add image

#### Fetch and Merge
```git pull```

TODO: add image

---
## Demo 
The demo will have 3 groups
1. Primary - The main person presenting they will demonstrate things to everyone.
2. Secondary - A person to help with the presentation by creating updates from another user that can be brought down.
3. Everyone - This is everyone else and some things we will want them to play with.

### Create Repo
- **Primary**
    - Open github.com and create a repository
    
    ![An image of the github page showing the new button in the top right](./images/github_repo.png)
    
    - Initialize an existing local repository
        ```
        cd <location to make repo>
        git init
        git add .
        git commit -m '<commit message>'
        ```
    - Connect the local repo to the remote
        - Assumes the local is already initialized and has committed files, and the remote repo already exists
        ```
        git branch -M main
        git remote add origin <git remote repo location>
        git push -u origin main
        ```
    
- **Secondary**
    - NONE
- **Everyone**
    - NONE

### Clone Repo
- **Primary** - 
- **Secondary** - 
- **Everyone** - 

### Make changes
- **Primary** - 
- **Secondary** - 
- **Everyone** - 

### Status
- **Primary** - 
- **Secondary** - 
- **Everyone** - 

### Add 

### Commit 

### Push 

### Fetch

### Merge

## Pull

## Merge

## Conflicts

## Branch

## Checkout

## Merge Branch

## gitignore


