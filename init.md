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

[Official Link](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

1. Generate a key for SSH

``` shell
ssh-keygen -t ed25519 -C "your_email@example.com"
Edit ~/.ssh/config
```

2. Edit ~/.ssh/config

``` shell
Host *
      AddKeysToAgent yes
      UseKeychain yes
      IdentityFile ~/.ssh/id_ed25519
```

3. Add ssh key to ssh agent

``` shell
ssh-add -K ~/.ssh/id_ed25519
```

4. Add pub to git

## Node
