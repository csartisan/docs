---
title: Finalizing
layout: default
has_children: no
nav_order: 4
---

# Finalizing

This page will walk you through submitting your changes to [csartisan.org](https://csartisan.org)

## Required Reading

GitHub uses a unique form of version control where users will create [pull requests]() and [commits]().

### Commits

Similar to saving a file that's been edited, a commit records changes to one or more files in your branch. GitHub assigns each commit a unique ID, called a SHA or hash, that identifies:

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

One more step! Before your articles can be added to the website, you have to share your changes to GitHub. This process mostly stays the same, and is easy to memorize. Follow the steps below to finalize your changes.

{: .important }
Every computer is different! It is hard to supply the right guide for every user. If sections of this guide do not apply, please contact Club IT *(Call/Text: [{{ site.techcontact }}](tel:{{ site.techcontact }}))* for personalised instruction. We are very sorry. 

#### 1. Making a branch

1. Open GitHub Desktop,
2. Create a new branch `⌘ + ⇧ + N` (Command + Shift + N),
3. Name new branch the current date and your name (ex. `2023-03-04-octavia`),
4. If displayed, select __"Bring changes to new branch"__, then __"Switch branch"__,
5. In the box on the bottom left that says "Summary", write the current date and your name (ex. `2023-03-04-octavia`),
6. Press __"Commit to [new branch]"__,
7. Push changes to origin `⌘ + P`,

#### 2. Making a pull request

1. Press __“Preview Pull Request”__,
1. Make sure the base branch is `main` and that you have "from" set to your new branch,
1. Press __"Create pull request"__, this will open a browser window where you can edit information if you please to,
1. Double check all of your information is correct and press __"Create pull request"__.

Congratulations! You have successfully created a Pull Request with your new articles. As soon as a GitHub manager reviews your changes, your articles will be added on the website.