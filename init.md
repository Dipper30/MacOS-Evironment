# Init

## Homebrew

### To install brew

    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

### Problem

If there is an error:
homebrew Warning: /opt/homebrew/bin is not in your PATH.

1. Open ~/.zshrc or ~/.bashrc (if no such file, create one)
2. Edit ~/.zshrc
    export PATH=/opt/homebrew/bin:$PATH
3. source ~/.zshrc

## Git

### Install git

    brew install git

### Set up ssh key

Generate a key for SSH
    ssh-keygen -t ed25519 -C "your_email@example.com"
Add pub to git

## Node

