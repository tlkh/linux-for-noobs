# Linux for Noobs

## What is Linux?

Linux is an open-source operating system (OS), just like Windows or Android.

Linux takes many forms, called **distros**. Here are some common ones:

**Mainstream Use (Desktop or Server)**

* Ubuntu ([website](https://www.ubuntu.com/desktop))
* Fedora ([website](https://getfedora.org/))
* Debian ([website](https://www.debian.org/))
* Elementary OS ([website](https://elementary.io/))

**Security**

* Kali Linux ([website](https://www.kali.org/))

**Elite `1337` pr0s usage**

* Arch Linux ([website](https://www.archlinux.org/))
* Gentoo ([website](https://www.gentoo.org/))

Of all the distros, Ubuntu is [one of the most widely used](https://insights.ubuntu.com/2016/04/07/ubuntu-is-everywhere/) distros, powering web servers, computers and other devices (such as IoT devices or robots).

Ubuntu is actually an (more user-friendly?) offshoot of Debian. They share many similarities, including `apt` and the `dpkg` **package manager** (more on that later).

Fedora is the other kid on the block, also very modern and pretty. It has a good reputation for security.

**Ubuntu** and **Fedora** are actually bankrolled by commercial companies. **Canonical** makes money supporting commercial users of Ubuntu, while Fedora's development is ultimately channelled into **Red Hat**'s commercial product, **Red Hat Enterprise Linux** (RHEL), which is used when security and stablity is paramount (think medical, government or miliary).

## What package manager..?

An analogy is the App Store. It's where you go to for "packages", which may take the form of actual "apps" like Firefox that have a graphical interface (GUI), command line tools like `htop`, or libraries that another package (such as python) might depend on.

In Ubuntu and Debian, the package manager is `apt`. To install a package, eg. Firefox, execute the command `sudo apt install firefox`. 

#### omg i'm lost halp

The command is executed in the **terminal** (command line). To open Terminal, either press `CTRL``ALT``T` or find Terminal in the Applications menu. If you have already connected via **SSH** (next section), you're staring at the Terminal.

Here's the breakdown:

1. `sudo` -- admin rights
2. `apt` -- package manager
3. `install` -- the "action" (another example is `purge`, which uninstalls a package completely)
4. `firefox` -- the package in question. You can actually list more than one package, like `sudo apt install htop firefox chromium-browser` to install `htop`, Firefox and Chromium (open-source version of Google Chrome). If you can't really recall the name of the package, you can hit the `TAB` button for a list of suggestions.

## Connecting to a Linux Machine

There are two ways of connecting to a *remote* Linux machine (such as a web server, or a Raspberry Pi running on the network):

1. SSH (secure shell) - command line
2. VNC (virtual network computing) - graphical desktop interface

SSH is more commonly used and almost universally present on Linux machines. It gives you access to the command line interface (terminal).

Command from Linux or macOS: `ssh pi@10.12.147.144`:

1. `ssh` -- call SSH
2. `pi` -- the user name you want to login as
3. `10.12.147.144` -- the address of the Linux device

Execute the command and type in your password. **Note: the password will not appear as you type it in.**

On Windows, you have to use [PuTTY](http://www.putty.org/).

VNC is more user friendly but usually requires a seperate install and configuration. 


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

