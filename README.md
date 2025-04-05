# binaries-for-Android

This repository contains binaries I compiled for Android running on **arm64** CPUs

The binaries in the directory **binaries** are all either static linked or dynamically linked for only the standard libraries from Android. They should therefore run on any Android OS
The binaries run on Android 13 and newer Android versions (most probably also on older versions)

Binaries in this repository as of **05.04.2025** are

| Binary | version | comment |
| ---| ---| ---| 
| 7zz  | 24.05 |
| gawk | 5.2.0 |  |
| bash | 5.2.37|  |
| bc | 1.08.1 |  |
| bmore | 1.4.2 | | 
| bvi | 1.4.2 | |
| cpio | 2.9 | |
| curl | 8.11.1 | |
| dig | 9.11.37 | |
| dcmtl |  |  for API version 33, 34, and 35 |
| funzip | 3.94 | |
| gunzip | 1.13 | |
| gzip | 1.13 | |
| less | 463 | |
| lessecho | 1.15 | |
| nano | 8.2 | |
| ngrep | 1.47.1 | |
| nmon | 16q | |
| openssl | 3.3.1.4 | |
| pigz | 2.8 | |
| rsync | 3.3.0 | |
| scdript | 2.48 | |
| sepolicy-inject |  |
| socat | 1.8.0.2 | |
| sqlite3 | 3.47.0 | |
| tmux | 3.5a | |
| unzip | 5.52 | |
| unzipsfx | 5.52 | |
| vim | 9.1 | |
| wget2 | 2.1.0 | |
| xxd | 9.1 | |
| xz | 5.6.2 | |
| zip | 3.0 | |



The files **openssh_9.9p2_v1.0.0.tar.gz** and **openssh_9.9p1_v1.1.0.tar.gz** in the directory **tar_files** contain **OpenSSH binaries and files** for the Android operating system, which can be installed in the directory **/data/local/tmp**  so that the user **shell** can start an sshd on the phone.


see 

[http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access](http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access)

or


[https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/](https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/)

for details
