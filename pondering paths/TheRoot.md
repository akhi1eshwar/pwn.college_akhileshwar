# The Root
### finding the root directory of a file/progran

**Flag** 'pwn.college{E1okUyQ-aPSleN9cHlTYG4PFPNK.QX4cTO0wSO1gjNzEzW}'

to get the flag, we only had to use the /pwn command, which basically means that after the "/"(the root of the filesystem), we look for the pwn directory which may contain other directories.

commands:
'''
hacker@paths~the-root:~$ /pwn
BOOM!!!
Here is your flag:
pwn.college{E1okUyQ-aPSleN9cHlTYG4PFPNK.QX4cTO0wSO1gjNzEzW}
hacker@paths~the-root:~$ 
'''

## What i learnt

through this challenge i learnt what the root of the file system is and what diretories are. The root is the main directory of the whole filesystem and contains all the directories. 
directories are basically just pathways in the file system that we need to use to access any file that we may need.

## References
none used.
