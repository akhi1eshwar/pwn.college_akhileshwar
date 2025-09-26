# hidden files

### in this challenge we learn how to find hidden files in a directory
**Flag** 'pwn.college{s1Q2Hdgve4h5sTT7clV-cXhT3Yp.QXwUDO0wSO1gjNzEzW}'

in this challenge i had to change directories to / and use ls -a to find the hidden files
after that i just used cat to retrieve the flag

```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv           bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-1288755702756  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-1288755702756
pwn.college{s1Q2Hdgve4h5sTT7clV-cXhT3Yp.QXwUDO0wSO1gjNzEzW}
hacker@commands~hidden-files:/$ 
```

## What i learnt
i learnt that files can also be hidden and there is a command ls -a to find those hidden files

## References
none
