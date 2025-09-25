# Implicit Relative Paths 

### using . to implicitly tell the system that we want that command run in the directory 
**Flag** 'pwn.college{skxT-3hNNmTmjfQYMO0VJ3eP_Md.QXxUTN0wSO1gjNzEzW}'

in this challenge, i had to use cd command to change directories to challenge and after that i used run but with ./ to implicitly tell the computer that i want to execute the program. 
otherwise it would simply tell that the command was not found. this is becuase it is a "naked" path.

'''
hacker@paths ~ implicit-relative-path:~ $ cd /challenge
hacker@paths ~ implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{skxT-3hNNmTmjfQYMO0VJ3eP_Md.QXxUTN0wSO1gjNzEzW}
hacker@paths ~ implicit-relative-path:/challenge$ 
'''

## What i learnt
this challenge teaches that if we use a naked path, the system could use the programs with the same name in the core directory. the computer doesn't run the program as a safety measure
and we are required to use the ./ to tell the computer that we want to execute the program

## References
none used.
