# Phase 2: Local Branching, Stashing & History

## Git Branch & Merge

  - Branches allow isolated experimentation without altering your stable production code.

  - List local branches:

        git branch

### Create a branch: 

        git branch feature-login

### Switch branches: 
  
        git switch feature-login (Alternative: git checkout feature-login)

### Create and Switch Shortcut: 

        git switch -c feature-dashboard

## Git Merge : Combine branch histories. To bring your feature changes into main, switch to the receiver first:

      git switch main
      git merge feature-login

### Branch Cleanup Options:

      git branch -d feature-login   # Safe delete (only works if fully merged)
      git branch -D feature-login   # Force delete unmerged branch

## Git Stash

  - When you need to switch tasks immediately but aren't ready to commit your messy, half-written code.

        git stash               # Save messy, uncommitted work safely to an internal clipboard
        git stash list          # See your saved stashes
        git stash pop           # Apply your saved changes back and remove them from the stash stack
        git stash apply         # Apply changes but keep them saved in the stash history
        git stash drop          # Delete a specific stash entry

## Git History & Tagging

  - Git History: Inspect the chronological timeline of your snapshots.

        git log
        git log --oneline     # Displays a highly scannable, single-line history layout

  - Git Tagging: Mark specific points in history as important, usually for software releases.

        git tag v1.0.0                          # Light weight tag on current commit
        git tag -a v1.1.0 -m "Production release v1.1"  # Annotated tag with a message
