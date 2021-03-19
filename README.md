## Dolphin service menu: Directory unmounter

Unmount anything mounted in a directory using "Unmount" from service menu. It can also try to delete directory after mount with "Unmount and delete directory" option.

It first tries to unmount without root privileges using `fusermount`, and if that doesn't work, it uses `pkexec` to execute umount with root privileges.

![Screenshot](screenshot.png)
