---
title: Finalizing
layout: default
has_children: no
nav_order: 4
---

# Finalizing

{: .danger }
This section of the guide may not have accurate information, but the steps have been tested on Windows 10 and macOS Ventura. Please report any problems. Thank you for contributing.

## Required Reading

GitHub uses a unique form of version control where users will create [pull requests]() and [commits]().

### Commits

Similar to saving a file that's been edited, a commit records changes to one or more files in your branch. Git assigns each commit a unique ID, called a SHA or hash, that identifies:

- The specific changes
- When the changes were made
- Who created the changes

When you make a commit, you must include a commit message that briefly describes the changes.

See [Commits](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/about-commits) for more info.

### Branches

Branches allow you to develop features, fix bugs, or safely experiment with new ideas in a contained area of your repository. The website is loaded based on the `main` branch and all developer changes are first made to the `staging` branch. 

### Pull Requests

Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch. Once you've created a pull request, you can push commits from your topic branch to add them to your existing pull request. Other contributors can review your proposed changes, add review comments, contribute to the pull request discussion, and even add commits to the pull request.

See [Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) for more info.

## Submitting changes

#### 1. Making a branch

1. Open GitHub Desktop,
2. Create a new branch `⌘ + ⇧ + N`,
3. Name new branch the current date and your name (ex. `2023-03-04-octavia`),
4. Select __"Bring changes to new branch"__, then __"Switch branch"__,
5. Press __"Commit to [new branch]"__,
6. Push changes to origin `⌘ + P`,

#### 2. Making a pull request

9. Press “Preview Pull Request”,
10. Make sure the base branch is `main` and that you have "from" set to your new branch,
11. Press __"Create pull request"__, this will open a browser window where you can edit information if you please to,
12. Double check all of your information is correct and press __"Create pull request"__.

Then, you will wait for approval from a GitHub manager.