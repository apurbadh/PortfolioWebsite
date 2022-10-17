---
title: "Delta OS"
date: 2021-04-03T22:53:58+05:30
draft: false
github_link: "https://github.com/gurusabarish/hugo-profile"
author: "Apurba Adhikari"
tags:
  - project
  - deltaos 

image: /images/projects/delta.png
description: ""
toc: 
---
This documentation helps you learn about Delta OS and how to run it on your PC.
## About
Delta OS is an Arch based distribution created for developers and people intrested in Arch Linux. It is created by the Delta OS team which is led by Mr. Apurba Adhikari. Due to Arch Linux having good amount of learning curve and a complex installation procedure, Delta OS tries to simplify it and brings a bit user friendly and beautiful interface giving almost same Arch experience. Delta OS comes built in with VS Code, Sublime, NodeJS and OpenJDK preinstalled for developers. In later version, our team is also planning to integrate Docker and Anaconda built-in. It also provides stunning looking XFCE4 desktop environment with LightDM display manager. Delta OS also has yay preinstalled which is a package manager for AUR(Arch User Repository) which makes installing apps really easy. Our team is also working to bring more of these to the table. Our latest plans include bring I3, AwesomeWM and KDE and also Pamac which is GUI for installing packages to the table.

## Development
Delta OS is created using archiso. It is a tool used by the famous Arch Linux to update and mange their iso file. Delta OS uses syslinux as its bootloader, but we decided to keep GRUB as its bootloader after it is installed. It also has support for EFI boot. For installation, it uses the famous Calamares Framework as an installer which is a tool which gives you GUI to ask user information, install it and run scripts.

## How to install it ?
Delta OS has very easy and straight forward installation.  I will be taking you through installation procedure here.

### Downloading the ISO
You can download the ISO from https://sourceforge.net/p/deltaos/. Or just build the code from https://sourceforge.net/p/deltaos/code

### What is the liveuser credentials? 
For the Liveuser, the credentials are 
~~~
Username : liveuser
Password : liveuser
~~~
*It is to note that the root user does not have any password*

### Making a bootable USB
There are multiple ways of making a live USB. You can create live USB from tools like Rufus or UNetbootin or create it from dd which is built-in with Linux.
UNetbootin : https://unetbootin.org/
Rufus : https://rufus.ie/en_US/

For creating live USB with DD
~~~
dd if=deltaos-0.1-x86_64.iso of=sdX bs=1M
~~~
*Note that sdX  should be replaced with your device name*

### Virtually running it
I will be going through how to run it in virtual box and Qemu as they are the most famous. It is gonna be very similar for other software as well, so you don't need to worry.

### Running it on Virtual Box
#### Create a new virtual machine
![](https://imgur.com/BcNhCm6.png)

#### Fill in all the information
![](https://imgur.com/vc8Tb3Q.png)

#### Go to settings 
![](https://imgur.com/CDLn9Io.png)

####  Add Delta OS ISO to the machine from the storage section
<img src="https://imgur.com/Utui6wj.png" width="780" height="520"/>

#### Run the virtual machine
<img src="https://imgur.com/EivNlwT.png" width="780" height="520"/>

### Running on Qemu
Running on qemu is really easy. You just need to run the following command.
~~~
qemu-system-x86_64 -boot d -cdrom deltaos-0.1-x86_64.iso -m 512
~~~

