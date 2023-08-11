---
title: Docker
layout: default
parent: Other
has_children: no
nav_order: 1
---

# Hosting the site locally with Docker

## Required Reading

{: .tip }
If there is a word you don't understand, see the [glossary](/docs/glossary/) definition for that word.

{: .danger }
This section of the guide is unfinished.

Hosting a local website means setting up your computer so you can see your website in a web browser, just like how it will look online. It's like a practice run before you actually put your website on the internet for everyone to see. This helps you catch and fix any problems before your website goes live.

However, this can take a little to set up, and every computer is different, so be prepared to solve some of these issues yourself. I recommend only doing this if you believe you have enough computer skill to do so.

## Setting up Docker

[Docker](https://www.docker.com/) is a tool to run locally stored applications. It does this by creating "containers", which are isolated environments that contain all the necessary files and libraries to run an application. We use Docker as a simple, standard tool for hosting the website locally. This accesses the cloned copy of the GitHub repository to host a website that is only accessible from *your* computer, where you can make live changes to any part of the website.

### "What does this section set up?"
This section will guide you through setting up the following:
- [Docker](https://www.docker.com/)
- Docker Desktop

### Requirements
- Any web browser.
- A clone of the [GitHub repo](https://github.com/csartisan/csartisan.github.io) (See [Getting Started](/docs/getting-started/)).
- macOS, Windows, Linux (instructions for Chromebooks do not exist yet).
- Minor experience in your OS's terminal.
- 2.5GB or more of free storage space.

### Setting up Docker Desktop

Like [GitHub Desktop](/docs/getting-started/github.html#setting-up-github-desktop), Docker Desktop is a program that controls a command line tool. These are often reffered to as "Frontends" or "GUIs". Another great reason why we use Docker Desktop is because it installs all neccesary files that it requires to use, which saves you a LOT of time and trouble. You will not need to interact with Docker Desktop at all during this process once it is set up, as long as you keep the app running then the process will work.

#### Installing

To install Docker Desktop, navigate to [Downloads](https://www.docker.com/get-started/) and download the file that corresponds to your OS. 

You WILL need to make an account to use Docker. Follow the instructions in the app to complete installation. 

## Hosting the website

Hosting a local webiste means that you're running a copy of the site on your own computer in a web page. This is how you can test how the website will look before you publish it on the internet. 

1. Ensure that Docker Desktop is running.
   
   It doesnt need to be focused, as long as it's running in the background.

   macOS users can check this by viewing the Menu Bar for the Docker logo.

2. Navigate to the clone of the GitHub repo.
   ```bash
   cd Documents/GitHub/csartisan.github.io
   ```
3. Run the following command to access `dockercompose.yml`:
    ```bash
    docker-compose up
    ```
4. In a web browser, enter `localhost:4000` into the URL bar. 

This will result in what looks like the CSArtisan website. This is the website that *you* are running off of your clone of the website! Mess around with files in the clone and see them change after a refresh of the webpage. Congratulations! You have successfully started a local development session!

{: .tip }
You can end this process at anytime by pressing `ctrl + C`.