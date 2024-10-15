# Changing File Ownership
I used the `ls-1` command to first list out all the files and the permissions associated with them. Then using the `chown` command I transferrred the ownership of the `flag` file to `hacker` and finally read the flag using `cat` command.
```bash
hacker@permissions~changing-file-ownership:~$ ls -l
total 40
-rw-r--r-- 1 hacker hacker   4 Oct 10 12:25  COLLEGE
-rw-r--r-- 1 hacker hacker   8 Oct 10 12:40  PWN
-rw-r--r-- 1 root   hacker   0 Oct 10 13:18  SECRET_ARG
-rw-r--r-- 1 root   hacker  77 Oct 10 13:21  cm1_0
-rw-r--r-- 1 root   hacker  17 Oct 10 13:27  cm1_o
-rw-r--r-- 1 root   hacker   0 Oct 10 13:25  cm1_output
-rw-r--r-- 1 root   hacker   0 Oct 10 13:09  cmd1_output
lrwxrwxrwx 1 hacker hacker   5 Oct  2 16:37  flag -> /flag
-rw-r--r-- 1 hacker hacker 829 Oct 10 12:35  instructions
-rw-r--r-- 1 hacker hacker  93 Oct 10 12:35  myflag
lrwxrwxrwx 1 hacker hacker   5 Oct  3 15:14  not-the-flag -> /flag
lrwxrwxrwx 1 hacker hacker   4 Oct  2 16:49  ourfile -> flag
-rw-r--r-- 1 root   hacker   0 Oct 10 13:05  output
-rw-r--r-- 1 root   hacker  77 Oct 10 13:03  pwn_output
-rw-r--r-- 1 root   hacker   0 Oct 10 13:06  result
-rw-r--r-- 1 root   hacker  77 Oct 10 13:24  temp_output
-rw-r--r-- 1 hacker hacker 435 Oct 10 12:31  the-flag
-rw-r--r-- 1 root   hacker  58 Oct  2 10:44 '~'
hacker@permissions~changing-file-ownership:~$ chown hacker flag
hacker@permissions~changing-file-ownership:~$ cat flag
pwn.college{8lUcqKGV0hAw6q7l_Sm0wNCnTiA.dFTM2QDL2AjN0czW}
```
Resource used was the pwn website.
