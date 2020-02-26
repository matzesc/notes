# Windows 10

- Back to [Personal Notes](README.md)

## Customization

### [Where to Find the Windows Wallpaper Location on Your PC][Wallpaper]

The default wallpapers are stored here:

    %WINDIR%\Web\

[Wallpaper]: https://www.techjunkie.com/windows-wallpaper-location/

---

### [How to Change Desktop Icon Horizontal and Vertical Spacing in Windows 10][Icon]

Icon spacing in Windows 10 can be change at this registry entry:

    HKEY_CURRENT_USER\Control Panel\Desktop\WindowMetrics

Change the `IconSpacing` entry to modify horizontal spacing. The default value
is `-1125` a setting of `-1710` increases the spacing between icons
sufficiently. Changes only apply after logging out and in again.

[Icon]: https://www.tenforums.com/tutorials/16941-change-desktop-icon-spacing-windows-10-a.html

---

### [Items unpinned from taskbar are back after restart/sign out on Windows 10][Taskbar]

Check the XML file in the user profile that restores pins on the task bar and
start menu:

    %LOCALAPPDATA%\Microsoft\Windows\Shell\LayoutModification.xml

You may need to make this file `Read Only` after modifications

[Taskbar]: https://superuser.com/questions/1251656/items-unpinned-from-taskbar-are-back-after-restart-sign-out-on-windows-10

---

### [TortoiseGit not showing icon overlays][Overlay]

Check this registry entry:

    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\ShellIconOverlayIdentifiers

At this point Windows 10 is limited to the top 15 icon overlays.

[Overlay]: https://stackoverflow.com/questions/25156238/tortoisegit-not-showing-icon-overlays

## Power Shell

- [How to Set PowerShell Script Execution Policy in Windows 10][PS1]
- [About Execution Policies][PS2]

[PS1]: https://www.tenforums.com/tutorials/54585-change-powershell-script-execution-policy-windows-10-a.html
[PS2]: https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6

## Office 365

Download [Language Accessory Pack for Office][Lang] if you want spelling and
grammar proofing for more then one language. You also want to download the
default language and install it again after other languages to get the default
language back for some of the Office icons in the Start Menu.

[Lang]: https://support.office.com/en-us/article/Language-Accessory-Pack-for-Office-82ee1236-0f9a-45ee-9c72-05b026ee809f

### Word Issues

- [Blacked out numbering in MS Word][Word]

[Word]: https://answers.microsoft.com/en-us/office/forum/office_2016-word/blacked-out-numbering-in-ms-word-2016/d2ec88d5-fcf6-41b6-bf05-487724585f51

## Proxy Settings

- [Web Proxy Auto-Discovery Protocol](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol)

## Windows Subsystem for Linux (WSL)

- [LxRunOffline](https://github.com/DDoSolitary/LxRunOffline)

### ArchLinux on WSL

- [ArchLinux on the Windows Subsystem for Linux](https://davidtw.co/writings/2017/archlinux-on-the-windows-subsystem-for-linux)
- [Getting Crazy with Windows Subsystem for Linux](https://www.brianketelsen.com/getting-crazy-with-windows-subsystem-for-linux/)
- [Deploy Arch Linux on Windows Subsystem for Linux “WSL”](https://medium.com/@mudrii/deploy-arch-linux-on-windows-subsystem-for-linux-wsl-a7e4cdf78c80)
- [ArchWSL](https://github.com/yuk7/ArchWSL)

## Action Center

### Action Center not opening

- [How to Fix Windows 10 Action Center not Opening Problem](https://www.xtremerain.com/fix-windows-action-center-not-opening/)
- [How to Fix the Action Center Not Opening in Windows 10](https://www.maketecheasier.com/fix-action-center-not-opening-windows10/)
- [Action Center Not Working in Windows 10 [SOLVED]](https://troubleshooter.xyz/wiki/fix-action-center-not-working-in-windows-10/)

Open Power Shell in Admin mode and run:

    Get-AppXPackage -AllUsers | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}

Running just this resolved the issue on my PC:

    Add-AppxPackage -DisableDevelopmentMode -Register "C:\Windows\SystemApps\ShellExperienceHost_cw5n1h2txyewy\AppXManifest.xml"
