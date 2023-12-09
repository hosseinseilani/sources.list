# The complete Linux distro sources.list

In Linux, the sources.list file is a configuration file that software repositories use for package installation and updates. It is commonly found in the /etc/apt/ directory.The sources.list file contains a list of URLs or repository addresses where the package manager can find software packages. These repositories may be maintained by the Linux distribution itself or by third-party individuals or organizations.

By editing the sources.list file, you can add, remove, or modify repository entries to control which software packages are available for installation on your Linux system. It is important to be cautious when modifying this file, as incorrect changes can lead to issues with package management.The package resource list is used to locate archives of the package distribution system in use on the system. This control file is located in /etc/apt/sources.list and additionally any files ending with ".list" in /etc/apt/sources.list.d are included. The source list is designed to support any number of active sources and a variety of source media. The file lists one source per line, with the most preferred source listed first. The format of each line is: type uri args. The first item, type, determines the format for args. uri is a Universal Resource Identifier (URI), which is a superset of the more specific and well-known Universal Resource Locator, or URL. The rest of the line can be marked as a comment by using a #.
In Linux, the sources.list file is a configuration file that software repositories use for package installation and updates. It is commonly found in the /etc/apt/ directory.

The sources.list file contains a list of URLs or repository addresses where the package manager can find software packages. These repositories may be maintained by the Linux distribution itself or by third-party individuals or organizations.By editing the sources.list file, you can add, remove, or modify repository entries to control which software packages are available for installation on your Linux system. It is important to be cautious when modifying this file, as incorrect changes can lead to issues with package management. The package resource list is used to locate archives of the package distribution system in use on the system. This control file is located in /etc/apt/sources.list and additionally any files ending with ".list" in /etc/apt/sources.list.d are included. The source list is designed to support any number of active sources and a variety of source media. The file lists one source per line, with the most preferred source listed first. The format of each line is: type uri args. The first item, type, determines the format for args. uri is a Universal Resource Identifier (URI), which is a superset of the more specific and well-known Universal Resource Locator, or URL. The rest of the line can be marked as a comment by using a #.


## Badges
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)


# To edit the sources.list file in Linux, you can follow these steps:
## Modifying sources.list with nano:
1. Open a terminal window on your Linux system.
2. Type the following command to open the sources.list file in a text editor with root privileges:
sudo nano /etc/apt/sources.list

3. This command will open the sources.list file in the nano text editor with root privileges, allowing you to make changes to the file.
4. Use the arrow keys to navigate to the line you want to edit or add a new line to the file.
5. Make the necessary changes to the file using the text editor.
6. Press Ctrl+O to save the changes to the file.
7. Press Ctrl+X to exit the text editor.

## Modyfiying sources.list with vim.
To edit the sources.list file with vim, you can follow these steps:
1. Open the terminal on your Linux system.
2. Type the following command to open the sources.list file in vim: 
sudo vim /etc/apt/sources.list
This will open the sources.list file with root privileges, which is necessary to make changes to the file.
3. Use the arrow keys to move the cursor to the line you want to edit.
4. Press the `i` key to enter insert mode, which allows you to make changes to the file.
5. Make the necessary changes to the file, using the vim editor.
6. Press the `Esc` key to exit insert mode.
7. Type `:wq` and press `Enter` to save the changes and exit vim.

That's it! Your changes should now be saved to the sources.list file.

## Modyfiying sources.list with geany editor.
To edit the sources.list file with Geany, you can follow these steps:
1. Install geany from default package manager:
2. Ubuntu or Debian-based distributions:

```bash
sudo apt-get install geany
```
4. Fedora:

```bash
sudo dnf install geany
```
6. CentOS or RHEL:

```bash
sudo yum install geany
```

7. Arch Linux:
```bash
sudo pacman -S geany
```
Then run sudo geany

6. Open Geany text editor on your Linux system.
7. In Geany, click on "File" in the menu bar and select "Open".
8. Navigate to the /etc/apt/ directory where the sources.list file is located.
9. Select the sources.list file and click "Open".
10. The file will open in Geany, and you can make any necessary changes to the repository URLs.
11. Once you have made your changes, click on "File" in the menu bar and select "Save" to save the modified file.
12. Please note that editing the sources.list file requires root privileges, so you may need to use sudo or switch to the root user before making any changes. Additionally, it's a good practice to create a backup of the sources.list 13. file before making any modifications.

# Debian 
## Debian 12 (Bookworm ) -- Full sources.list

```bash
deb http://deb.debian.org/debian bookworm main non-free-firmware 
deb-src http://deb.debian.org/debian bookworm main non-free-firmware 

deb http://deb.debian.org/debian-security/ bookworm-security main non-free-firmware 
deb-src http://deb.debian.org/debian-security/ bookworm-security main non-free-firmware 

deb http://deb.debian.org/debian bookworm-updates main non-free-firmware
deb-src http://deb.debian.org/debian bookworm-updates main non-free-firmware
```

# debian 12 contrib

