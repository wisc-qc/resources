# Beginner's Guide to GitHub
GitHub is a code hosting platform that uses Git (version control system) to collaborate on and manage projects. From open-source software to private team repositories, GitHub is an expansive, versatile platform. Having a single copy of local code on your personal laptop is dangerous. Instead, actively commit to a GitHub repository both as a means to back up your work and get it out to others.
## Table of Contents
- [Beginner's Guide to GitHub](#beginners-guide-to-github)
  - [Table of Contents](#table-of-contents)
  - [Understanding GitHub](#understanding-github)
  - [Setting Up Your GitHub Account](#setting-up-your-github-account)
  - [Creating a Repository](#creating-a-repository)
  - [Cloning Repositories](#cloning-repositories)
  - [Committing Changes](#committing-changes)
  - [Creating and Managing Branches](#creating-and-managing-branches)
  - [Pull Requests](#pull-requests)
  - [Merging Changes](#merging-changes)
  - [Understanding Issues](#understanding-issues)
  - [Collaboration and Contribution](#collaboration-and-contribution)
  - [Summary](#summary)

## Understanding GitHub

GitHub is more than just a website. It's a platform that supports a community of developers, projects, and collaborative endeavors. It hosts a vast array of resources along with network graphs, repositories, tools for managing change, and feature requests.

## Setting Up Your GitHub Account

1. Visit [GitHub](https://github.com/) and sign up for an account.
2. Choose a subscription plan. If you're new, you likely want to start with the free option.
3. Verify your email address.

## Creating a Repository

A repository (or 'repo') is like a folder for your project. It contains all of your project’s files and stores each file’s revision history.

1. Click the '+' icon on the top right of GitHub's navigation bar and select 'New repository'.
2. Name your repository, and add a brief description.
3. Initialize with a README if you want to include documentation.
4. Click 'Create repository'.

## Cloning Repositories

Cloning a repository creates a local copy of the remote repo. This allows you to edit the files in your preferred environment without altering the source files on GitHub. Here's how to clone a repository:

1. **Find the Repository**: Navigate to the main page of the repository that you're interested in.

2. **Copy the URL**: Under the repository name, click the "Code" button. Here you'll find the URL to clone the repository. Make sure you're copying the URL under "Clone with HTTPS" (it should look something like `https://github.com/username/repository.git`).

    ![Clone with HTTPS](https://docs.github.com/assets/images/help/repository/https-url-clone-cli.png)

    > Note: If you've set up SSH for GitHub, you can use the "Clone with SSH" option.

3. **Clone the Repository**: Open your terminal (for MacOS, Linux distributions) or command prompt/git bash (for Windows). Navigate to the directory where you want to clone the repository using the `cd` command.

4. **Execute the Clone Command**: Type `git clone`, and then paste the URL you copied earlier. It should look like this:
    ```bash
    git clone https://github.com/username/repository.git
    ```
    Press `Enter` to create your local clone.

5. **Navigate into Your Cloned Repository**: Once the repository is cloned, you'll have a local version on your computer. Use the `cd` command to navigate into the directory of the cloned repository. Now, you can start working on it!

    ```bash
    cd repository
    ```

6. **Set Upstream (Optional)**: If you're planning on pulling updates from the original repository, set the 'upstream' to keep your local repository up to date. In your terminal, run:
    ```bash
    git remote add upstream https://github.com/username/repository.git
    ```
    This step is crucial if you're contributing to open-source projects or working with a team.

Now, you're all set! You have a local copy where you can develop, test, and run the code without affecting the live project. Remember to pull updates regularly if the repository is actively changing.


## Committing Changes

Committing is like saving a file. You can make any changes to your repository files and once you’re ready, you commit those changes.

1. Make changes to a file in your repo.
2. Write a short, meaningful commit message describing the changes.
3. Click 'Commit changes'.

## Creating and Managing Branches

Branches allow development work to happen parallel to the main branch, often referred to as 'main' or 'master', without disrupting the production version.

1. Go to your new repository and click the drop-down at the top of the file list that says 'branch: main.'
2. Type a branch name into the new branch text box.
3. Select 'Create branch'.

## Pull Requests

Pull requests announce your changes to other developers and request that someone reviews and pulls in your contribution and merges them into their branch.

1. Click the 'Pull Request' tab, then from the Pull Request page, click the green 'New pull request' button.
2. Select the branch you made your changes in.
3. Review your proposed changes.
4. Click 'Create Pull Request'.

## Merging Changes

After the pull request, when your changes get approved, you or someone else will merge the changes back into the main branch.

1. Go to your pull request.
2. Click the 'Merge pull request' button to merge the changes into the main branch.
3. Click 'Confirm merge'.
4. Once merged, you have the option to delete the branch that was merged.

## Understanding Issues

Issues are a great way to keep track of tasks, enhancements, and bugs for your projects. They’re kind of like email, except they can be shared and discussed with the rest of your team.

1. Click 'Issues' in the repository’s right sidebar.
2. Click 'New Issue'.
3. Give your issue a title and write a description for your issue.
4. Click 'Submit new issue'.

## Collaboration and Contribution

Collaboration in GitHub is as straightforward as sharing your repository with others. Contributors can make changes by pushing commits to the shared repository.

1. Share your repository link with collaborators.
2. They can clone your repository, create a new branch, make changes, and create a pull request.
3. Review the changes, then merge them into the appropriate branch.

## Summary

GitHub empowers you to work collaboratively with other developers, maintain version control, and manage your project's progress. This guide is just the starting point. As you get more comfortable, you’ll find that the platform has much more to offer.

---

Remember, the best way to understand GitHub is by using it. Don't hesitate to experiment, make mistakes, and ask the community for help. Good luck with your coding journey!
