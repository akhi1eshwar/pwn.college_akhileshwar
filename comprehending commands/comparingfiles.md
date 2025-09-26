# Comparing Files
### this challenge asks you to differentiate between two files in the same directory

**Flag** 'pwn.college{oZylgOVhnBz61UF24gOtpWywe8M.01MwMDOxwSO1gjNzEzW}'

in this challenge i had to first cd to /challenge. from there i used the diff command to differentiate between two files decoys_only.txt and decoys_and_real.txt
one file contained the flag, which i used to get through the diff command.

```
hacker@commands~comparing-files:~$ cd /challenge
hacker@commands~comparing-files:/challenge$ diff decoys_only.txt decoys_and_real.txt
80a81
> pwn.college{oZylgOVhnBz61UF24gOtpWywe8M.01MwMDOxwSO1gjNzEzW}
```

## What I learnt

i learnt that diff compares two files line by line and tells you what the differences are. for example in the code snippet we see that there is "80a81"
which means that the second file has an additional line after 80th line. "after line80 of file1, add line81 of file2"
the line81 contained the flag.

## References
none
