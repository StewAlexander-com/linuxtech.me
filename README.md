# [linuxtech.me](http://LinuxTech.me)

**Linuxtech.me Repo**

----
[Linux Commands](#Linux-Commands)  
[Linux Apps](#Linux-Apps)  
[Linux Toolbox](http://cb.vu/unixtoolbox.xhtml)  
[Linux Sys-Admin Tools](https://github.com/epcim/awesome-sysadmin2)  
[Linux Shell Tools](https://github.com/alebcay/awesome-shell/blob/master/README.md)  
[Facebook Blog](https://www.facebook.com/stewalexandercom)  
[CLI Tools](https://github.com/agarrharr/awesome-cli-apps)  
----

# Linux-Commands

-  **ac** : prints stats about a users connect time in hours, $ac -pd shows daily user connect time (​psacct needs to be installed and running first)  
-  **anacron** : cron job scheduler for a system that is not running 24 hours a day.  
-  **arch**: same as uname -m, prints the machine name  
-  **atop** : daily logging, like htop, may need to download  
-  **bat** : cat clone, download here  
-  **bmon** : bandwidth monitor  
-  **cat /etc/ *release** : gives you linux / debian release info  
-  **cat /proc/info** : gives you processor info  
-  **ccze** : log colorizer, useful for reading var/log/messages (ex. “$sudo tailf /varl/og/messages I ccze” or “$sudo cat /var/log/messages / ccze -m ansi |less -r”)  
-  **cd** - : sends the user to the last directory they were in before the present one  
-  **clear** : clears the screen  
-  **ctrl-a / ctrl- e** : “$ctrl-a” go to the beginning of a line, “$ctrl-e” go to the end of the line  
-  **ctrl-z** : pauses the running process, "$bg" to background, "$fg" to return it to the foreground  
-  **df- h** : space on volumes, human readable  
-  **dig** : DNS lookup utility  
-  **dmesg -H** : (H flag not available on all systems) boostrap info  
-  **du -hs** : directory sizes, human readable  
-  **eject** : eject removable media (as in an attached USB flash drive, etc)  
-  **env** : shows you some info on the shell environment  
-  **mkdir** -p : creates full path ex. "$sudo makdir -p home/Maildir/{cur,new,tmp}"  
-  **export VISUAL=nano; visudo** : sets nano as the visudo editor  
-  **find /etc -name - conf** : finds and displays all the config files under /etc  
-  **free -h** : show you available space on disks, in human readable format  
-  **grep -Pri .** : searches for text tin the directory and subdirectories and puts it on the screen, ex: "$grep -Pri ." searches current directory"  
-  **head** : lists top of file  
-  **inode** : contains all the information about any linux / Unix file, is an address to a specific disk block, IS the unix file except for the name, which is stored in the directory (together with the inode number) as a reference to the inode data. It truly is the file; the name one sees in the directory is just a reference.  
-  **inxi -Finc 0 > system_data.txt** : Provides a file that lists a large list of system hardware related details, somewhat like the Windows "C:\ systeminfo" command  
-  **kill $(pgrep mozilla)** : Kills all processes associated with Mozilla Firefox, substitute the app name for "mozilla" to kill it.  
-  **lastlog** : Shows all users that have logged in (or have the capability to login) and the dates and times of their logins, to limit this to those users who have logged in at some point use "$lastlog |grep -iv never"  
-  **ldd** : Lists the library dependencies of an executable  
-  **less** : Pager, shows any text document where you can move through the document by one line, and or page, at a time  
-  **locate** : (run"$sudo updatedb" first): fast search for files  
-  **logsave** : saves command / terminal/ ssh session output to a file on the desktop with a timestamp  
-  **lsblk** : lists all the block devices / partitions of the system  
-  **lslogins -u** : show all users with logins, “$lslogins -Lu” show last user logins  
-  **lsof** : list of open files on the system, may require downloading lsof  
-  **lvm**: logical volume manager for LUNs and disk partitions  
-  **man -f** : lists details associated with the commands must run "$sudo makewhatis" first  
-  **man -k** : searches man pages for the word or string  
-  **man ascii** : outputs an ascii table  
-  **nano**: text editor, ex “$nano mytext”, may require downloading nano  
-  **ncdu -rx /** : Scans the existing file system and orders directories by largest to smallest data size, fantastic for finding where all the free space has gone (think windirtree), may require downloading ncdu  
-  **nl**: adds line numbers to a file  
- **nmblookup -A** : get the (Windows) netbios name from an IP address  
-  **nmon / glances** : tools for displaying realtime stats on the system, may require downloading  
-  **pstree -p** : shows processes and PID in a tree format, very useful  
-  **pushd / popd** : collects directories to a stack, moves between stack items  
-  **rev** : reverses the output (as in “$sudo cat var/log/messages |rev”)  
- **rpm -qa** --last : shows files installed in descending order  
-  **rpm -qa** : list all installed apps  
-  **rpm -qa** --last |head : shows recently installed files  
-  **screen** : for creating virtual terminals (more useful if logged in remotely, such as by ssh)  
-  **script** : logs all transactions of a terminal to a file  
-  **set** : shows other shell environmental variables  
-  **ss** : socket statistics, "$ss -a |grep -E "\b([0-9]{1,3}\.){3}[0-9]{1,3}\b|[^a-z][^:]:[^:][^:][0-9]" provides only sockets that are attached to an or any IP address.  
-  **stat** : provides user /group data for the file or directory, ex. “$sudo stat myfile”  
-  **su -** : root privallages and root environment, use with caution  
-  **su** : root privallages but keeps the current user environment, good for debugging  
-  **sudo -k** : kills the sudo timer so root access isn't kept  
-  **sudo -s** : Open a shell account with root privileges, use with caution  
-  **sudo !!** : does the previous command again and puts ""sudo"" in front"  
-  **sudo cat /etc/passwd** : show list of users on the system, “$sudo cat /etc/passwd |grep -iv nologin” show all users with logins  
-  **sudo yum makecache fast** : update yum fast mirror package index  
-  **tail** : lists end of file  
-  **uname -a** : gives you linux kernel information  
-  **users** : lists users on the system ("$w" and "$last" are also helpful)"  
-  **visudo** : safe secure way of editting the etc/sudoers file, locks the file, checks syntax  
- **yum check-update** : shows programs on the system that have available updates  
[… & more Linux commands here](http://www.linux-commands-examples.com/_alpha-numerical)
----

# Linux-Apps

1.  [Apache](https://httpd.apache.org) / [NGINX](https://nginx.org/en/) power the web
2.  [Docker](https://www.docker.com/), [Vagrant](https://www.vagrantup.com/), [KVM](https://www.linux-kvm.org/page/Main_Page), [VirtualBox](https://www.virtualbox.org/), & [VMware](https://www.vmware.com/) power system deployment
3.  [RedHat Enterprise Linux (RHEL)](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux), [Suse Linux Enterprise Server (SLES)](https://www.suse.com/products/server/), [CentOS](https://www.centos.org/), [Debian](https://www.debian.org/) and [Windows Server](https://www.microsoft.com/en-us/cloud-platform/windows-server) are the OS’s that power the web
4.  [Glances](https://nicolargo.github.io/glances/), [htop](http://hisham.hm/htop/), [gtop](https://github.com/aksakalli/gtop), [bmon](https://github.com/tgraf/bmon) and [inxi](https://smxi.org/docs/inxi.htm) are for monitoring system behavior
5.  [Exa](https://the.exa.website/), [ccze](http://freshmeat.sourceforge.net/projects/ccze/), [lnav](http://lnav.org/) and [cat](https://ss64.com/bash/cat.html) are for viewing stuff in the command line
6.  [Nano](https://www.nano-editor.org/), [Vim](https://www.vim.org/) and [Micro](https://micro-editor.github.io/) (see below) are for editing
7.  [Brackets](http://brackets.io/), [pycharm](https://www.jetbrains.com/pycharm/), and [spyder](https://github.com/spyder-ide/spyder/blob/master/README.md) are for python development
8.  [ELinks](http://elinks.or.cz/) is for browsing the web via the command line
9.  [Shorewall](http://shorewall.org/index.html) as a system based firewall
10.  [Webmin](http://www.webmin.com/) for controlling Linux servers via the web
11.  [Fishhell](https://fishshell.com/) as a bash replacement, see it’s command tab completion (start typing a command, or type a command + space, then tab, to see options / flags), want to learn more? [Check this out](https://rootnroll.com/d/fish-shell/)
12.  [Tilix](https://github.com/gnunn1/tilix) as terminal emulator
13.  [Grsync / rsync](http://www.opbyte.it/grsync/) for backup
14.  [Brasero](https://wiki.gnome.org/Apps/Brasero) cd/dvd burning gnome desktop utility
15.  [Nbtscan](http://www.unixwiz.net/tools/nbtscan.html)- netbios scanner
16.  [Mc](https://midnight-commander.org/) - “Midnight Comander” a command line, terminal “DOS-like” visual interface that interactively does the work of ls, mv, cp, rm, mkdir, and ftp (and their clones like exa), useful for beginners and or those who like graphics.
17.  [TLDR](https://tldr.sh/) - Useful examples to a large list of Linux / Mac and Windows commands (did you know that tldr means "to long didn't read"? Now you do ... )
18.  [Micro](https://micro-editor.github.io/) - Most Linux users know of the editors Vim, and perhaps Nano (see above); Micro is another editor with easy to learn commands (like ctrl-s for save) plus syntax highlighting ...
