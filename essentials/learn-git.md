# Beginner's Guide to Git
Git is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. This guide covers the basics you need to know to get started with Git.

<img src="https://www.miximum.fr/wp-content/uploads/2013/07/git_workflow.png">

### Why Version Control?
Version control is essential in software development, providing a safety net for code changes, facilitating team collaboration, and preventing data loss. It enables tracking of modifications, easy rollback to functional states, and streamlined integration of concurrent updates, significantly enhancing project efficiency and continuity.

## Installation
Before you can use Git, you need to install it on your computer.

#### For Windows:
Download the installer from the [Git official](https://git-scm.com/) site.
Follow the installation steps using the wizard.
#### For Mac:
1. Install Homebrew, then run `brew install git` in the terminal.
2. Alternatively, download the installer from the [Git official site](https://git-scm.com/) and follow the prompts.
#### For Linux:
Stop reading this guide you know what you're doing.

## Setting up Git
After installing Git, set your username and email address, which are used in your commits. Run the following commands in your terminal:

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

## Starting a Repository
To start using Git, you need to initialize a repository, a virtual storage of your project, allowing you to record changes and revert to previous versions if needed.

* To initialize a new repository, navigate to your project's directory in the terminal and type:
```bash
git init
```
* to clone an existing repository, use:
```bash
git clone https://github.com/username/repository.git
```

## Git Basic Commands
Here are basic commands you'll use frequently in Git:
* **git status:** Check the status of your repository including staging, modifications, and branch information.
```bash
git status
```
* **git add:** Add changes in your working directory to your staging area.
```bash
git add . # add all files in directory
```
```bash
git add {filename} # add a particular file
```
* **git commit:** Commit your changes and record what you did within the commit message.
```bash
git commit -m "Commit message"
```
* **git log:** View the version history for the current branch.
```bash
git log
```

## Working with Branches
Branching is a feature that lets you work on different versions of a repository at one time. This is particularly helpful when in the process of iterating on a stable design, developing experimental features, or when working as a team.
* **git branch:** List all the branches in your repo, and also tell you what branch you're currently on.
```bash
git branch
```
* **git checkout:** Switch to a specific branch and update the working directory.
```bash
git checkout {branchname}
```
* **git merge:** Merge changes from one branch into another.
```bash
git merge {branchname}
```

## Merging Changes
When you're ready to merge changes from one branch into your main branch (often `master` or `main`):

1. Switch to the main branch:
```bash
git checkout main
```

2. Merge the feature branch into the main branch
```bash
git merge {feature-branch-name}
```

## Resolving Conflicts
Sometimes, Git can't automatically resolve conflicts between two branches. When this happens, you must resolve the conflicts manually by editing the files shown by Git.

1. Edit the files to fix the conflicts.
2. Add the resolved files by using git add.
3. After resolving all conflicts and testing your code, commit the changes.

## Remote Repositories
Remote repositories are versions of your project hosted on the Internet or network. View our resource on GitHub!
* **git push:** Uploads all local branch commits to GitHub.
```bash
git push # uploads all local branch commits to github
```
* **git pull:** Fetch and download content from a remote repository and immediately update the local repository to match that content.
```bash
git pull # updates your local working directory to the most recent version on github
```

If this isn't making sense, take a glance at this image. Sometimes a picture is worth a thousand words.
<img src=https://pbs.twimg.com/media/FjJ62xKXkAYfFjt.jpg>
