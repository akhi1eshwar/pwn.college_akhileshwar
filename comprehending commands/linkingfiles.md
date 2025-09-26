# linking files

### this challenge asks us to create a symbolic link to a file 

**flag** 'pwn.college{Qfduj8LqOIk7qgyXtPpl0WbQBeQ.QX5ETN1wSO1gjNzEzW}'

in this challenge wewere asked to make a symbolic link to the flag with ~/not-the-flag
after that i just went to /challenge/catflag to get the flag.

```
hacker@commands~linking-files:/challenge$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:/challenge$ /home/hacker/not-the-flag
-bash: /home/hacker/not-the-flag: Permission denied
hacker@commands~linking-files:/challenge$ file ~/not-the-flag
/home/hacker/not-the-flag: symbolic link to /flag
hacker@commands~linking-files:/challenge$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{Qfduj8LqOIk7qgyXtPpl0WbQBeQ.QX5ETN1wSO1gjNzEzW}
hacker@commands~linking-files:/challenge$ 

```

## What i learnt
how to make symbolic links to already existing files

## references
none.
