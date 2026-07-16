# binaries-for-Android

This repository contains binaries I compiled for Android running on **arm64** CPUs (well, most of them)

The binaries in the directory **binaries** are all either static linked or dynamically linked for only the standard libraries from Android. They should therefore run on any Android OS
The binaries run on Android 13 and newer Android versions (most probably also on older versions)

Binaries in this repository as of **15.04.2026** are

| Binary | version | source code | comment |
| ---| ---| ---| ---|
| static_gdb16/* | 16.3 | https://sourceware.org/gdb/ | statically linked gdb binaries |
| static_gdb17.1/*  | 17.1 | https://sourceware.org/git/binutils-gdb.git | statically linked gdb binaries | 
| static_gdb17.2/*  | 17.2 | https://sourceware.org/git/binutils-gdb.git | statically linked gdb binaries |
| 7zz_26.01_static  | 26.01 | https://www.7-zip.org | this is a statically linked binary |
| 7zz | 26.01 | https://www.7-zip.org | |
| aapt2 | | |
| bash | 5.2.37|  https://www.gnu.org/software/bash/ | dynamically linked for the <br>Android OS libraries |
| bash-static | 5.2.37|  https://www.gnu.org/software/bash/ | this is a statically linked binary |
| bash-static-stripped  | 5.2.37|  https://www.gnu.org/software/bash/ | This is statically linked and stripped <br>binary |
| bat | 0.26.1 | https://github.com/sharkdp/bat | bat is a replacement for cat |
| bc | 1.08.1 | https://www.gnu.org/software/bc/ | |
| bmore | 1.5.0 | https://bvi.sourceforge.net/ |  |
| bmore.static | 1.5.0 | https://bvi.sourceforge.net/ | this is a statically linked binary | 
| bpftool_5.16.0 | 5.16.0 | | bpftool compiled with the source code <br>from /e/ 4.0 (= Android 16) and the kernel files for <br>the ASUS Zenfone 8 | 
| bpftool_static_5.16.0 | 5.16.0 | | bpftool compiled with the source code from  <br>/e/ 4.0 (= Android 16) <br>and the kernel <br>files for the ASUS Zenfone 8 <br> this is a statically linked binary|
| btop | 1.4.7 | https://github.com/aristocratos/btop | btop can be used by any user now. However,  btop needs root <br>access or permissive SElinux mode <br>to read the network statistics.<br> When started by a non-root ser with SELinux enabled, <br>btop prints "[limited]" after the IP address |
| bvi | 1.5.0 | https://bvi.sourceforge.net/ | |
| bvi.static | 1.5.0 | https://bvi.sourceforge.net/ | this is a statically linked binary |
| cpio | 2.15 | https://www.gnu.org/software/cpio/ |  |
| curl | 8.17.0 | https://github.com/curl/curl |  |
| curl-8.19.0 | 8.19.0 |  https://github.com/curl/curl |  |
| darkhttpd | 1.17 | https://github.com/emikulic/darkhttpd | | 
| darkhttpd_static | 1.17 | https://github.com/emikulic/darkhttpd | this is a statically linked binary |
| dig | 9.11.37 | https://gitlab.isc.org/isc-projects/bind9 | dig is used for hostname resolution <br>via DNS (like nslookup)  |
| dog | 0.2.0 |  https://github.com/ogham/dog | dog is a replacement for dig or nslookup |
| dnsmasq | 2.92rc3 | https://thekelleys.org.uk/dnsmasq/doc.html | see http://bnsmb.de/Magisk_Modules.html#Documentation_for_the_Magisk_Module_with_dnsmasq or https://xdaforums.com/t/module-magisk-module-with-dnsmasq-for-the-android-os.4784807/ for the documentation |
| dmctl_binaries |  |  | dmctl binaries compiled for <br>Android 13, 14, 15, and 16 |
| dua | 2.38.0 | https://github.com/Byron/dua-cli | dua is a replacment for du |
| dust | 1.2.4 | https://github.com/bootandy/dust | dust is a replacement for du | 
| eza | 0.23.5 | https://github.com/eza-community/eza | eza is a replacement for ls
| fd | 10.4.2 | https://github.com/sharkdp/fd | fd is a replacement for find |
| find | 4.9.0 | https://www.gnu.org/software/findutils/ | |  
| funzip | 3.94 | https://infozip.sourceforge.net/ | |
| fuser | 22.14 | https://github.com/acg/psmisc | | 
| gawk | 5.3.2 |  https://www.gnu.org/software/gawk/ | |
| gunzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| gzip | 1.13 | https://www.gnu.org/software/gzip/ |  |
| htop_3.5.1 | 3.5.1 | https://github.com/htop-dev/htop | the default config file for this htop binary<br>  is /data/local/tmp/etc/htoprc | 
| htop_static_3.5.1 | 3.5.1 | https://github.com/htop-dev/htop | this is a statically linked binary; <br> the default config file for this htop binary <br>is /data/local/tmp/etc/htoprc |
| jq-1.7.1 | 1.7.1 | https://jqlang.org/ | | 
| klllall | 22.14 | https://github.com/acg/psmisc | | 
| lpadd | | | |
| less | 661 | https://ftp.gnu.org/gnu/less/ | |
| lessecho | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| lesskey | 1.15 | https://ftp.gnu.org/gnu/less/ | |
| losetup | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| lpdump | | | | 
| ltrace | 0.8.1 | https://ltrace.org/ | | 
| ltrace_static | 0.8.1 | https://ltrace.org | this is a statically linked binary |
| mkfs.ext3 | 1.47.2 | https://git.kernel.org/pub/scm/fs/ext2/e2fsprogs.git | | 
| mkfs.ext4 |1.47.2 | https://git.kernel.org/pub/scm/fs/ext2/e2fsprogs.git | | 
| mksh | @(#)MIRBSD KSH R59 2025/12/23 | https://github.com/MirBSD/mksh | | 
| mount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| mount_dynamic_partitions | 1.1.0 | https://github.com/bnsmb/parse-android-dynparts-for-Android | http://bnsmb.de/My_HowTos_for_Android.html#How_to_mount_the_root_filesystem__and_other_dynamic_partitions_in_Android_in_readwrite_mode
| nano_9.1 | 9.1 | https://www.nano-editor.org/git.php | |
| nano_static_9.1 | 9.1 | https://www.nano-editor.org/git.php | this is a statically linked binary|
| ncat  | 7.93 | https://nmap.org/ncat/ | | 
| ngrep | 1.48.3 | https://github.com/jpr5/ngrep| |
| nmon | 16q | https://nmon.sourceforge.io/pmwiki.php |  |
| openssl-3.5.6 | 3.5.6 |  https://github.com/openssl/openssl | OpenSSL 3.5 is an LTS version |
| openssl-4.0.0 | 4.0.0 | https://github.com/openssl/openssl | |
| openvpn | 2.7 | https://openvpn.net/ | | 
| pagemon | 0.02.06 | https://github.com/ColinIanKing/pagemon | |
| pigz | 2.8 | https://zlib.net/pigz/ | |
| procs | 0.14.12 | https://github.com/dalance/procs | procs is a replacment for ps |
| protoc-32.1.0 | 32.1.0 | https://github.com/protocolbuffers/protobuf | | 
| pstree | 22.14 | https://github.com/acg/psmisc | | 
| ripgrep | 15.1.0 | https://github.com/BurntSushi/ripgrep | ripgrep is a recursively searching grep | 
| rsync | 3.4.1 | https://github.com/RsyncProject/rsync | |
| script | 2.48 | https://github.com/util-linux/util-linux/ | |
| sepolicy-inject |  | |
| socat | 1.8.0.2 | http://www.dest-unreach.org/socat  | |
| sqlite3 | 3.50.1 | https://github.com/sqlite/sqlite/ |  |
| sqlite3.static | 3.50.1 | https://github.com/sqlite/sqlite/ | this is a statically linked binary |
| sqlite3_3.51.1 | 3.51.1 |  https://github.com/sqlite/sqlite/ | |
| strace | 6.18 | https://github.com/strace | | 
| stunnel | 5.77 | https://www.stunnel.org/ | | 
| stunnel_static | 5.77 | https://www.stunnel.org/ | this is a statically linked binary |
| tmux | 3.5a | https://github.com/tmux/tmux  | see below for additional infos | 
| toybox_with_debug_infos | 0.8.11-android | | toybox binary compiled with debug infos |
| umount | util-linux 2.40 | https://github.com/util-linux/util-linux/ | this is a statically linked binary |
| unfsd | 0.11.0 | https://github.com/unfs3/unfs3 | a userland NFS v3 daemon; <br> see [here](http://bnsmb.de/Magisk_Modules.html#Documentation_for_the_Magisk_Module_with_unfsd3) or this [post](https://xdaforums.com/t/guide-how-to-share-directories-on-the-phone-running-android-via-nfs-as-non-root-user.4756743/) in XDA| 
| unzip | 5.52 | https://infozip.sourceforge.net/ | |
| unzipsfx | 5.52 | https://infozip.sourceforge.net/ | |
| vim_9.1_static | 9.1 | https://github.com/vim/vim  | this is a statically linked binary|
| vim_9.2 | 9.2 | https://github.com/vim/vim  | |
| wget2 | 2.1.0 | https://gitlab.com/gnuwget/wget2 | |
| xcp | 0.24.8 | https://github.com/tarka/xcp | a companion for the cp command | 
| xxd | 9.1 | https://github.com/vim/vim  | |
| xz | 5.8.1 | https://github.com/tukaani-project/xz | |
| zip | 3.0 | https://infozip.sourceforge.net/Zip.html | |

Older versions of some of the tools are in the sub directory [./archive](https://github.com/bnsmb/binaries-for-Android/tree/main/binaries/archive). 


------
**Notes**

To use the **tmux** binary as user **shell**, the SELinux permissions 
```
"allow shell shell_data_file sock_file { create getattr setattr write unlink }"  
"allow shell devpts chr_file { read write open }" 
```
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
**Update 24.02.2026**

see this post 

[https://xdaforums.com/t/exe-static-linux-binaries-for-arm-android-cryptsetup-encfs-f2fs-tools-testdisk-photorec.3709380/](https://xdaforums.com/t/exe-static-linux-binaries-for-arm-android-cryptsetup-encfs-f2fs-tools-testdisk-photorec.3709380/)

for a list of other available Unix binaries for Android




