# GIT related notes

- [Main Page](README.md)

# Configure Git

- [Setting Up Git](https://githowto.com/setup)
- [Git core.safecrlf different behavior on files with same line endings](https://stackoverflow.com/questions/19978063/git-core-safecrlf-different-behavior-on-files-with-same-line-endings)

Configure your name and email:

    git config --global user.name "Your Name"
    git config --global user.email "your_email@whatever.com"

## File Line Ending handling

### Linux Line Ending configuration

    git config --global core.autocrlf input
    git config --global core.safecrlf true

### Windows Line Ending configuration

    git config --global core.autocrlf true
    git config --global core.safecrlf true

## Using different Emails for Repos

Add local configuration to the repo that uses a different email after cloning or creating it:

    git config --local user.email "different@email.com"
