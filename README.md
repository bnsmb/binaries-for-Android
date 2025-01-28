# binaries-for-Android

This repository contains binaries I compiled for Android running on **arm64** CPUs

The binaries in the directory **binaries** are all either static linked or dynamically linked for only the standard libraries from Android. They should therefore run on any Android OS
The binaries run on Android 13 and newer Android versions (most probably also on older versions)



The file **openssh_9.9p1_v1.1.0.tar.gz** in the directory **tar_files** contains **OpenSSH binaries and files** for the Android operating system, which can be installed in the directory **/data/local/tmp**  so that the user **shell** can start an sshd on the phone.

see 

[http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access](http://bnsmb.de/My_HowTos_for_Android.html#How_to_connect_to_Android_via_ssh_as_user_shell_without_root_access)

or


[https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/](https://xdaforums.com/t/guide-how-to-connect-to-android-via-ssh-as-user-shell-without-root-access.4707534/)

for details
