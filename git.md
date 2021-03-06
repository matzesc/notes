# GIT related notes

- Back to [Personal Notes](README.md)

## Configure Git

- [Setting Up Git](https://githowto.com/setup)
- [Git core.safecrlf different behavior on files with same line endings](https://stackoverflow.com/questions/19978063/git-core-safecrlf-different-behavior-on-files-with-same-line-endings)
- [git config | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-config)

Configure your name and email:

    git config --global user.name "Your Name"
    git config --global user.email "your.name@example.com"

### File Line Ending Behavior

#### Linux Line Ending Configuration

    git config --global core.autocrlf input
    git config --global core.safecrlf warn

#### Windows Line Ending Configuration

    git config --global core.autocrlf true
    git config --global core.safecrlf warn

### Using different Emails for Repositories

Add local configuration to the repo that uses a different email after cloning or creating it:

    git config --local user.email "different@email.com"

### Changing Remote's URL

- [Changing a remote's URL](https://help.github.com/en/github/using-git/changing-a-remotes-url)
- [How to change the URI (URL) for a remote Git repository?](https://stackoverflow.com/questions/2432764/how-to-change-the-uri-url-for-a-remote-git-repository)

check current URL:

    git remote -v

update to new URL

    git remote set-url origin new.git.url/here

### Fixing Configuration Problems

- [How can I remove an entry in global configuration with git config?](https://stackoverflow.com/questions/11868447/how-can-i-remove-an-entry-in-global-configuration-with-git-config)
- [Trying to commit Git files but getting :: fatal: LF would be replaced by CRLF in \<some file in repo\>](https://stackoverflow.com/questions/15467507/trying-to-commit-git-files-but-getting-fatal-lf-would-be-replaced-by-crlf-in)

## Git Usage

### Git Documentation

- [Git Documentation](https://git-scm.com/doc)
- [git ready](http://gitready.com/)
- [Git Tutorials and Training | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)

### Windows Specific Topics

- [Git on Windows switch between Windows Secure Channel and OpenSSL](https://stackoverflow.com/questions/45742607/switch-to-native-windows-secure-channel-library-from-openssl-library-on-wind)

### Git Workflows

- [An overview of recommended workflows with Git](https://git-scm.com/docs/gitworkflows)
- [Comparing Workflows](https://www.atlassian.com/git/tutorials/comparing-workflows)

#### Git Flow Workflow

- [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
- [GitFlow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)
- [GitFlow](https://www.gitflow.com/)
- [GitFlow on GitHub](https://github.com/nvie/gitflow)

### Git Usage Examples

- [99% of the Git commands you'll need at work, demonstrated in a single script](https://bitbucket.org/BitPusher16/dotfiles/raw/49a01d929dcaebcca68bbb1859b4ac1aea93b073/refs/git/git_examples.sh)

### Git Submodules/Subtree

- [Github Blog - Working with submodules](https://github.blog/2016-02-01-working-with-submodules/)
- [Git subtree: the alternative to Git submodule](https://www.atlassian.com/git/tutorials/git-subtree)
- [Git Submodules vs Git Subtrees](https://martowen.com/2016/05/01/git-submodules-vs-git-subtrees/)

### Git Worktrees

- [Git - git-worktree Documentation](https://git-scm.com/docs/git-worktree)
- [Git - Worktrees](https://devtut.github.io/git/worktrees.html#using-a-worktree)
- [Git Worktrees: Parallel Development Guide](https://tecadmin.net/git-worktrees-parallel-development-guide/)

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

## Git Web-Services

### Git Repository Hosting

- [Github](https://github.com/)
- [Gitlab](https://gitlab.com/)
- [Bitbucket](https://bitbucket.org/)

### Other Git Related Services

- [Travis CI](https://travis-ci.org/)
- [GitBook](https://www.gitbook.com/)

## Git Related Projects

- [Git Large File Storage](https://git-lfs.github.com/)
- [git-annex](https://git-annex.branchable.com/)
