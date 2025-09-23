# Intro to Arguments
### We are asked to use commands with areguments to retrieve the flag

**Flag** 'pwn.college{ABsq_GMndGzjhpgTSQH4z8lPjjX.QX4YjM1wSO1gjNzEzW}'

in this challenge we are asked to only use "hello hackers" command but i made the mistake of using echo before the hello hackers portion.
because of that mistake i couldn't get the flag, and instead the terminal responded with "hello hackers"
i re read the instructions and by using the argument hello hackers i got the flag

```
hacker@hello~intro-to-arguments:~$ echo hello hackers!
hello hackers!
hacker@hello~intro-to-arguments:~$ hello hackers
Success! Here is your flag:
pwn.college{ABsq_GMndGzjhpgTSQH4z8lPjjX.QX4YjM1wSO1gjNzEzW}
hacker@hello~intro-to-arguments:~$ 
```

##What i learned
in this challenge i learnt how to use commands with arguments. this just data added to the command which the shell responds to.
the first word is the command and subsequent the argument

using "echo", the terminal simply gives back or "echoes" out the arguement back.

## References
