---
title: GitHub
layout: default
parent: Getting Started
has_children: no

---
# GitHub

[GitHub](https://github.com) is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

{: .developers }
Contributing requires you to have made a GitHub account and been accepted into the CSArtisan GitHub Team. If you aren't on the team and need to be, please request access by contacting the development team, preferably with your school email.

CSArtisan uses GitHub to manage versions, manage edit permissions, and host the website. You will use GitHub as a place to submit added articles and have them reviewed by an editor. 

To continue, you need to make a GitHub account. You can do this by going to [github.com](https://github.com) and selecting and fulfilling the sign-up process. It is not necessary to select any pricing plan other than Free.

## Setting up GitHub Desktop

Once your account is created, we must download GitHub Desktop.

GitHub Desktop is a computer application that allows you to edit a GitHub repository as local files. It is important to be careful when using GitHub Desktop, as it is possible to lose contribution progress if you miss a step. 

### Installation

You can install GitHub Desktop on any supported operating system.

To install GitHub Desktop, navigate to [https://desktop.github.com/](https://desktop.github.com/) and download the appropriate version of GitHub Desktop for your operating system. Follow the prompts to complete the installation. For troubleshooting, see [Installing GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/installing-and-authenticating-to-github-desktop/installing-github-desktop).

When it has finished installing, open it and authenticate your GitHub account, this is to allow you to edit repositories that you are permitted to edit.

### Installing Git

Git is a command line tool that is necessary for using GitHub Desktop. If you do not already have Git installed, you can download and install the latest version of Git from https://git-scm.com/downloads.

Once Git has been successfully installed, you're ready to start using GitHub Desktop.

## Cloning the website

In GitHub, cloning refers to downloading a local copy of a repository. With this clone you will upload your fully formatted posts and "push" them- or sync them, using GitHub Desktop.

1. Open Github Desktop
2. Click "Current Repository" dropdown button in top-left corner,
3. Click "Add" dropdown button,
4. Select "Clone Repository...",
5. Select "URL" from top navigation bar,
6. Paste `https://github.com/csartisan/csartisan.github.io/tree/beta` in input space.
    - If this gives a red error that says "This folder already contains files...", the repository has already been cloned onto your device and you can continue.

Congratulations! You have created a local version of the website on your device. 

###### How to find your local repository

Accessing the files is easy. In a file explorer such as Finder, go to the following file path that corresponds to your operating system. Where `[USERNAME]` is the username of your current profile.

|macOS|Windows|
|---|---|
|`/Users/[USERNAME]/github/csartisan.github.io/` | `C:\Users\[USERNAME]\github\csartisan.github.io\` |

{: .important }
These paths are the default. The rest of the guide uses these paths, so move them at your own risk.

Making changes to these folders won't change the website just yet, but it is recommended not to change anything right now.

{: .next }
Proceed to [Markdown Editors](md/md-editors.html)