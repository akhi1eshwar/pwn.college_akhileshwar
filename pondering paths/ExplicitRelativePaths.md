# Explicit Relative paths, from /
### we get to know what explicit relatives paths are and how to use them in this challenge

**Flag** 'pwn.college{oQURPbVP8D74-ybMgYY3s45FBx9.QXwUTN0wSO1gjNzEzW}'

in this challenge, i had to change the cwd to /, and after that i tried to do the challenge/run. of course that was correct but not how i was instructed to go through with the task.
i retried using ./challenge/run and the program run and i got the flag.

'''
hacker@paths ~ explicit-relative-paths-from-:~$ cd /
hacker@paths ~ explicit-relative-paths-from-:/$ challenge/run
Incorrect...
This challenge must be called with a relative path that explicitly starts with a `.`!
hacker@paths ~ explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oQURPbVP8D74-ybMgYY3s45FBx9.QXwUTN0wSO1gjNzEzW}
'''

## What i learnt
What an explicit relative path is. by using the . or .. before the slash we can tell the terminal where exactly we want to access the file from.
if we are working on a file in folder 1 in abc directory but we need another file from folder 2 in the same directory, we can access the file without changin pathways using the '.'.
this reduces a lot of typing and saves time.

## References used
google search on better understanding of the . and .. functions.
