
<table style="width:100%;">
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<tbody>
<td><h2 id="linux-toolbox" class="wsite-content-title" style="text-align:center;"><a href="http://cb.vu/unixtoolbox.xhtml">Linux Toolbox</a></h2></td>
<td><h2 id="linux-sys-admin-tools" class="wsite-content-title" style="text-align:center;"><a href="https://github.com/epcim/awesome-sysadmin2">Linux Sys-Admin Tools</a></h2></td>
<td><h2 id="linux-shell-tools" class="wsite-content-title" style="text-align:center;"><a href="https://github.com/alebcay/awesome-shell/blob/master/README.md">Linux Shell Tools</a></h2></td>
<td><h2 id="facebook-blog" class="wsite-content-title" style="text-align:center;"><a href="https://www.facebook.com/stewalexandercom">Facebook Blog</a></h2></td>
<td><h2 id="cli-tools" class="wsite-content-title" style="text-align:center;"><a href="https://github.com/agarrharr/awesome-cli-apps">CLI Tools</a></h2></td>
</div></td>
</tr>
</tbody>
</table>

------------------------------------------------------------------------

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><div>
<div id="479135938417427821" class="wcustomhtml" data-align="center" style="width: 100%; overflow-y: hidden;">
<span id="Linux"></span>
<h2 id="linux-commands-1">Linux Commands</h2>
</div>
</div></td>
</div></td>
</tr>
</tbody>
</table>

