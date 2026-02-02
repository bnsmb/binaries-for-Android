# binaries-for-Android

This repository contains binaries I compiled for Android running on **arm64** CPUs (well, most of them)

The binaries in the directory **binaries** are all either static linked or dynamically linked for only the standard libraries from Android. They should therefore run on any Android OS
The binaries run on Android 13 and newer Android versions (most probably also on older versions)

Binaries in this repository as of **02.02.2026** are

| Binary | version | source code | comment |
| ---| ---| ---| ---|
| static_gdb/ | 16.3 | https://sourceware.org/gdb/ | statically linked gdb binaries |
| 7zz_25.00_static  | 25.00 | https://www.7-zip.org | statically linked | 
| 7zz | 25.01 | https://www.7-zip.org | |
| bash | 5.2.37|  https://www.gnu.org/software/bash/ | dynamically linked for the Android OS libraries |
| bash-static | 5.2.37|  https://www.gnu.org/software/bash/ | statically linked |
| bash-static-stripped  | 5.2.37|  https://www.gnu.org/software/bash/ | statically linked and stripped |
| bc | 1.08.1 | https://www.gnu.org/software/bc/ | |
| bmore | 1.5.0 | https://bvi.sourceforge.net/ |  |
| bmore.static | 1.5.0 | https://bvi.sourceforge.net/ | this is a statically linked binary | 
| btop | 1.4.4 | https://github.com/aristocratos/btop | btop needs root access or permissive selinux mode |
| bvi | 1.5.0 | https://bvi.sourceforge.net/ | |
| bvi.static | 1.5.0 | https://bvi.sourceforge.net/ | this is a statically linked binary |
| cpio | 2.9 | https://www.gnu.org/software/cpio/ |  |
| curl | 8.17.0 | https://github.com/curl/curl |  |
| dig | 9.11.37 | https://gitlab.isc.org/isc-projects/bind9 |  |
| dcmtl |  |  |  for API version 33, 34, and 35 |
| find | 4.9.0 | https://www.gnu.org/software/findutils/ | |  
| funzip | 3.94 | https://infozip.sourceforge.net/ | |
| fuser | 22.14 | https://github.com/acg/psmisc | | 
| gawk | 5.3.2 |  https://www.gnu.org/software/gawk/ | |
| gunzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| gzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| htop | 3.4.1 | https://github.com/htop-dev/htop | the default config file for this htop binary is /data/local/tmp/etc/htoprc | 
| htop_static | 3.4.1 | https://github.com/htop-dev/htop | this is a statically linked binary; the default config file for this htop binary is /data/local/tmp/etc/htoprc | 
| klllall | 22.14 | https://github.com/acg/psmisc | | 
| less | 661 | https://ftp.gnu.org/gnu/less/ | |
| lessecho | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| lesskey | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| losetup | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| lpdump | | | | 
| mkfs.ext3 | 1.47.2 | https://git.kernel.org/pub/scm/fs/ext2/e2fsprogs.git | | 
| mkfs.ext4 |1.47.2 | https://git.kernel.org/pub/scm/fs/ext2/e2fsprogs.git | | 
| mksh | @(#)MIRBSD KSH R59 2025/06/02 | https://github.com/MirBSD/mksh | | 
| mount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| nano | 8.2, 8.4, 8.5, 8.6, 8.7 | https://www.nano-editor.org/git.php | |
| ncat  | 7.93 | https://nmap.org/ncat/ | | 
| ngrep | 1.47.1 | https://github.com/jpr5/ngrep| |
| nmon | 16q | https://nmon.sourceforge.io/pmwiki.php |  |
| openssl | 3.5.5 |  https://github.com/openssl/openssl | OpenSSL 3.5 is an LTS version |
| pigz | 2.8 | https://zlib.net/pigz/ | |
| protoc-32.1.0 | 32.1.0 | https://github.com/protocolbuffers/protobuf | | 
| pstree | 22.14 | https://github.com/acg/psmisc | | 
| rsync | 3.4.1 | https://github.com/RsyncProject/rsync | |
| script | 2.48 | https://github.com/util-linux/util-linux/ | |
| sepolicy-inject |  | |
| socat | 1.8.0.2 | http://www.dest-unreach.org/socat  | |
| sqlite3 | 3.50.1 | https://github.com/sqlite/sqlite/ | |
| sqlite3.static | 3.50.1 | https://github.com/sqlite/sqlite/ | this is a statically linked binary |
| sqlite3-3.50.4 | 3.50.4 | https://github.com/sqlite/sqlite/ | |
| sqlite3-3.50.4.static  | 3.50.4 | https://github.com/sqlite/sqlite/ | this is a statically linked binary |
| sqlite3_3.51.1 | 3.51.1 |  https://github.com/sqlite/sqlite/ | |
| strace | 6.18 | https://github.com/strace | | 
| tmux | 3.5a | https://github.com/tmux/tmux  | see below for additional infos | 
| toybox_with_debug_infos | 0.8.11-android | | toybox binary compiled with debug infos |
| umount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| unfsd | 0.11.0 | https://github.com/unfs3/unfs3 | a userland NFS v3 daemon; see [here](http://bnsmb.de/Magisk_Modules.html#Documentation_for_the_Magisk_Module_with_unfsd3) or this [post](https://xdaforums.com/t/guide-how-to-share-directories-on-the-phone-running-android-via-nfs-as-non-root-user.4756743/) in XDA| 
| unzip | 5.52 | https://infozip.sourceforge.net/ | |
| unzipsfx | 5.52 | https://infozip.sourceforge.net/ | |
| vim | 9.1 | https://github.com/vim/vim  | |
| wget2 | 2.1.0 | https://gitlab.com/gnuwget/wget2 | |
| xxd | 9.1 | https://github.com/vim/vim  | |
| xz | 5.8.1 | https://github.com/tukaani-project/xz | |
| zip | 3.0 | https://infozip.sourceforge.net/Zip.html | |

------

**Notes**

To use the **tmux** binary as user **shell**, the SELinux permissions 

"allow shell shell_data_file sock_file { create getattr setattr write unlink }"  
"allow shell devpts chr_file { read write open }" 

are required; without these permissions **root** access is necessary to run **tmux** in an adb session

-------

The files **openssh_9.9p2_v1.0.0.tar.gz**, **openssh_9.9p1_v1.1.0.tar.gz**, and **openssh_10.0p2_v1.2.0.tar.gz** in the directory **tar_files** contain **OpenSSH binaries and files** for the Android operating system, which can be installed in the directory **/data/local/tmp**  so that the user **shell** can start an **sshd** on the phone.


see 

[http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access](http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access)

or


[https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/](https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/)

for details

-------

The tar files **terminfo.tar** and **terminfo_without_hardlinks.tar** contain **terminfo databases**. Terminfo databases are required by programs that have been compiled with **ncurses** or a similar library (such as **gdb**).
Not all Android versions contain a terminfo database. To use one of these terminfo databases, extract the tar file in the directdory **/data/local/tmp** on the phone and set the environment variables **TERMINFO** and **TERM**, e.g.

```
export TERMINFO=/data/local/tmp/terminfo
export TERM=vt100
```

--------

