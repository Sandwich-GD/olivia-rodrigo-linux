# Olivia Rodrigo Linux

## Why?
Why i made this distro, is because hannah montana linux just got remade for newer systems (shoutout noah cagle).

Apart from that, i already tried everything in linux, from ricing multiple distros (manjaro, fedora, cachyos, linux mint, ubuntu, etc.), to LFS, to stupid scripts, to hardening, i got REALLY REALLY bored.

So, i got inspired from noah cagle remaking/updating hannah montana linux from the really really old version to the new 26.0 version, and i decided, i wanted to remake justin bieber linux.

Soon, i found out justin bieber linux was based on puppy linux, which i havent even used in my entire life, and also, even though there was a debian build, i dont think they made a puppy linux based template i could use, to remake justin bieber linux.

And also, even if there is a puppy linux template, i dont think i would be able to rice the desktop environment.

## How?

I used [archiso](https://github.com/archlinux/archiso), with the releng template. I did use opencode to help in some ways, like [dconf](https://github.com/GNOME/dconf), and setting up [qemu](www.qemu.org).

## Installing
With a virtual machine:

1. Install virtualbox or qemu, if you dont know how to install qemu, heres a guide: https://www.qemu.org/download/#windows
2. Get the ISO file from the releases tab
3. Set up your virtual machine
4. Start it!

With a USB

1. Get a flashing tool like rufus, or balenaetcher. Also check out ventoy, since you can flash it once, and keep throwing isos onto it, and boot whichever one you want, in a menu.
2. Reboot and repeatedly press F12
3. Set your usb as the main boot device
4. Save changes
5. Done!

## Tools 

[dconf](github.com/GNOME/dconf) is an excellent tool if you have a (specifically) gnome rice in a live iso, and you want to export it. One thing is, that i set up a shared library between qemu and my host, so i could effectively copy the dconf dump into a folder on my host.

[qemu](www.qemu.org) is also an excellent tool, for lightweight virtual machines. 

It uses the qcow2 disk format, and it supports many architectures, e. g. riscv, 32-bit, 64-bit, arm, aarch64, ppc(64), etc., and also, it comes in handy, if you dont want to set up a whole virtual machine in virtualbox, and want to quickly test iso files. 

It also comes in handy if you want to run an iso without the bloat of virtualbox.