```bash
deb http://deb.debian.org/debian/ bookworm contrib main non-free non-free-firmware
deb-src http://deb.debian.org/debian/ bookworm contrib main non-free non-free-firmware

deb http://deb.debian.org/debian/ bookworm-updates contrib main non-free non-free-firmware
deb-src http://deb.debian.org/debian/ bookworm-updates contrib main non-free non-free-firmware

deb http://deb.debian.org/debian/ bookworm-proposed-updates contrib main non-free non-free-firmware
deb-src http://deb.debian.org/debian/ bookworm-proposed-updates contrib main non-free non-free-firmware

deb http://deb.debian.org/debian/ bookworm-backports contrib main non-free non-free-firmware
deb-src http://deb.debian.org/debian/ bookworm-backports contrib main non-free non-free-firmware

deb http://deb.debian.org/debian-security/ bookworm-security contrib main non-free non-free-firmware
deb-src http://deb.debian.org/debian-security/ bookworm-security contrib main non-free non-free-firmware
```

## Debian 11 main stable
```bash
deb http://deb.debian.org/debian bullseye main
deb-src http://deb.debian.org/debian bullseye main
deb http://deb.debian.org/debian-security/ bullseye-security main
deb-src http://deb.debian.org/debian-security/ bullseye-security main
deb http://deb.debian.org/debian bullseye-updates main
deb-src http://deb.debian.org/debian bullseye-updates main
```

## debian 11 contrib non-free
```bash
deb http://deb.debian.org/debian bullseye main contrib non-free
deb-src http://deb.debian.org/debian bullseye main contrib non-free

deb http://deb.debian.org/debian bullseye-updates main contrib non-free
deb-src http://deb.debian.org/debian bullseye-updates main contrib non-free

deb http://deb.debian.org/debian bullseye-backports main contrib non-free
deb-src http://deb.debian.org/debian bullseye-backports main contrib non-free

deb http://security.debian.org/debian-security/ bullseye-security main contrib non-free
deb-src http://security.debian.org/debian-security/ bullseye-security main contrib non-free
```

## debian10
```bash
deb http://deb.debian.org/debian buster main contrib non-free
deb-src http://deb.debian.org/debian buster main contrib non-free

deb http://deb.debian.org/debian buster-updates main contrib non-free
deb-src http://deb.debian.org/debian buster-updates main contrib non-free

deb http://deb.debian.org/debian buster-backports main contrib non-free
deb-src http://deb.debian.org/debian buster-backports main contrib non-free

deb http://security.debian.org/debian-security/ buster/updates main contrib non-free
deb-src http://security.debian.org/debian-security/ buster/updates main contrib non-free
```

## Debian main without a codename
```bash
deb http://deb.debian.org/debian/ stable main non-free non-free-firmware contrib
deb-src http://deb.debian.org/debian/ stable main non-free non-free-firmware contrib

deb http://deb.debian.org/debian/ testing main non-free non-free-firmware contrib
deb-src http://deb.debian.org/debian/ testing main non-free non-free-firmware contrib

deb http://deb.debian.org/debian-security stable-security main contrib non-free non-free-firmware
deb-src http://deb.debian.org/debian-security stable-security main contrib non-free non-free-firmware
```bash

## Debian Sid (Unstable)
```bash
deb http://ftp.us.debian.org/debian/ sid main contrib non-free
deb-src http://ftp.us.debian.org/debian/ sid main

deb http://ftp.us.debian.org/debian/ testing main contrib non-free
deb-src http://ftp.us.debian.org/debian/ testing main
```

# Ubuntu 
## Ubuntu 24.04 LTS
```bash
deb http://archive.ubuntu.com/ubuntu/ noble main restricted
deb http://archive.ubuntu.com/ubuntu/ noble-updates main restricted

deb http://archive.ubuntu.com/ubuntu/ noble universe
deb-src http://archive.ubuntu.com/ubuntu/ noble universe
deb http://archive.ubuntu.com/ubuntu/ noble-updates universe
deb-src http://archive.ubuntu.com/ubuntu/ noble-updates universe

deb http://archive.ubuntu.com/ubuntu/ noble-backports main restricted universe multiverse
deb-src http://archive.ubuntu.com/ubuntu/ noble-backports main restricted universe multiverse

deb http://security.ubuntu.com/ubuntu/ noble-security main restricted
deb http://security.ubuntu.com/ubuntu/ noble-security universe
deb-src http://security.ubuntu.com/ubuntu/ noble-security universe
deb http://security.ubuntu.com/ubuntu/ noble-security multiverse
deb-src http://security.ubuntu.com/ubuntu/ noble-security multiverse
```

