  # <u> -------------------- Git and GitHub -------------------- <u/>
  
  ## What is git and version control?
  - Git is a powerful tool the keeps track of every change you make to your file.
  - Everytime we make a change to our file, git records

        what changed
        when changed
        who changed
        where changed

  - Irrespective of any kind of files, git tracks the changes.

        which line has edited
        when it was edited
        who has edited

  - It also saves the data of files everytime it gets edited in the form of versions and we can access all these versions at anytime also we can get back to previous versions.

## Difference between git and github
  - Git is a tool that works locally on our computer.
  - It tracks all the changes that we made to our files and keep them organised.
 
  - Github acts as a central online server where we upload all our project code after completion.
  - That code is available to everyone in our project team and that can be edited by anyone at any time with permissions.

  - Github, Gitlab and Bitbucket are the same.

## Git is mainly divided into two major parts

  - Local (git-bash/computer : Refers to our own computer where, we work with our project and all the data of our project is stored.
  - Remote (github/gitlab/bitbucket) :   Lives in the cloud, we can access/pull the code, edit and upload/push the code to cloud.

## Get Started with Git

  - Now that Git is installed and configured, and it knows who you are, you can start using Git.

  - Lets create our first repository

### Key Steps to Get Started

  - Create a project folder
  - Navigate to the folder
  - Initialize a Git repository
  - Creating Git Folder
  - Start by creating a new folder for our project:

  - Example

        mkdir myproject
        cd myproject

        mkdir creates a new directory.
        cd changes our working directory.

  - Now we are in the correct directory and can initialize Git!

  - If you're using Windows, you can open Git Bash directly in your project folder:

## Initialize Git

  - Now that we are in the correct folder, we can initialize Git on that folder:

  - Example

        git init 
        Initialized empty Git repository in /Users/user/myproject/.git/

  - You just created your first Git Repository!

### What is a Repository?

  - A Git repository is a folder that Git tracks for changes.

  - The repository stores all your project's history and versions.

### What Happens When You Run git init?

  - Git creates a hidden folder called .git inside your project.

  - This is where Git stores all the information it needs to track your files and history.

  - Example: Show Hidden .git Folder (Linux/macOS)

        ls -a
        .  ..  .git

  - On Windows, you may need to enable "Show hidden files" in File Explorer to see the .git folder.

### Troubleshooting

    git: command not found
        Solution: Make sure Git is installed and added to your PATH. Restart your terminal if needed.
    Permission denied
        Solution: Try running your terminal as administrator (Windows) or use sudo (macOS/Linux) if needed.
