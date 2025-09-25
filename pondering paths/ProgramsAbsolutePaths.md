# Program and Absolute Paths
### a slightly more difficult challenge to find an absolute path of a program

**Flag** 'pwn.college{kx97_fctaF51j72DRT7-1kH3TKV.QX1QTN0wSO1gjNzEzW}'

in this challenge i just had to add the command "challenge" after the "/ root" to get to the point to run the program. instead of directly running it from the root.
this shows that the run program was not in the root but a directory called challenge in root.

'''
hacker@paths ~ program-and-absolute-paths: ~ $ /challenge/run
Correct!!!
/challenge/run is an absolute path! Here is your flag:
pwn.college{kx97_fctaF51j72DRT7-1kH3TKV.QX1QTN0wSO1gjNzEzW}
hacker@paths~program-and-absolute-paths:~$ 
'''

## What i learnt
I learnt locating the directories in the root and running a program from that directory. this strengthened my understanding of file systems.

## References
none used.
