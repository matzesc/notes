# Linux related notes

- Back to [Personal Notes](README.md)

## Bash Shell

search for `word` occurrence in specific file type (e.g. `*.md`):

    grep -inH --color "word" `find . -name "*.md" -print`

See [ripgrep](https://github.com/BurntSushi/ripgrep) as an alternative to `grep .. | find ..`

bash extensions:

- [bash-completion](https://github.com/scop/bash-completion)

## ZSH Shell

- [Oh My ZSH](https://ohmyz.sh/)
- [Github - Oh My ZSH](https://github.com/robbyrussell/oh-my-zsh)
- [Powerlevel9k - theme for ZSH](https://github.com/Powerlevel9k/powerlevel9k)
- [Powerlevel10k](https://github.com/romkatv/powerlevel10k)
- [zsh-syntax-highlight](https://github.com/zsh-users/zsh-syntax-highlighting)

## Shell Scripting

- [Advanced Bash-Scripting Guide](http://tldp.org/LDP/abs/html/)
- [Bash scripting cheatsheet](https://devhints.io/bash)
- [Conditions in bash scripting](https://linuxacademy.com/blog/linux/conditions-in-bash-scripting-if-statements/)
- [BASH Frequently Asked Questions](http://mywiki.wooledge.org/BashFAQ)
- [pushd, popd vs cd, cd- in bash and zsh](https://unix.stackexchange.com/questions/272965/pushd-popd-vs-cd-cd-in-bash-and-zsh)
- [Bash Shell – Test if File or Directory Exists](https://tecadmin.net/bash-shell-test-if-file-or-directory-exists/)

## Command Line Tools

- [An Illustrated Guide to Some Useful Command Line Tools](https://www.wezm.net/technical/2019/10/useful-command-line-tools/)
- [Linux man pages](https://linux.die.net/man/)
- [Man Pages](https://www.mankier.com/)
- [5 Command Line Tools to Break Your Dependence on the GUI](https://www.putorius.net/5-cool-command-line-tools.html)

### Highlight Matches

- [Colorized grep — viewing the entire file with highlighted matches](https://stackoverflow.com/questions/981601/colorized-grep-viewing-the-entire-file-with-highlighted-matches)
- [Highlight text similar to grep, but don't filter out text](https://stackoverflow.com/questions/7393906/highlight-text-similar-to-grep-but-dont-filter-out-text)

This highlights `pattern1` and `pattern2` in file `file_name`:

    grep --color -E '^|pattern1|pattern2' file_name

## Regular Expression

- [Wikipedia - Regular expression](https://en.wikipedia.org/wiki/Regular_expression)
- [Regular-Expression.info](https://www.regular-expressions.info/)
  - [Regular Expressions Tutorial](https://www.regular-expressions.info/tutorial.html)
- [Online regex tester and debugger](https://regex101.com/)
- [.NET - Regular Expression Options](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-options)
- [ECMAScript / Javascript Regular Expressions Tutorial](http://wikiict.org/spring/spring-cloud-tutorials/ecmascript-javascript-regular-expressions-tutorial/)

## Default Directories for Dotfiles

- [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
- [Arch Linux Wiki XDG Base Directory](https://wiki.archlinux.org/index.php/XDG_Base_Directory)

How to save your personal dotfiles:

- [The best way to store your dotfiles: A bare Git repository](https://www.atlassian.com/git/tutorials/dotfiles)
- [Youtube - Git Bare Repository - A Better Way To Manage Dotfiles](https://www.youtube.com/watch?v=tBoLDpTWVOM)

## Keyboard Shortcuts

- [Xfce keyboard shortcuts](https://defkey.com/xfce-shortcuts)
- [Termite Terminal shortcuts](https://github.com/thestinger/termite)

## Xfce Desktop

- disable [Display Power Management / Black Screen](https://askubuntu.com/questions/932931/how-do-i-disable-xfce-display-power-management-in-xubuntu-16-04-at-the-command-l)

use this command to disable Display Power Management:

    xfce4-power-manager -q

## Fonts

- [Powerline fonts](https://github.com/powerline/fonts)
- [Nerd Fonts](https://www.nerdfonts.com/)
