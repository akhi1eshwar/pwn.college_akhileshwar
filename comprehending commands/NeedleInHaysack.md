# grepping for a needle in haysack
### this challenge introduces us to the concept of grepping by text searching

**Flag** 'pwn.college{YFu6erZ5ROMUpSD2MMzI_S6pe8-.QX3EDO0wSO1gjNzEzW}'

i used the grep command with the SEARCH_STRING. the search string was "pwn.college" as all of the flags start with that.
after the pwn.college string i just added the absolute path of the file i wanted to search the string from which was /challenge/data.txt
the command brought the flag to me.

```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn.college /challenge/data.txt
pwn.college{YFu6erZ5ROMUpSD2MMzI_S6pe8-.QX3EDO0wSO1gjNzEzW}
```

## What i learnt
i learnt how to use grep command. sometimes files that we are looking for are too big for cat, that is why we use the grep command to search for what we need.

## References
none
