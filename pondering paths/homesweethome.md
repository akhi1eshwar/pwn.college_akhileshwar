# Home Sweet Home

### this challenge, we had to write an absolute path to a file in the home directory

**Flag** 'pwn.college{MlYwgEBp0j6labQR01iTVqorlht.QXzMDO0wSO1gjNzEzW}'

i had some trouble understanding what to do in the beginning, but eventually understood what the problem meant. i just located to a new file /challenge/run ~/a and the flag got copied to it. after that it simply printed out the flag

```
hacker@paths~home-sweet-home:~$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{MlYwgEBp0j6labQR01iTVqorlht.QXzMDO0wSO1gjNzEzW}

```

## what i learnt
~ is short for /home/hacker

## references
none
