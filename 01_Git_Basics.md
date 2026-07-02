# <u> -------------------- Git Basics -------------------- <u/>

#### Prerequisites : We should install git in our windows to continue with the tutorials.

## Git Bash

  - Git Bash is a terminal for Windows that lets you use Git commands.

  - After installing Git, you can find Git Bash in your Start menu.

  - You can use Git Bash just like the Command Prompt, but with extra Unix commands (like ls and pwd).

## Configure Git

  - Now let Git know who you are. This is important for version control systems, as each Git commit uses this information:

  - You can change these settings at any time, they only affect how your name and email appear in your commits.

#### User Name

  - Your name will be attached to your commits. Set it with:

  - Example

        git config --global user.name "Your Name"

  - Note: If you make a typo or mistake, just run the command again with the correct value.

  - The new setting will overwrite the old one.

#### Email Address

  - Your email is also attached to your commits. Set it with:

  - Example

        git config --global user.email "you@example.com"

  - Change the user name and email to your own.

  - You will probably also want to use this when registering to GitHub later on.

  - Note: If you forget to set your name or email, Git will prompt you the first time you try to commit.

  - You can always change these settings later, and previous commits will keep the old info.

  - Use --global to set the value for every repository on your computer.

  - Use --local (the default) to set it only for the current repository.

## Why Configure Git?

  - Git uses your name and email to label your commits.

  - If you do not set these, Git will prompt you the first time you try to commit.

  - Now you have added the minimum of configuration needed to start using Git.

## Viewing Your Configuration

- You can see all your Git settings with:

- Example: List All Settings

        git config --list
        user.name=Your Name
        user.email=you@example.com
        core.editor=code --wait
        alias.st=status
        init.defaultbranch=main
        ...

  - To view a specific value, use:

  - Example: View a Specific Setting

        git config user.name
        Your Name

## Changing or Unsetting Config Values

  - To change a value, just run the git config command again with the new value.

  - To remove a setting, use --unset:

  - Example: Unset an Alias

        git config --global --unset code.editor

## Default Branch Name

  - Set the default branch name for new repositories (for example, main instead of master):

  - Example: Set Default Branch Name

        git config --global init.defaultBranch main

## Configuration Levels

  - There are three levels of configuration:

        System (all users): git config --system
        Global (current user): git config --global
        Local (current repo): git config --local

  - The order of precedence is:

        Local (current repo)
        Global (current user)
        System (all users)

  - The reason to use the different levels is that you can set different values for different users or repositories.

  - This can be used for example to set different default branches for different repositories and users.

  - Example: Set a Local Config

  - Local settings only apply to the current repository.

        git config user.name "Project Name"

  - Example: Set a Global Config

  - Global settings apply to all repositories for the current user.

        git config --global user.name "Global Name"

  - Example: Set a System Config

  - System settings apply to all repositories for all users.

        git config --system user.name "System Name"

## 
