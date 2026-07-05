# Phase 3: GitHub Integration & SSH Security

## GitHub Get Started & SSH Setup

  - GitHub Get Started: Sign up at GitHub.com to host your repositories securely online.

### Git What is SSH?

  -  Secure Shell (SSH) is an encrypted protocol used to securely communicate with GitHub servers without typing passwords every single time.

## GitHub Add SSH:

  - Generate a key pair: ssh-keygen -t ed25519 -C "your.email@example.com"

  - Start agent: eval "$(ssh-agent -s)" and add your private key: ssh-add ~/.ssh/id_ed25519

  - Copy your public key contents (cat ~/.ssh/id_ed25519.pub) and add it to your GitHub profile settings under SSH and GPG keys.

## GitHub Set Remote

  - Link your pre-existing offline local repository to your cloud GitHub repository.

        git remote add origin git@github.com:your-username/your-repo-name.git
        git remote -v    # Verify your remote endpoint links
