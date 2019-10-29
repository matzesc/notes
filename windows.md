# Windows 10

- [Personal Notes](README.md)

## Customization

- [Where to Find the Windows Wallpaper Location on Your PC](https://www.techjunkie.com/windows-wallpaper-location/)

The default wallpapers are store here:

    %WINDIR%\Web\

- [How to Change Desktop Icon Horizontal and Vertical Spacing in Windows 10](https://www.tenforums.com/tutorials/16941-change-desktop-icon-spacing-windows-10-a.html)

Icon spacing in Windows 10 can be change in the registry:

    HKEY_CURRENT_USER\Control Panel\Desktop\WindowMetrics

Change the `IconSpacing` entry to modify horizontal spacing. The default value is `-1125` a setting of `-1710` increased the spacing between icons sufficiently. Changes only apply after logging out and in again.

- [Items unpinned from taskbar are back after restart/sign out on Windows 10](https://superuser.com/questions/1251656/items-unpinned-from-taskbar-are-back-after-restart-sign-out-on-windows-10)

There is a XML file in the user profile that restores pins on the task bar and start menu:

    %LOCALAPPDATA%\Microsoft\Windows\Shell\LayoutModification.xml

## Office 365

- [Language Accessory Pack for Office](https://support.office.com/en-us/article/Language-Accessory-Pack-for-Office-82ee1236-0f9a-45ee-9c72-05b026ee809f)

## Proxy Settings

- [Web Proxy Auto-Discovery Protocol](https://en.wikipedia.org/wiki/Web_Proxy_Auto-Discovery_Protocol)
