#Position Thy Self
### in this challenge we apply the cd command to change directories

**Flag** 'pwn.college{MUKIm79YQ_GcXN0JDYbGWy5zY3h.QX2QTN0wSO1gjNzEzW}'

first i entered the command /challenge/run, as it was directed in the challenge.
throught this step, the actual directory of the program was revealed so i used the cd (change directory) command to change the pathway.
after that i simply used /challenge/run which worked this time as i was in the correct directory and the flag was given.

'''
hacker@paths ~ position-thy-self: ~  $ /challenge/run
Incorrect...
You are not currently in the /tmp directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths ~ position-thy-self: ~ $ cd /tmp
hacker@paths ~ position-thy-self:/tmp$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{MUKIm79YQ_GcXN0JDYbGWy5zY3h.QX2QTN0wSO1gjNzEzW}

'''

## What I learnt 
i learnt how to use the cd command to switch directories in the middle of me being in some other directory.

i also saw that after the cd command, the ~ before the $ changes to the directory's name.

## References
none used.
