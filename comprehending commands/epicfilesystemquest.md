# Epic Filesystem Quest

### this challenge tests all the commands we learnt before

**Flag** 'pwn.college{ELlm1ld1R-Ea-6c1P0L6Ns6xUDd.QX5IDO0wSO1gjNzEzW}'

in this challenge i had to follow all the paths that the terminal gave me, after all that i got the flag

```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
TRACE  challenge  flag  lib32   media  opt   run   sys  var
bin    dev        home  lib64   mnt    proc  sbin  tmp
boot   etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ ls -a
.           TRACE  challenge  flag  lib32   media  opt   run   sys  var
..          bin    dev        home  lib64   mnt    proc  sbin  tmp
.dockerenv  boot   etc        lib   libx32  nix    root  srv   usr
hacker@commands~an-epic-filesystem-quest:/$ /challenge
-bash: /challenge: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ cat challenge
cat: challenge: Is a directory
hacker@commands~an-epic-filesystem-quest:/$ cat TRACE
Tubular find!
The next clue is in: /usr/share/doc/liblrcalc1
hacker@commands~an-epic-filesystem-quest:/$ cd /user/share/doc/liblrcalc1
-bash: cd: /user/share/doc/liblrcalc1: No such file or directory
hacker@commands~an-epic-filesystem-quest:/$ cd /usr
hacker@commands~an-epic-filesystem-quest:/usr$ cd /share/doc
-bash: cd: /share/doc: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr$ cd /user
-bash: cd: /user: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr$ cd /share/doc/liblrcalc1
-bash: cd: /share/doc/liblrcalc1: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr$ cat /usr/share/doc/liblrcalc1
cat: /usr/share/doc/liblrcalc1: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr$ cd /usr/share/doc
hacker@commands~an-epic-filesystem-quest:/usr/share/doc$ cat liblrcalc1
cat: liblrcalc1: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/doc$ cd /liblrcalc1
-bash: cd: /liblrcalc1: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/doc$ cd liblrcalc1
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/liblrcalc1$ ls
ALERT  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/liblrcalc1$ ls -a
.  ..  ALERT  changelog.Debian.gz  copyright
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/liblrcalc1$ cat ALERT
Tubular find!
The next clue is in: /usr/share/icons/Humanity/status/32

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/liblrcalc1$ cd /usr/share/icons/Humanity/status/32
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ ls -a
.                                info.svg
..                               keys.svg
.README                          keys.xpm
aptdaemon-add.svg                locked.svg
dialog-error.svg                 messagebox_critical.svg
dialog-information.svg           messagebox_info.svg
dialog-question.svg              messagebox_warning.svg
dialog-warning.svg               network-wireless-encrypted.svg
error.svg                        status_lock.svg
gnome-dev-wavelan-encrypted.svg  stock_dialog-error.svg
gnome-unknown.svg                stock_dialog-info.svg
gtk-dialog-error.svg             stock_dialog-question.svg
gtk-dialog-info.svg              stock_dialog-warning.svg
gtk-dialog-question.svg          stock_lock.svg
gtk-dialog-warning.svg           stock_unknown.svg
gtk-missing-image.svg            xfce-system-lock.svg
image-missing.svg                xfce-unknown.svg
important.svg
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cat .README
Yahaha, you found me!
The next clue is in: /usr/lib/python3/dist-packages/zope

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cat /usr/lib/python3/dist-packages/zope
cat: /usr/lib/python3/dist-packages/zope: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ ls /usr/lib/python3/dist-packages/zope
HINT-TRAPPED  __init__.py  __pycache__  interface
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cat /usr/lib/python3/dist-packages/zope/HINT-TRAPPED
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/include/config/pcmcia

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ ls /opt/linux/linux-5.4/include/config/pcmcia
BRIEF-TRAPPED  load
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cat /opt/linux/linux-5.4/include/config/pcmcia/BRIEF-TRAPPED
Congratulations, you found the clue!
The next clue is in: /usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cd /usr/lib/python3/dist-packages/ympy/printing/pretty/__pycache__
-bash: cd: /usr/lib/python3/dist-packages/ympy/printing/pretty/__pycache__: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ ls /usr/lib/python3/dist-packages/sympy/printing/pretty/__pychache__
ls: cannot access '/usr/lib/python3/dist-packages/sympy/printing/pretty/__pychache__': No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cat /usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__
cat: /usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/share/icons/Humanity/status/32$ cd /usr/lib/python3/dist-packages/sympy/printing/pretty
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty$ ls
__init__.py  __pycache__  pretty.py  pretty_symbology.py  stringpict.py  tests
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty$ cd /__pycache__
-bash: cd: /__pycache__: No such file or directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty$ cat __pycache__
cat: __pycache__: Is a directory
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty$ cd __pycache__
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__$ ls
DISPATCH  __init__.cpython-38.pyc  pretty.cpython-38.pyc  pretty_symbology.cpython-38.pyc  stringpict.cpython-38.pyc
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__$ cat DISPATCH
Great sleuthing!
The next clue is in: /usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/STIX-Web/Size4
hacker@commands~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/printing/pretty/__pycache__$ cd /usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/STIX_Web/Size4
hacker@commands~an-epic-filesystem-quest:/usr$ cd /lib/python3
hacker@commands~an-epic-filesystem-quest:/lib/python3$ cd /usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/STIX-Web/Size4
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/STIX-Web/Size4$ ls
Regular  SPOILER
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/STIX-Web/Size4$ cat SPOILER
Congratulations, you found the clue!
The next clue is in: /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/stdlib/2and3/pydoc_data

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/usr/share/javascript/mathjax/unpacked/jax/output/HTML-CSS/fonts/STIX-Web/Size4$ cd  /usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/stdlib/2and3/pydoc_data
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/stdlib/2and3/pydoc_data$ ls
REVELATION  __init__.pyi  topics.pyi
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/stdlib/2and3/pydoc_data$ cat REVELATION
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/hwtracing/coresight

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/jedi/third_party/typeshed/stdlib/2and3/pydoc_data$ cd /opt/linux/linux-5.4/drivers/hwtracing/coresight
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/hwtracing/coresight$ ls -a
.           coresight-catu.c       coresight-etm-perf.c     coresight-etm4x-sysfs.c  coresight-priv.h        coresight-tmc.c
..          coresight-catu.h       coresight-etm-perf.h     coresight-etm4x.c        coresight-replicator.c  coresight-tmc.h
.BLUEPRINT  coresight-cpu-debug.c  coresight-etm.h          coresight-etm4x.h        coresight-stm.c         coresight-tpiu.c
Kconfig     coresight-etb10.c      coresight-etm3x-sysfs.c  coresight-funnel.c       coresight-tmc-etf.c     coresight.c
Makefile    coresight-etm-cp14.c   coresight-etm3x.c        coresight-platform.c     coresight-tmc-etr.c
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/hwtracing/coresight$ cat .BLUEPRINT
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{ELlm1ld1R-Ea-6c1P0L6Ns6xUDd.QX5IDO0wSO1gjNzEzW}
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/hwtracing/coresight$
```

## What i learnt
how to use all the commands we learnt befere together
## References
none
non

``````