## ubuntu 22.04 LTS
```bash
deb http://archive.ubuntu.com/ubuntu/ jammy main restricted universe multiverse
deb-src http://archive.ubuntu.com/ubuntu/ jammy main restricted universe multiverse

deb http://archive.ubuntu.com/ubuntu/ jammy-updates main restricted universe multiverse
deb-src http://archive.ubuntu.com/ubuntu/ jammy-updates main restricted universe multiverse

deb http://archive.ubuntu.com/ubuntu/ jammy-security main restricted universe multiverse
deb-src http://archive.ubuntu.com/ubuntu/ jammy-security main restricted universe multiverse

deb http://archive.ubuntu.com/ubuntu/ jammy-backports main restricted universe multiverse
deb-src http://archive.ubuntu.com/ubuntu/ jammy-backports main restricted universe multiverse

deb http://archive.canonical.com/ubuntu jammy partner
deb-src http://archive.canonical.com/ubuntu jammy partner
```

## Ubuntu 20.04 LTS
```bash
deb http://ports.ubuntu.com/ubuntu-ports focal main restricted universe multiverse
deb-src http://ports.ubuntu.com/ubuntu-ports focal main restricted universe multiverse

deb http://ports.ubuntu.com/ubuntu-ports focal-updates main restricted universe multiverse
deb-src http://ports.ubuntu.com/ubuntu-ports focal-updates main restricted universe multiverse

deb http://ports.ubuntu.com/ubuntu-ports focal-backports main restricted universe multiverse
deb-src http://ports.ubuntu.com/ubuntu-ports focal-backports main restricted universe multiverse

deb http://ports.ubuntu.com/ubuntu-ports focal-security main restricted universe multiverse
deb-src http://ports.ubuntu.com/ubuntu-ports focal-security main restricted universe multiverse

deb http://archive.canonical.com/ubuntu focal partner
deb-src http://archive.canonical.com/ubuntu focal partner
```

## Ubuntu 18.04 LTS
```bash
deb http://us.archive.ubuntu.com/ubuntu/ bionic main restricted
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic main restricted

deb http://us.archive.ubuntu.com/ubuntu/ bionic-updates main restricted
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic-updates main restricted

deb http://us.archive.ubuntu.com/ubuntu/ bionic universe
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic universe

deb http://us.archive.ubuntu.com/ubuntu/ bionic-updates universe
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic-updates universe

deb http://us.archive.ubuntu.com/ubuntu/ bionic multiverse
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic multiverse

deb http://us.archive.ubuntu.com/ubuntu/ bionic-updates multiverse
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic-updates multiverse

deb http://us.archive.ubuntu.com/ubuntu/ bionic-backports main restricted universe multiverse
deb-src http://us.archive.ubuntu.com/ubuntu/ bionic-backports main restricted universe multiverse

deb http://archive.canonical.com/ubuntu bionic partner
deb-src http://archive.canonical.com/ubuntu bionic partner

deb http://security.ubuntu.com/ubuntu bionic-security main restricted
deb-src http://security.ubuntu.com/ubuntu bionic-security main restricted

deb http://security.ubuntu.com/ubuntu bionic-security universe
deb-src http://security.ubuntu.com/ubuntu bionic-security universe

deb http://security.ubuntu.com/ubuntu bionic-security multiverse
deb-src http://security.ubuntu.com/ubuntu bionic-security multiverse
```

# kali
## kali-rolling branch 
```bash
deb http://http.kali.org/kali kali-rolling main contrib non-free non-free-firmware
```
## kali-last-snapshot branch 
```bash
deb http://http.kali.org/kali kali-last-snapshot main contrib non-free non-free-firmware
```

## kali-experimental branch 
```bash
deb http://http.kali.org/kali kali-experimental main contrib non-free non-free-firmware
```

## kali-bleeding-edge branch
```bash
deb http://http.kali.org/kali kali-bleeding-edge main contrib non-free non-free-firmware
```

# parrot Linux
```bash
deb http://deb.parrotsec.org/parrot stable main contrib non-free
deb-src http://deb.parrotsec.org/parrot stable main contrib non-free
```
# or
```bash
deb https://deb.parrot.sh/parrot/ parrot main contrib non-free
deb-src https://deb.parrot.sh/parrot/ parrot main contrib non-free
deb https://deb.parrot.sh/parrot/ parrot-security main contrib non-free
deb-src https://deb.parrot.sh/parrot/ parrot-security main contrib non-free
deb https://deb.parrot.sh/parrot parrot-backports main contrib non-free
deb-src https://deb.parrot.sh/parrot parrot-backports main contrib non-free
```

# PureOS 
## PureOS byzantium codename
```bash
deb https://repo.pureos.net/pureos byzantium main
deb https://repo.pureos.net/pureos byzantium-updates main
deb https://repo.pureos.net/pureos byzantium-security main
```
## PureOS amber codename
```bash
deb https://repo.pureos.net/pureos amber main
deb https://repo.pureos.net/pureos amber-updates main
deb https://repo.pureos.net/pureos amber-security main
```
## PureOS crimson codename
```bash
deb https://repo.pureos.net/pureos crimson main
deb https://repo.pureos.net/pureos crimson-updates main
deb https://repo.pureos.net/pureos crimson-security main
```

## Authors
- [@hossein seilani](https://www.seilany.ir)
