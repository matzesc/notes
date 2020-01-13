# [VirtualBox](https://www.virtualbox.org/) related notes

- Back to [Personal Notes](README.md)

## VirtualBox Host

Windows 10 Host

## [Debian](https://www.debian.org/) / [Ubuntu](https://ubuntu.com/) based distros

- [Ubuntu](https://ubuntu.com/)
- [Linux Mint](https://linuxmint.com/)

### VirtualBox Guest Additions for Ubuntu

[How to install Guest Additions for Ubuntu guest](https://askubuntu.com/questions/22743/how-do-i-install-guest-additions-in-a-virtualbox-vm)

Install VirtualBox Guest Additions packages

    sudo apt install build-essential linux-headers dkms
    sudo apt install virtualbox-guest-utils virtualbox-guest-x11 virtualbox-guest-dkms

### Using Shared Folder with Ubuntu guest

- [VirtualBox/SharedFolders](https://help.ubuntu.com/community/VirtualBox/SharedFolders)
- [Access to shared folders in Virtual Box](https://askubuntu.com/questions/161759/how-to-access-a-shared-folder-in-virtualbox#161883)

add Ubuntu user to "vboxsf" group:

    sudo usermod -aG vboxsf <username>

Reboot to make sure the user rights are updated system wide.

Manually mount a shared folder with the name "Shared":

    sudo mount -t vboxsf Shared /media/vboxshared

### Disable Automatic Updates

- [How To Stop Installing Updates Automatically On Ubuntu Or Debian (Unattended Upgrades)](https://www.linuxuprising.com/2019/07/how-to-stop-installing-updates.html)
- [How to Enable/Disable Unattended Upgrades in Ubuntu 16.04](https://linoxide.com/ubuntu-how-to/enable-disable-unattended-upgrades-ubuntu-16-04/)

disable automatic updates:

    sudo dpkg-reconfigure unattended-upgrades

### Disable Boot Splash Screen and Show Boot Text

- [Ask Ubuntu - How do I disable the boot splash screen, and only show kernel and boot text instead?](https://askubuntu.com/questions/33416/how-do-i-disable-the-boot-splash-screen-and-only-show-kernel-and-boot-text-inst)
- [Disable Purple Splash Screen on Boot in Ubuntu 18.04 / Higher](http://ubuntuhandbook.org/index.php/2019/06/disable-purple-splash-screen-boot-ubuntu-18-04-higher/)

edit grub configuration

    sudo vim /etc/default/grub

find line with `GRUB_CMDLINE_LINUX_DEFAULT="quiet splash"` and remove `quite`
and `splash`. Update Grub with

    sudo update-grub

### Enable Grub Menu and Change Log Level

- [Ask Ubuntu - How to get to the GRUB menu at boot-time?](https://askubuntu.com/questions/16042/how-to-get-to-the-grub-menu-at-boot-time)
- [CentOS / RHEL 7 : How to change the verbosity of debug logs during booting](https://www.thegeekdiary.com/centos-rhel-7-how-to-change-the-verbosity-of-debug-logs-during-booting/)
- [Introduction to the Linux kernel log levels](https://linuxconfig.org/introduction-to-the-linux-kernel-log-levels)

## [Arch](https://www.archlinux.org/) based distros

- [Arch Linux](https://www.archlinux.org/)
- [Manjaro](https://manjaro.org/)
- [Arco Linux](https://arcolinux.com/)

### VirtualBox Guest Additions for Arch

Set "Display"->"Graphics Controller" to "VBoxSVGA" for proper multi display and
automatic resizing support.

Install [VirtualBox Guest Additions](https://wiki.archlinux.org/index.php/VirtualBox#Installation_steps_for_Arch_Linux_guests) packages:

    sudo pacman -S virtualbox-guest-utils xf86-video-vmware

## Grub Display Resolution

Find a supported resolution with `vbeinfo` command in GRUB.

Modify `/etc/default/grub`, e.g.:

    # The resolution used on graphical terminal
    # note that you can use only modes which your graphic card supports via VBE
    # you can see them in real GRUB with the command `vbeinfo'
    GRUB_GFXMODE=1600x1200x32,1280x1024x32,auto
    
    # Uncomment to allow the kernel use the same resolution used by grub
    GRUB_GFXPAYLOAD_LINUX=keep

update GRUB with

    sudo grub-mkconfig -o /boot/grub/grub.cfg

and  reboot

## LightDM Display Resolution

Find a supported resolution with

    xrandr -q

Modify `/etc/lightdm/lightdm.conf` and find `display-setup-script` location,
e.g.:

    display-setup-script=xrandr --output Virtual1 --mode 1920x1200

and reboot
