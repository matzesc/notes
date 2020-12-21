# Emacs

## [GNU Emacs](https://www.gnu.org/software/emacs/)

- [Using Emacs as a Server](https://www.gnu.org/software/emacs/manual/html_node/emacs/Emacs-Server.html)
- [How to Start Emacs on MS-Windows](https://www.gnu.org/software/emacs/manual/html_node/emacs/Windows-Startup.html)

### [Emacs Wiki](https://www.emacswiki.org)

- [Emacs Client](https://www.emacswiki.org/emacs/EmacsClient)
- [Ms Windows Installation](https://www.emacswiki.org/emacs/MsWindowsInstallation)

### Info & Tutorials

- [Xah Emacs Site](http://ergoemacs.org/)
- [Mastering Emacs - Articles](https://www.masteringemacs.org/all-articles)
- [Sacha Chua Emacs Blog](https://sachachua.com/blog/)
- [Using Emacs Series](https://cestlaz.github.io/stories/emacs/)

## [Org Mode](https://orgmode.org/)

- [Handling Links](https://orgmode.org/manual/Handling-Links.html)

Capture URL links from browser with `org-cliplink` or `SPC m l c` in Doom Emacs.

### [Org-Roam](https://www.orgroam.com/)

- [Org-roam User Manual](https://www.orgroam.com/manual/)
- [Github - org-roam](https://github.com/org-roam/org-roam)

## Doom Emacs & Org-Roam on Windows 10

- [Doom, Emacs & Windows](https://earvingad.github.io/posts/doom_emacs_windows/)

Install [GNU Emacs for Windows](https://www.gnu.org/software/emacs/download.html#windows) to a location of your choice.

Install the following packages for Doom-Emacs support:

```
choco install git
choco install ripgrep
choco install fd
```

for org-roam support add these additional packages:

```
choco install sqlite
choco install graphviz
```

Set `HOME` environment variable to your Windows user directory.
Open GIT bash, set path and alias for emacs in your `~/.bashrc`.

```
# path
export PATH=$PATH:<emacspath>/bin/
# alias
alias emacs='<emacspath>/bin/emacsclientw.exe --alternate-editor="<emacspath_win>\bin\runemacs.exe" -c'
alias emacsd='<emacspath>/bin/emacs.exe --daemon'
```

Clone Doom Emacs to `.emacs.d`.

`git clone https://github.com/hlissner/doom-emacs ~/.emacs.d'`

Initialize Doom Emacs from GIT bash.

`~/.emacs.d/bin/doom init`

### Create a Windows Shortcut

Set Target to:

`<emacspath_win>\bin\emacsclientw.exe --alternate-editor="<emacspath_win>\bin\runemacs.exe" -c`

## Emacs Package Archives

- [MELPA](https://melpa.org)
- [GNU ELPA](http://elpa.gnu.org/)
- [The Emacsmirror](https://emacsmirror.net/)

## Emacs Lisp

- [The Emacs Package Developer’s Handbook](https://github.com/alphapapa/emacs-package-dev-handbook)
- [The Emacs Lisp Style Guide](https://github.com/bbatsov/emacs-lisp-style-guide)

### Youtube videos

- [Youtube - An Introduction to Emacs Lisp](https://www.youtube.com/watch?v=2z-YBsd5snY)
- [Youtube - Writing A Spotify Client in 16 Minutes](https://www.youtube.com/watch?v=XjKtkEMUYGc)
- [Youtube - Writing Games with Emacs](https://www.youtube.com/watch?v=gk39mp8Vy4M)
- [Youtube - Xah Lee Live Stream. emacs lisp for beginner.](https://www.youtube.com/watch?v=1HspB643qdw)

## Emacs & GPG

- [Keeping Secrets in Emacs with GnuPG and Auth Sources](https://www.masteringemacs.org/article/keeping-secrets-in-emacs-gnupg-auth-sources)
- [Setting up GPG for Emacs](https://lars.ingebrigtsen.no/2019/08/26/setting-up-gpg-for-emacs/)
