# touching files
### this challenge directs us to make new files through the terminals

**Flag** 'pwn.college{AGay8kT7AIQIBJHQvHjvfVsowF-.QXwMDO0wSO1gjNzEzW}'

in this challenge we were directed to create new fiies using the touch command. the files that were required to create were pwn and college
i changed the directories to /tmp and then used the touch command.
after that i had to simply run /challenge/run to get the flag.

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{AGay8kT7AIQIBJHQvHjvfVsowF-.QXwMDO0wSO1gjNzEzW}
```

## What i learnt
touch command is used to create a new file straight through the terminal

## references
none
