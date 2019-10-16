# GIT related notes

- [Main Page](README.md)

## Configure Git

- [Setting Up Git](https://githowto.com/setup)
- [Git core.safecrlf different behavior on files with same line endings](https://stackoverflow.com/questions/19978063/git-core-safecrlf-different-behavior-on-files-with-same-line-endings)

Configure your name and email:

    git config --global user.name "Your Name"
    git config --global user.email "your.name@example.com"

### File Line Ending Behavior

#### Linux Line Ending Configuration

    git config --global core.autocrlf input
    git config --global core.safecrlf true

#### Windows Line Ending Configuration

    git config --global core.autocrlf true
    git config --global core.safecrlf true

### Using different Emails for Repositories

Add local configuration to the repo that uses a different email after cloning or creating it:

    git config --local user.email "different@email.com"

## Git Usage

### Git Documentation

- [Git Documentation](https://git-scm.com/doc)
- [git ready](http://gitready.com/)

### Git Workflows

- [An overview of recommended workflows with Git](https://git-scm.com/docs/gitworkflows)
- [Comparing Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows)

#### Git Flow Workflow

- [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
- [Gitflow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
- [GitFlow](https://www.gitflow.com/)
- [GitFlow on GitHub](https://github.com/nvie/gitflow)

### Git Usage Examples

- [99% of the Git commands you'll need at work, demonstrated in a single script](https://bitbucket.org/BitPusher16/dotfiles/raw/49a01d929dcaebcca68bbb1859b4ac1aea93b073/refs/git/git_examples.sh)

## Git fixing history issues

### Remove Large Files from a Repository

- [Permanently remove files and folders from Git repo](https://dalibornasevic.com/posts/2-permanently-remove-files-and-folders-from-a-git-repository)
- [Python script to find largest files in repository](https://gist.github.com/nk9/b150542ef72abc7974cb#file-largestfiles-py)
- [How to find/identify large commits in git history?](https://stackoverflow.com/questions/10622179/how-to-find-identify-large-commits-in-git-history)
- [Removing and purging files from git history](https://blog.ostermiller.org/git-remove-from-history)

Delete a specific file from GIT history:

    git filter-branch --index-filter 'git rm --cached --ignore-unmatch filename' HEAD

### Change Author Email Address

- [Changing author info](https://help.github.com/en/articles/changing-author-info)
