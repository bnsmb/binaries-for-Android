# binaries-for-Android

This repository contains binaries I compiled for Android running on **arm64** CPUs (well, most of them)

The binaries in the directory **binaries** are all either static linked or dynamically linked for only the standard libraries from Android. They should therefore run on any Android OS
The binaries run on Android 13 and newer Android versions (most probably also on older versions)

Binaries in this repository as of **22.06.2025** are

| Binary | version | source code | comment |
| ---| ---| ---| ---|
| 7zz  | 24.05 | https://www.7-zip.org | | 
| gawk | 5.3.2 |  https://www.gnu.org/software/gawk/ | |
| bash | 5.2.37|  https://www.gnu.org/software/bash/ | dynamically linked for the Android OS libraries |
| bash-static | 5.2.37|  https://www.gnu.org/software/bash/ | statically linked |
| bash-static-stripped  | 5.2.37|  https://www.gnu.org/software/bash/ | statically linked and stripped |
| bc | 1.08.1 | https://www.gnu.org/software/bc/ | |
| bmore | 1.4.2 | https://bvi.sourceforge.net/ |  |
| bvi | 1.4.2 | https://bvi.sourceforge.net/ | |
| cpio | 2.9 | https://www.gnu.org/software/cpio/ |  |
| curl | 8.13.0 | https://github.com/curl/curl |  |
| dig | 9.11.37 | https://gitlab.isc.org/isc-projects/bind9 |  |
| dcmtl |  |  |  for API version 33, 34, and 35 |
| funzip | 3.94 | https://infozip.sourceforge.net/ | |
| gunzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| gzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| less | 661 | https://ftp.gnu.org/gnu/less/ | |
| lessecho | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| lesskey | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| losetup | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| mount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| nano | 8.2 | https://www.nano-editor.org/git.php | |
| ngrep | 1.47.1 | https://github.com/jpr5/ngrep| |
| nmon | 16q | https://nmon.sourceforge.io/pmwiki.php | |
| openssl | 3.3.1.4 |  https://github.com/openssl/openssl | |
| pigz | 2.8 | https://zlib.net/pigz/ | |
| rsync | 3.3.0 | https://github.com/RsyncProject/rsync | |
| script | 2.48 | https://github.com/util-linux/util-linux/ | |
| sepolicy-inject |  | |
| socat | 1.8.0.2 | http://www.dest-unreach.org/socat  | |
| sqlite3 | 3.50.1 | https://github.com/sqlite/sqlite/ | |
| tmux | 3.5a | https://github.com/tmux/tmux  | see below for additional infos | 
| unzip | 5.52 | https://infozip.sourceforge.net/ | |
| unzipsfx | 5.52 | https://infozip.sourceforge.net/ | |
| vim | 9.1 | https://github.com/vim/vim  | |
| wget2 | 2.1.0 | https://gitlab.com/gnuwget/wget2 | |
| xxd | 9.1 | https://github.com/vim/vim  | |
| xz | 5.8.1 | https://github.com/tukaani-project/xz | |
| zip | 3.0 | https://infozip.sourceforge.net/Zip.html | |
| pstree | 22.14 | https://github.com/acg/psmisc | | 
| fuser | 22.14 | https://github.com/acg/psmisc | | 
| klllall | 22.14 | https://github.com/acg/psmisc | | 
| umount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |

------

**Notes**

To use the **tmux** binary as user **shell**, the SELinux permissions 

"allow shell shell_data_file sock_file { create getattr setattr write unlink }"  
"allow shell devpts chr_file { read write open }" 

are required; without these permissions **root** access is necessary to run **tmux** in an adb session

-------

The files **openssh_9.9p2_v1.0.0.tar.gz**, **openssh_9.9p1_v1.1.0.tar.gz**, and **openssh_10.0p2_v1.1.0.tar.gz** in the directory **tar_files** contain **OpenSSH binaries and files** for the Android operating system, which can be installed in the directory **/data/local/tmp**  so that the user **shell** can start an **sshd** on the phone.


see 

[http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access](http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access)

or


[https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/](https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/)

for details
