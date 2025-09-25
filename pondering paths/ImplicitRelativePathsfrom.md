# Implicit relative paths, from /
### in this challenge, we use relative paths to reach the required program

**Flag** 'pwn.college{4oXF8lgXR59k5zpardOWYMTmwgP.QX5QTN0wSO1gjNzEzW}'

in this program i tried to do the /challenge/run but it told me that i was in the incorrect current working directory "cwd"
i switched the cwd to / using cd
after that i used a relative path challenge/run (notice there is no '/' before challenge)
and from that i got the flag.

'''
hacker@paths ~ implicit-relative-paths-from-:/$ cd /
hacker@paths ~ implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{4oXF8lgXR59k5zpardOWYMTmwgP.QX5QTN0wSO1gjNzEzW}
'''

## What i learnt
i learnt what relative paths are and why cwd's are important to be in to use relative paths. using absolute paths by /, we could access the directory or program from anywhere.
this doesn't happen in relative paths and we need to be in correct directory. 
if a cwd is / the relative path goes something like xyz/abc and we wont need to use the / befere xyz becaue the terminal already knows what directory we currently are in.

## References
none used.
