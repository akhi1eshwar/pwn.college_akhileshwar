# Position Elsewhere
## now to position from one directory to another, we once again use change directory command

**Flag** 'pwn.college{gHBulA8xkFE8uRxYF6zwqgiEeZY.QX3QTN0wSO1gjNzEzW}'

this challenge was almost exactly similar to the previous one. i ran /challenge/run but it didn't work because i wasn't in the correct directory
the terminal told me which directory the program was in so i added the directory using the cd command. only this time, the directory was a bit longer.
after i ran /challenge/run again, it worked and i got the flag.

'''
hacker@paths ~ position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths ~ position-elsewhere:~$ cd /usr/share/doc
hacker@paths ~ position-elsewhere:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{gHBulA8xkFE8uRxYF6zwqgiEeZY.QX3QTN0wSO1gjNzEzW}
hacker@paths~position-elsewhe
'''

## What i learnt

I learnt how to change directories in the linux terminal

## References

none used.
