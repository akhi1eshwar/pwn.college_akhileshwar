# Position Yet Elsewhere

## we position ourselves into another directory this time

**Flag** 'pwn.college{IFcTAgCtTGbZKOsgSZhS72bcxX4.QX4QTN0wSO1gjNzEzW}'

same as the last two challenges, we now go to another directory to find the absolute path to the program using cd.


'''
hacker@paths~position-yet-elsewhere: ~ $ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc/fontconfig directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths ~ position-yet-elsewhere: ~ $ cd /usr/share/doc/fontconfig
hacker@paths ~ position-yet-elsewhere:/usr/share/doc/fontconfig$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{IFcTAgCtTGbZKOsgSZhS72bcxX4.QX4QTN0wSO1gjNzEzW}
'''

## What i Learnt
futher mastery on the cd command

## References
none used.