• <strong>ac</strong> : prints stats about a users connect time in hours, $ac -pd shows daily user connect time (​<em>psacct needs to be installed and running first</em>)<br />
• <strong>anacron</strong> : cron job scheduler for a system that is not running 24 hours a day.<br />
• <strong>arch</strong> : same as uname -m, prints the machine name<br />
• <strong>atop </strong>:  daily logging, like htop, may need to download<br />
• b<strong>at </strong>:  cat clone, download <em><a href="https://github.com/sharkdp/bat">here</a></em><br />
• <strong>bmon </strong>: bandwidth monitor<br />
• <strong>cat /etc/*release </strong>: gives you linux / debian release info<br />
• <strong>cat /proc/info </strong>: gives you processor info<br />
• <strong>ccze </strong>: log colorizer, useful for reading var/log/messages (ex. “$sudo tailf /varl/og/messages I ccze” or “$sudo cat /var/log/messages / ccze -m ansi |less -r”)​<br />
• <strong>cd -</strong> : sends the user to the last directory they were in before the present one<br />
• <strong>clear </strong>: clears the screen<br />
• <strong>ctrl-a / ctrl- e</strong> : “$ctrl-a” go to the beginning of a line, “$ctrl-e” go to the end of the line<br />
• <strong>ctrl-z</strong> : pauses the running process, "$bg" to background, "$fg" to return it to the foreground<br />
• <strong>df- h</strong> : space on volumes, human readable​<br />
• <strong>dig</strong> : DNS lookup utility<br />
• <strong>dmesg -H </strong>: (H flag not available on all systems) boostrap info<br />
• <strong>du -hs </strong>: directory sizes, human readable<br />
• <strong>eject </strong>: eject removable media (as in an attached USB flash drive, etc)<br />
• <strong>env </strong>: shows you some info on the shell environment<br />
• <strong>mkdir -p</strong> : creates full path ex. "$sudo makdir -p home/Maildir/{cur,new,tmp}"<br />
• <strong>export VISUAL=nano; visudo </strong>: sets nano as the visudo editor<br />
• <strong>find /etc -name *conf </strong>: finds and displays all the config files under /etc<br />
• <strong>free -h</strong> : show you available space on disks, in human readable format<br />
• <strong>grep -Pri</strong> : searches for text tin the directory and subdirectories and puts it on the screen, ex: "$grep -Pri ." searches current directory<br />
• <strong>head </strong>: lists top of file<br />
• <strong>inode </strong>: contains all the information about any linux / Unix file, is an address to a specific disk block, IS the unix file except for the name, which is stored in the directory (together with the inode number) as a reference to the inode data. It truly is the file; <em>the name one sees in the directory is just a reference</em>.<br />
• <strong>inxi -Finc 0 &gt; system_data.txt </strong>: Creates a file that lists a huge amount of system hardware related details, somewhat like the Windows "C:\ systeminfo" command, requires downloading inxi (click <a href="https://github.com/smxi/inxi">here</a> for details)<br />
• <strong>kill $(pgrep mozilla</strong>) : Kills all processes associated with Mozilla Firefox, substitute the app name for "mozilla" to kill it.<br />
• <strong>lastlog </strong>: Shows all users that have logged in (or have the capability to login) and the dates and times of their logins, to limit this to those users who have logged in at some point use "$lastlog |grep -iv never"<br />
• <strong>ldd </strong>:  Lists the library dependencies of an executable<br />
• <strong>less </strong>: Pager, shows any text document where you can move through the document by one line, and or page, at a time
• <strong>locate</strong> :  (run"$sudo updatedb" first): fast search for files<br />
• <strong>logsave </strong>: saves command / terminal/ ssh session output to a file on the desktop with a timestamp<br />
• <strong>lsblk </strong>: lists all the block devices / partitions of the system<br />
• <strong>lslogins -u</strong> : show all users with logins, “$lslogins -Lu” show last user logins<br />
•<strong> lsof </strong>: list of open files on the system, <em>may require downloading lsof</em><br />
• <strong>lvm </strong>: logical volume manager for LUNs and disk partitions<br />
• <strong>man -f</strong> : lists details associated with the commands must run "$sudo makewhatis" first<br />
• <strong>man -k</strong> : searches man pages for the word or string <br />
• <strong>man ascii</strong> : outputs an ascii table<br />
<span style="font-weight:normal">• </span><strong>nano</strong><span style="font-weight:normal">: </span>text editor, ex “$nano mytext”, <em>may require downloading nano</em><br />
<span style="font-weight:normal">• </span><strong>ncdu -rx /</strong> : Scans the existing file system and orders directories by largest to smallest data size, fantastic for finding where all the free space has gone (think WinDirTree ), <em>may require downloading ncdu</em><br />
<span style="font-weight:normal">• </span><strong>nl</strong><span style="font-weight:normal">:</span> adds line numbers to a file<br />
<span style="font-weight:normal">• </span><strong>nmblookup</strong><span style="font-weight:normal"><strong> -A</strong> </span>: get the (Windows) netbios name from an IP address<br />
<span style="font-weight:normal">• </span><strong>nmon<span style="font-weight:normal"> / </span>glances</strong> : tools for displaying realtime stats on the system, <em>may require downloading </em><br />
<span style="font-weight:normal">• </span><strong>pstree -p</strong> : shows processes and PID in a tree format, very useful<br />
<span style="font-weight:normal">• </span><strong>pushd<span style="font-weight:normal"> / </span>popd</strong> : collects directories to a stack, moves between stack items<br />
<span style="font-weight:normal">• </span><strong>rev</strong> : reverses the output (as in “$sudo cat var/log/messages |rev”)<br />
<span style="font-weight:normal">• </span><strong>rpm -qa --last</strong> : shows files installed in descending order<br />
<span style="font-weight:normal">• </span><strong>rpm -qa</strong> : list all installed apps<br />
<span style="font-weight:normal">•<strong> </strong></span><strong>rpm -qa --last |head</strong> : shows recently installed files<br />
<span style="font-weight:normal">• </span><strong>screen</strong> : for creating virtual terminals (<em>more useful if logged in remotely, such as by ssh</em>)<br />
<span style="font-weight:normal">• </span><strong>script</strong> : logs all transactions of a terminal to a file<br />
<span style="font-weight:normal">• </span><strong>set</strong> : shows other shell environmental variables<br />
<span style="font-weight:normal">• </span><strong>ss</strong> : socket statistics, "$ss -a |grep -E "\b([0-9]{1,3}\.){3}[0-9]{1,3}\b|[^a-z][^:]:[^:][^:][0-9]" provides only sockets that are attached to an or any IP address.<br />
<span style="font-weight:normal">• </span><strong>stat</strong> : provides user /group data for the file or directory, ex. “$sudo stat myfile”<br />
<span style="font-weight:normal">•<strong> </strong></span><strong>su -</strong> : root privallages and root environment, use with caution<br />
<span style="font-weight:normal">• </span><strong>su</strong> : root privallages but keeps the current user environment, good for debugging<br />
<span style="font-weight:normal">• </span><strong>sudo -k</strong> : kills the sudo timer so root access isn't kept<br />
<span style="font-weight:normal">• </span><strong>sudo -s</strong> : Open a shell account with root privileges, use with caution<br />
<span style="font-weight:normal">• </span><strong>sudo !!</strong> : does the previous command again and puts ""sudo"" in front"<br />
<span style="font-weight:normal">• </span><strong>sudo cat /etc/passwd</strong><em> </em>: show list of users on the system, “$sudo cat /etc/passwd |grep -iv nologin” show all users with logins<br />
<span style="font-weight:normal">• </span><strong>sudo yum makecache fast</strong> : update yum fast mirror package index<br />
<span style="font-weight:normal">•<strong> </strong></span><strong>tail</strong> : lists end of file<br />
<span style="font-weight:normal">• </span><strong>uname -a</strong> : gives you linux kernel information<br />
<span style="font-weight:normal">• </span><strong>users</strong> : lists users on the system ("$w" and "$last" are also helpful)<span style="font-weight:normal">"</span><br />
<span style="font-weight:normal">• </span><strong>visudo</strong> <span style="font-weight:normal">: </span>safe secure way of editting the etc/sudoers file, locks the file, checks syntax<br />
<span style="font-weight:normal">• </span><strong>yum check-update</strong> <span style="font-weight:normal">:</span> shows programs on the system that have available updates<br />
<em><strong><a href="http://www.linux-commands-examples.com/_alpha-numerical">… &amp; more Linux commands here</a> and  <a href="https://en.wikipedia.org/wiki/List_of_Unix_commands">here</a></strong></em>

------------------------------------------------------------------------

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><div>
<div id="408847822115879374" class="wcustomhtml" data-align="center" style="width: 100%; overflow-y: hidden;">
<span id="Apps"></span>
<h2 id="linux-apps-1">Linux Apps</h2>
</div>
</div></td>
<td><div class="wsite-spacer" style="height:10px;">

</div></td>
</tr>
</tbody>
</table>

1. [Apache](https://httpd.apache.org/) / [NGINX](https://nginx.org/en/)
power the web  
2. [Docker](https://www.docker.com/),
[Vagrant](https://www.vagrantup.com/),
[KVM](https://www.linux-kvm.org/page/Main_Page),
[VirtualBox](https://www.virtualbox.org/), &
[VMWare](http://www.vmware.com/) power system deployment  
3. [RedHat Enterprise Linux
(RHEL)](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux),
[Suse Linux Enterprise Server
(SLES)](https://www.suse.com/products/server/)[,](https://www.suse.com/products/server/)
[CentOS](https://www.centos.org/), [Debian](https://www.debian.org/) and
[Windows](https://www.microsoft.com/en-us/cloud-platform/windows-server)
[Server](https://www.microsoft.com/en-us/cloud-platform/windows-server)
are the OS’s that power the web  
4. [Glances](https://nicolargo.github.io/glances/),
[htop](http://hisham.hm/htop/),
[gtop](https://github.com/aksakalli/gtop),
[bmon](https://github.com/tgraf/bmon) and Inixi are for monitoring
system behavior  
5. [Exa](https://github.com/ogham/exa),
[ccze](http://freshmeat.sourceforge.net/projects/ccze/),
[lnav](http://lnav.org/) and cat are for viewing stuff in the command
line  
6. [Nano](https://www.nano-editor.org/) and
[vim](https://www.vim.org/) and  are for editing  
7. [Brackets](http://brackets.io/),
[pycharm](https://www.jetbrains.com/pycharm/), and
[spyder](https://github.com/spyder-ide/spyder/blob/master/README.md) are
for python development  
8. [ELinks](http://elinks.or.cz/) is for browsing the web via the
command line  
9. [Shorewall](http://shorewall.org/index.html) as a system based
firewall  
10. [Webmin](http://www.webmin.com/) for controlling Linux servers via
the web  
11. [Fishshell](https://fishshell.com/) as a bash replacement, check out
it’s command tab completion (start typing a command, or type a command +
space, then tab, to see options / flags), want to learn more? Check this
*[out](https://rootnroll.com/d/fish-shell/)*  
12. [Tilix](https://github.com/gnunn1/tilix) as terminal emulator  
13. [Grsync / rsync](http://www.opbyte.it/grsync/) for backup  
14. [Brasero](https://wiki.gnome.org/Apps/Brasero) cd/dvd burning gnome
desktop utility  
15. [Nbtscan](http://www.unixwiz.net/tools/nbtscan.html) - netbios
scanner  
16. [Mc](https://midnight-commander.org/) - “Midnight Comander” a
command line, terminal “DOS-like” visual interface that interactively
does the work of ls, mv, cp, rm, mkdir, and ftp (and their clones like
exa), useful for beginners and or those who like graphics.  
17. [Micro](https://micro-editor.github.io/) - Most Linux users know of
the editors Vim, and perhaps Nano (see above); Micro is another editor
with easy to learn commands (like ctrl-s for save) plus syntax
highlighting ...  
18. [Pi-Hole](https://pi-hole.net/), a DNS blackhole that can be loaded
on several different versions of Linux (including Debian Ubuntu), to
keep ads away from your PC / Mac  
18. [TLDR](https://tldr.sh/) - Useful examples to a large list of Linux
/ Mac and Windows commands (did you know that tldr means "*to long
didn't read*"? Now you do ... ), *see below for the TLDR master list as
a PDF*

------------------------------------------------------------------------

------------------------------------------------------------------------

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><div>
<div id="353595331972954433" class="wcustomhtml" data-align="left" style="width: 100%; overflow-y: hidden;">
<span id="Cmd"></span>
<h2 id="must-have-command-line-apps">Must-have Command Line Apps</h2>
</div>
</div></td>
<td><div class="wsite-spacer" style="height:10px;">

</div></td>
</tr>
</tbody>
</table>

**Shell Replacements:**

1.  **[Fish](https://fishshell.com/)** - "Friendly interactive shell",
    shell replacement for BASH, provides syntax coloring, tab
    completions, themes and well *awesomeness *
2.  **[Zsh / Oh my Zsh](https://ohmyz.sh/)** - Shell replacement for
    BASH if you need / want POSIX compliance (if you don't know what
    POSIX is, we recommend **Fish**)

  
**Tools:**

1.  **[Micro](https://micro-editor.github.io/)** - As discussed above, a
    *really cool* text editor that provides syntax highlighting and more
    (otherwise we recommend *Vim* as an alternative)
2.  **[Ranger](https://github.com/ranger/ranger)** - A directory / file
    explorer providing an easier way to find files via the terminal -
    *sort of like Windows Explorer for the console.*
3.  **[Ncdu](https://dev.yorhel.nl/ncdu)** - Must-have tool that easily
    figures out how much space is on a system, and where big files /
    directories are lurking - *kinda like* *WinDirTree for Windows*
4.  [Bat](https://github.com/sharkdp/bat) - a Linux "cat" command
    alternative, provides syntax highlighting and enumeration in a
    clean, efficient interface - *we love this, and think you would too*
5.  **[MTR-tiny](https://www.linode.com/docs/networking/diagnostics/diagnosing-network-issues-with-mtr/)** -
    A package that combines ping and traceroute into a single tool with
    *superpowers* to isolate networking issues
6.  **[Lnav](https://lnav.org/)** - As discussed above, a tool to
    explore and decipher all of those *pesky cryptic log files* you need
    to review in order to troubleshoot an issue
7.  [Mulittail](https://www.vanheusden.com/multitail/) - View multiple
    log files at a time via the console - *often helps to uncover what's
    going on in a borked OS*
8.  **[Tig](https://github.com/jonas/tig)** - A terminal based Git
    client (for the *crafty* developers among you)
9.  **[Rtorrent](https://github.com/rakshasa/rtorrent)** - terminal
    based BitTorrent client - *for all that (ahem) legal downloading you
    do  ***;-)**
10. **[Ned](https://github.com/nevdelap/ned)** - because sed <span
    class="underline">sucks</span> - *yes it does *
11. [MyCli](https://github.com/dbcli/mycli) - Console client for MySql /
    MariaDB databases that does auto-completion and syntax
    highlighting  - *As most services with a web interface have a
    database in the back-end*
12. [Glances](https://nicolargo.github.io/glances/) - Console *(and
    web*) based server monitoring tool  (like top on steroids) - *See
    what's going on "at a glance", we use this often to monitor web
    services*
13. [Taskwarrior](https://taskwarrior.org/) - Manage ToDo / task lists
    from the console - *We like our Markdown GUI clients for individual
    lists, but this is mighty useful when you don't have a GUI*
14. [Calcurse](https://www.calcurse.org/) - Calendar and appointment
    tool for the console *- Again, for when you don't have a GUI to run
    Google Chrome / Firefox etc.*
15. [Htop](https://hisham.hm/htop/) - Top clone with syntax highlighting
    and mouse support - *The go-to must-have command line tool to
    understand what a Linux system is doing*
16. [Pandoc](https://pandoc.org/) - document converter *- Have a
    MediaWiki or .doc file you need to turn into html? This will do it,
    as well as whole lot more.*
17. [FireJail](https://firejail.wordpress.com/) - a Type of
    *[chroot](https://en.wikipedia.org/wiki/Chroot)* jail to sandbox
    processes, services, and or apps so they have less of a chance of
    affecting the greater environment - *This is one approach, another
    is to use a [Docker container](https://www.docker.com/why-docker),
    in specific circumstances*
18. [Docker](https://www.docker.com/) - the primary program to
    deploy services and or apps as
    [containers](https://www.docker.com/resources/what-container) -
    *review the links and this*
    *[cheat-sheet](https://www.docker.com/sites/default/files/d8/2019-09/docker-cheat-sheet.pdf)*
    *for more, invaluable to development / DevOps*

**Games:**

-   **[Nudoku](https://www.linuxlinks.com/nudoku/)** - Sudoko for the
    console / terminal (*available also for the Mac via homebrew*) -
    *it's not **all** about work*
-   **[Ninvaders](http://ninvaders.sourceforge.net/)** - Play space
    invaders via the console (*available also for the Mac via
    homebrew*) - *Because 80's Atari games never ever get old...*
-   [Bastet](https://fph.altervista.org/prog/bastet.html) - A Tetris
    clone for the console - *C'mon it's Tetris, for the console ... how
    isn't this cool?*
