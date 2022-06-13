# Marvel task 3: Resource article
In this task, I will be detailing the process of installing and setting up Ubuntu on your computer.

## Downloading the Ubuntu ISO image
At the time of writing, Ubuntu 20.04 was the stable LTS release. You may download the ISO from [here.](https://releases.ubuntu.com/20.04.4/)
Ensure that you download the Desktop image.

## Creating a bootable USB stick
For this step, you will need to download a software utility called [Rufus.](https://rufus.ie/en/)

<img src="https://rufus.ie/pics/rufus_en.png" height="30%" width="30%">

Once you have downloaded it, plug in a USB flash drive of at least 8GB capacity into your computer and write the ISO file into it. The image shows version 18.04, but the procedure is the same for version 20.04 as well.

## Booting into the USB flash drive

Plug in the Bootable USB flash drive that you just wrote the ISO to, into the computer on which you want to install Ubuntu. Turn on the computer, head into the BIOS and choose the USB flash drive as the boot device. 

<img src="https://expertreviews.b-cdn.net/sites/expertreviews/files/styles/er_main_wide/public/2015/08/boot_priority_with_usb_drive.png" height="50%" width="50%">

## Installing Ubuntu 20.04
Once you have successfully booted up into the USB flashdrive, you should see the Ubuntu Welcome screen:

<img src="https://assets.ubuntu.com/v1/6855ab78-welcome-screen.png" height="50%" width="50%">

Select "Install Ubuntu", and proceed with the installation. 

### Setting Up the keyboard layout
Choose the appropriate keyboard layout from the list below. Usually, Ubuntu automatically detects it for you, so it mustn't be too much of a hassle.

<img src="https://assets.ubuntu.com/v1/47f9c406-select-keyboard-layout.png" height="50%" width="50%">

### Choosing the installation type

Choose between Normal installation or Minimal Installation. The former installs the most basic applications and utilities that the average user would need on a personal computer. The latter installs a minimal version of the operating system which is suitable for power users, who would like to have control over what applications are installed on their machine.

<img src="https://assets.ubuntu.com/v1/e2bd1af8-download-updates.png" height="50%" width="50%">

### Partitioning and allocating disk space

At this stage, you have 2 options:
1. You could erase everything and install Ubuntu. Ubuntu will set up the partition automatically.
2. You could choose to set up the partitions yourself.
#### 1. Erase Everything and install Ubuntu
You just need to click on "Erase disk and install Ubuntu". The rest of the process will be taken care of by Ubuntu.

<img src="https://assets.ubuntu.com/v1/930ca887-continue-installation.png" height="50%" width="50%">

#### 2. Allocate partitions yourself.
Here, you need to click on "Something else." and proceed.

You will see the following screen:

<img src="https://www.tecmint.com/wp-content/uploads/2018/05/Choose-Free-Space-Partition.png" height="50%" width="50%">

You have to set up the partitions on your own here.
I suggest the following partition scheme:

```
swap area: Twice the storage capacity of your RAM.
/ - Root mount point: Anywhere from 30GB to 50GB, depending on whether or not you plan on installing a lot of applications.
/home - Home mount point: The space that is remaining can be assigned to the /home partition.
```

### Miscellaneous settings

Set your location:

<img src="https://assets.ubuntu.com/v1/5f9e0960-select-location.png" height="50%" width="50%">

Set up your Login credentials:

<img src="https://assets.ubuntu.com/v1/422d18ea-login-details.png" height="50%" width="50%">

And finally, wait for your installation to complete. Make sure that you restart your computer after the installation completes. Also, remove the installation medium when Ubuntu prompts you to.

## Post-install setup

Once Ubuntu boots up, it will ask you to set up a few settings to make your experience seamless. Ensure that you set up the settings accordingly.

After that, connect to the internet, open up the terminal and type the following command:

` sudo apt update && sudo apt upgrade `

The terminal will prompt you for your password. Enter the password and proceed with the update.

In case you face any issues with the installation process, feel free to post your queries in the [forum.](https://ubuntuforums.org/)

You have now successfully installed Ubuntu. Hope you enjoy all that Linux has to offer!
