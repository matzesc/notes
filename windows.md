# Windows 10

- Back to [Personal Notes](README.md)

## Customization

### [Where to Find the Windows Wallpaper Location on Your PC](https://www.techjunkie.com/windows-wallpaper-location/)

The default wallpapers are stored here:

    %WINDIR%\Web\

---

### [How to Change Desktop Icon Horizontal and Vertical Spacing in Windows 10](https://www.tenforums.com/tutorials/16941-change-desktop-icon-spacing-windows-10-a.html)

Icon spacing in Windows 10 can be change at this registry entry:

    HKEY_CURRENT_USER\Control Panel\Desktop\WindowMetrics

Change the `IconSpacing` entry to modify horizontal spacing. The default value is `-1125` a setting of `-1710` increases the spacing between icons sufficiently. Changes only apply after logging out and in again.

---

### [Items unpinned from taskbar are back after restart/sign out on Windows 10](https://superuser.com/questions/1251656/items-unpinned-from-taskbar-are-back-after-restart-sign-out-on-windows-10)

Check the XML file in the user profile that restores pins on the task bar and start menu:

    %LOCALAPPDATA%\Microsoft\Windows\Shell\LayoutModification.xml

You may need to make this file `Read Only` after modifications

---

### [TortoiseGit not showing icon overlays](https://stackoverflow.com/questions/25156238/tortoisegit-not-showing-icon-overlays)

Check this registry entry:

    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\ShellIconOverlayIdentifiers

At this point Windows 10 is limited to the top 15 icon overlays.

## Power Shell

- [How to Set PowerShell Script Execution Policy in Windows 10](https://www.tenforums.com/tutorials/54585-change-powershell-script-execution-policy-windows-10-a.html)
- [About Execution Policies](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)

## Office 365

Download [Language Accessory Pack for Office](https://support.office.com/en-us/article/Language-Accessory-Pack-for-Office-82ee1236-0f9a-45ee-9c72-05b026ee809f) if you want spelling and grammar proofing for more then one language. You also want to download the default language and install it again after other languages to get the default language back for some of the Office icons in the Start Menu.

## Proxy Settings

- [Web Proxy Auto-Discovery Protocol](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol)

## Windows Subsystem for Linux (WSL)

- [LxRunOffline](https://github.com/DDoSolitary/LxRunOffline)

### ArchLinux on WSL

- [ArchLinux on the Windows Subsystem for Linux](https://davidtw.co/writings/2017/archlinux-on-the-windows-subsystem-for-linux)
- [Getting Crazy with Windows Subsystem for Linux](https://www.brianketelsen.com/getting-crazy-with-windows-subsystem-for-linux/)
- [Deploy Arch Linux on Windows Subsystem for Linux “WSL”](https://medium.com/@mudrii/deploy-arch-linux-on-windows-subsystem-for-linux-wsl-a7e4cdf78c80)
- [ArchWSL](https://github.com/yuk7/ArchWSL)
