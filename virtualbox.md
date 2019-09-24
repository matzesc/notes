# [VirtualBox](https://www.virtualbox.org/)
Windows 10 Host

# [Debian](https://www.debian.org/) based distros
- [Ubuntu](https://ubuntu.com/)
- [Linux Mint](https://linuxmint.com/)

# [Arch](https://www.archlinux.org/) based distros
- [Manjaro](https://manjaro.org/)
- [Arco Linux](https://arcolinux.com/)


## VirtualBox Guest Additions

Set "Display"->"Graphics Controller" to "VBoxSVGA" for proper multi display and automatic resizing support.

Install [VirtualBox Guest](https://wiki.archlinux.org/index.php/VirtualBox#Installation_steps_for_Arch_Linux_guests) addition packages:

    sudo pacman -S virtualbox-guest-utils xf86-video-vmware

## Grub Display Resolution

Find a supported resolution with `vbeinfo` command in GRUB.

Modify `/etc/default/grub`, e.g.:

```
# The resolution used on graphical terminal
# note that you can use only modes which your graphic card supports via VBE
# you can see them in real GRUB with the command `vbeinfo'
GRUB_GFXMODE=1600x1200x32,1280x1024x32,auto

# Uncomment to allow the kernel use the same resolution used by grub
GRUB_GFXPAYLOAD_LINUX=keep
```

update GRUB with

    sudo grub-mkconfig -o /boot/grub/grub.cfg

and  reboot

## LightDM Display Resolution

Find a supported resolution with

    xrandr -q

Modify `/etc/lightdm/lightdm.conf` and find `display-setup-script` location, e.g.:

    display-setup-script=xrandr --output Virtual1 --mode 1920x1200

and reboot