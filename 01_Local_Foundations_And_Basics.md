# Phase 1: Local Foundations & Basics

## <u> What is Git? <u/>

  - Git is a popular version control system.

  - It was created by Linus Torvalds in 2005, and has been maintained by Junio Hamano since then.

  - It is used for:

        Tracking code changes
        Tracking who made changes, what are the changes made, when they chnaged, where they changed 
        Coding collaboration

## <u> Basic Terms <u/>

  - Repository: A folder where Git tracks your project and its history.
  - Clone: Make a copy of a remote repository on your computer.
  - Stage: Tell Git which changes you want to save next.
  - Commit: Save a snapshot of your staged changes.
  - Branch: Work on different versions or features at the same time.
  - Merge: Combine changes from different branches.
  - Pull: Get the latest changes from a remote repository.
  - Push: Send your changes to a remote repository.

## <u> Working with Git <u/>

  - Initialize Git on a folder, making it a Repository
  - Git now creates a hidden folder to keep track of changes in that folder
  - When a file is changed, added or deleted, it is considered modified
  - You select the modified files you want to Stage
  - The Staged files are Committed, which prompts Git to store a permanent snapshot of the files
  - Git allows you to see the full history of every commit.
  - You can revert back to any previous commit.
  - Git does not store a separate copy of every file in every commit, but keeps track of changes made in each commit!

## <u> Why Git? <u/>

  - Over 70% of developers use Git!
  - Developers can work together from anywhere in the world.
  - Developers can see the full history of the project.
  - Developers can revert to earlier versions of a project.

## <u> What is GitHub? <u/>

  - Git is not the same as GitHub.
  - GitHub makes tools that use Git.
  - GitHub is the largest host of source code in the world, and has been owned by Microsoft since 2018.
  - In this tutorial, we will focus on using Git with GitHub.

## Git Install 

  - Download and install Git from [git-scm.com](https://git-scm.com/). Verify the installation in your terminal :

        git --version

## Git Config & Help

  - Before committing, establish your identity and know how to find documentation.

  - Set Identity :

        git config --global user.name "Your Name"
        git config --global user.email "your.email@example.com"

  - Verify Configs :

        git config --list

## Git Help : Access help manuals directly inside your terminal.

        git help commit   # Opens complete manual page for the commit command
        git commit -h     # Displays quick, concise command line options


##  Git Get Started & New Files

### Initialize Repo : Turn an ordinary local directory into a watched Git repository.

        cd path/to/your/project
        git init

### Tracking New Files : Create a new file (e.g., index.html) or track modifications. 
  
  - Check the status :

        git status

        # Use compact short view option
        git status -s

### Git Staging & Commit

  - Git uses a unique 3-stage architecture : Working Directory (sandbox) ➔ Staging Area (loading dock) ➔ Local Repository (permanent snapshot).

#### Git Staging : Prepare files for a snapshot.

        git add index.html   # Stage a single file
        git add .            # Stage all new, modified, and deleted files

#### Git Commit : Create a permanent, labeled snapshot in history.

        git commit -m "Initial commit: Add base layout structure"
        # Shortcut option: Stage and commit tracked modifications simultaneously
        git commit -a -m "Fast-tracked layout adjustments"
