# Learning complex usage
### this challenge gives you a task to get flag using --printfile argument
 **Flag** 'pwn.college{Ua3AqHQDYSyW_2UT3l66RzONp5Q.QX1ITO0wSO1gjNzEzW}'

i used /challenge/challenge --printfile /challenge/DESCRIPTION.md as directed in the hints
after that i tried to retrieve the flag the same method.


```
acker@man~learning-complex-usage:~$ /challenge/challenge --printfile /challenge/DESCRIPTION.md
Correct argument! Here is the /challenge/DESCRIPTION.md file:
While using most commands is straightforward, the usage of some commands can get quite complex.
For example, the arguments to commands like `sed` and `awk`, which we're definitely not getting into right now, are entire programs in an esoteric programming language!
Somewhere on the spectrum between `cd` and `awk` are commands that take arguments to their arguments...

This sounds crazy, but you've already encountered this with the `find` level in [Basic Commands](/linux-luminarium/commands).
`find` has a `-name` argument, and the `-name` argument itself takes an argument specifying the name to search for.
Many other commands are analogous.

Here is this level's documentation for `/challenge/challenge`:

> Welcome to the documentation for `/challenge/challenge`! This program allows you to print arbitrary files to the terminal, when given the `--printfile` argument. The argument to the `--printfile` argument is the path of the flag to read. For example, `/challenge/challenge --printfile /challenge/DESCRIPTION.md` will print out the description of the level!

Given that documentation, go get the flag!
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile flag
Correct argument! Here is the flag file:
cat: flag: No such file or directory
hacker@man~learning-complex-usage:~$ /challenge/challenge --printfile /flag
Correct argument! Here is the /flag file:
pwn.college{Ua3AqHQDYSyW_2UT3l66RzONp5Q.QX1ITO0wSO1gjNzEzW}
hacker@man~learning-complex-usage:~$ 

```

## What i learnt
what complex commands are and how to use them

## References
none.
