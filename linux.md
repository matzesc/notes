# Linux related notes

- [Main Page](README.md)
- [VirtualBox](virtualbox.md) related notes
- [Python programming](python.md) related notes

## Bash Command Line

search for word occurrence in specific files:

    grep -inH --color "word" `find . -name "*.md" -print`

## Default Directories for Dotfiles

See:
- [XDG Base Directory Specification](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html)
- [Arch Linux Wiki XDG Base Directory](https://wiki.archlinux.org/index.php/XDG_Base_Directory)

## Keyboard Shortcuts

- [Xfce keyboard shortcuts](https://defkey.com/xfce-shortcuts)
- [Termite Terminal shortcuts](https://github.com/thestinger/termite)

## Xfce Desktop

- disable [Display Power Management / Black Screen](https://askubuntu.com/questions/932931/how-do-i-disable-xfce-display-power-management-in-xubuntu-16-04-at-the-command-l)

```
    xfce4-power-manager -q
```
