# help for builtins
### this challenge dives further into using commands around man, --help etc

**flag** 'pwn.college{MoINBRP8eTvwhVjav2StPmsT4UJ.QX0ETO0wSO1gjNzEzW}'

in this challenge i first used help and after that i found the builtin for challenge which was challenge only
to expand it, i used help challenge to get all the arguments for challenge
after that i used the argument to get the flag.


```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!
    
    Options:
      --fortune		display a fortune
      --version		display the version
      --secret VALUE	prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "MoINBRP8".
hacker@man~help-for-builtins:~$ challenge --secret MoINBRP8
Correct! Here is your flag!
pwn.college{MoINBRP8eTvwhVjav2StPmsT4UJ.QX0ETO0wSO1gjNzEzW}

hacker@man~help-for-builtins:~$ 
```

## what i learnt
how to use the help built in

## references 
none

```
