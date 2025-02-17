# `Linux :`

## What is Linux?
Linux is an open-source operating system modeled on Unix and developed in the C language.

* Linux first released on **Sep 17,1991 by LINUS TORVALDS**

## Features of Linux:

* It is reliable as it runs smoothly and does not need to be rebooted repeatedly.
* Significantly reduces the monitor cost.
* Linux is open source.
* Huge Base of developers that freely provide support.
* Licensing freedom to re-use and re-publish the code.
* Can be customized if you want to change your system's look.
* New enhancements happening and updates come frequently.
* More secure than other operating systems.

### What will happen when we turn on a computer/laptop?

It is the process when the system is initialized during boot-up. 
* This process involves several stages to load the operating system.

**Stages:**
### Power-On:
When you turn on your computer, electricity is supplied to all components (e.g., CPU, memory).
### BIOS/UEFI:
* Basic Input/Output System (BIOS) or Unified Extensible Firmware Interface (UEFI) is the first program that runs.
* It performs a Power-On Self-Test (POST) to check if hardware components are working properly.
* It then looks for the boot device (e.g., SSD/HDD).
### Boot Loader (GRUB):
* Linux typically uses GRUB (Grand Unified Bootloader) as the boot loader.
* GRUB presents a menu to choose which operating system or kernel to boot (if multiple are installed).
* Once a selection is made, GRUB loads the selected kernel into memory.
### Kernel Initialization:
* The kernel is loaded into memory.
* It initializes hardware drivers, sets up memory management, and prepares the system for user space.
### Init Process:
* After the kernel is loaded, the init process is executed.
* The init process is responsible for starting and managing system services and processes.

init 0 → Shutdown

init 6 → Reboot
### User Space Initialization:
* The init process initiates the user space environment.
This includes mounting file systems, starting system daemons, and launching user login prompts.
### Login Prompt:
The user is prompted to log in by entering their username and password to access the system.


### Architecture of Linux:
Hardware
    
↓

Kernel
    
↓


Shell

**Kernel:** It is the interface between the applications and the actual process done at the hardware level.

**Shell:** It is the interface that takes user commands and sends them to the kernel.

**How Shell Works:**

Command to be executed or shell script

 → 


Linux Shell 

→ 

Converted to library language by Shell 

→ 

Sent to Linux Kernel

`Eg:`

cat 

→

bash

→

00110011

→

Linux Kernel

### Types of Shell :

* Bash
* C Shell
* Korn Shell
* tsch Shell

### What is GNU or GNU tool?

* GNU stands for GNU's Not Unix

* GNU tools are a bunch of useful programs that help you manage files, edit text , write code and control your linux system

## What is Linux Distributions:
It is an O.S having Linux Kernel and GNU tools packaged with some more applications.

* There are more than 600 distribution available based on :

    * The Development group
    * Their Specific requirement 
    * Customizaion
* They are community and commercial    
* Some of the popular Linux distributions are 

   * Ubuntu, 
   * Fedora, 
   * RedHat, 
   * Debian, 
   * CentOS, etc.
## File : 
You don't need a command to check the CPU info, but can print file  **""/proc/cpuinfo"** like a simple plain text file.

* There are some specific files that represents hardware devices, system information etc....
* The /proc file system in Linux gives detail about the kernel's run-time operation in form of plain text files.


### Types of Files in Linux:
**If the file starts with :**


_  - Normal file

d = Normal directory

l = Symbolic link (Shortcut to a file / directory)

p = Pipe (It is similar to socket, but users can not work with it directly)

S = Socket (Pass the data between two processes)

C = Processes Character between communication.


### Run Levels in Linux:

0 - Halt the system

1 - Single-user mode

2 - Multiple user mode with no network file system

3 - Multiple user mode in CLI, but no GUI

4 - User definable

5 - Multiple user mode in GUI

6 - Reboot

We can use these run levels with the init command. 

`Example:` init 0

### Pipe:

* Pipe is represented as "|" and is used to direct the output of one command to another.
* It creates an internel connection between wo or more commands
* The data is passed to other commands directly instaed of using temporary text files.
* Pipe is unidirectional, and data flows from left to right.
* Pipe along with grep is commonly used 

* ` Example:` 
           
    cat file.txt | grep Linux

## Linux Directory System :
The Linux directory system is hierarchical and starts from the root directory. 
* Below are the key directories and their purposes:

   * ### / (Root Directory) :
   This is the top-level directory and the parent of all other directories.
Represented by a forward slash (/).
   * ### /root:
   Home directory for the root user (administrator).
Provides the working environment for the root user.
   * ### /home:
Home directory for other users in Linux.
Provides a working environment for non-root users.
    * ###/bin:
Contains essential binary commands used by all users (e.g., ls, cp, mv).
    * ### /boot:
Contains the kernel, bootloader files, and boot configuration files.
Holds files necessary for booting the operating system.
/dev:
Contains device files (e.g., /dev/sda for disks, /dev/cdrom for CD-ROM).
Similar to the Device Manager in Windows.
/etc:
Contains system-level configuration files (e.g., /etc/passwd for user info, /etc/network/interfaces for network configuration).
/usr:
Default directory for installing software applications.
Contains user-installed programs and libraries.
/sbin:
Contains binary commands used only by the superuser (root).
Examples include system administration commands.
/var:
Contains data that frequently changes while the system is operational.
Includes log files, databases, and other files that change in size.
 
Linux Directory Structure /mnt This directo... by Subhan Shaik Mohammed
Subhan Shaik Mohammed
Linux Directory Structure
/mnt
This directory is used to mount a filesystem temporarily. It is empty by default.
/media
Used by the system to automatically mount removable media such as CDs, DVDs, USB drives, and Zip drives. It contains all of the removable media like CD-ROM and pendrive.
/lib
It contains library files that are used in the operating system. It is similar to DLL files in Windows. Library files in Linux are shared object files.
/proc
It contains process files. Its contents are not permanent as they keep changing. It is also called a virtual directory. It contains useful information used by the OS, such as RAM, SWAP, and CPU details.
/lib and /lib64
These directories hold libraries needed by programs, such as libc.so.6.
/opt
This filesystem holds additional software installed on the system. A sub-directory is created for each installed software. It is an optional directory for users and contains third-party software.
Root Directory Structure Diagram
root
 |
 |-- home
 |-- usr
 |   |-- bin
 |   |-- local
 |   |-- sbin
 |   |-- include
 |-- etc
 |-- root
 |-- opt
 |-- lib
 |-- boot
 |-- bin
 |-- mnt
 |-- var
 |   |-- tmp
 |   |-- log
 |   |-- cache
 |   |-- spool
 |-- media
 |-- tmp
has context menu