# GIT related notes

# Configure Git

- [Setting Up Git](https://githowto.com/setup)

Configure your name and email:

    git config --global user.name "Your Name"
    git config --global user.email "your_email@whatever.com"

## Linux specific

    git config --global core.autocrlf input
    git config --global core.safecrlf true

## Windows specific

    git config --global core.autocrlf true
    git config --global core.safecrlf true

## Using different emails for Repos

Configure the repo that uses a different email after cloning:

    git config --local user.email "different@email.com"





