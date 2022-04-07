#### NimvalArch

###System Discription
This is completely automated arch install. It includes prompts to select your desired desktop environment, window manager, AUR helper, and whether to do a full or minimal install. The KDE desktop environment on arch includes all the packages I use on a daily basis, as well as some customizations.

## Troubleshooting

__[Arch Linux Installation Guide](https://github.com/rickellis/Arch-Linux-Install-Guide)__
__[Arch Linux RickEllis Installation Guide](https://github.com/rickellis/Arch-Linux-Install-Guide)__

__[Arch Linux Wiki Installation Guide](https://wiki.archlinux.org/title/Installation_guide)__

The main script will generate .log files for every script that is run as part of the installation process. These log files contain the terminal output so you can review any warnings or errors that occurred during installation and aid in troubleshooting. 

### No Wifi

You can check if the WiFi is blocked by running `rfkill list`.
@@ -47,6 +50,14 @@ After unblocking the WiFi, you can connect to it. Go through these 5 steps:

#5: Find your network, and run `station [device name] connect [network name]`, enter your password and run `exit`. You can test if you have internet connection by running `ping google.com`, and then Press Ctrl and C to stop the ping test.

## Reporting Issues

An issue is easier to resolve if it contains a few important pieces of information.
1. Chosen configuration from /configs/setup.conf (DONT INCLUDE PASSWORDS)
1. Errors seen in .log files
1. What commit/branch you used
1. Where you were installing (VMWare, Virtualbox, Virt-Manager, Baremetal, etc)
    1. If a VM, what was the configuration used.

## Credits
- Modified Version of a script called ArchTitus located here https://github.com/ChrisTitusTech/ArchTitus
- Original packages script was a post install cleanup script called ArchMatic located here: https://github.com/rickellis/ArchMatic

