# Fun With Groups Names
I used the `ls-1` command to first list out all the files and the permissions associated with them. I figured out that the `grp9840` has access to `flag` symlink. Then using the `id` command I figured out that my group id is also `grp9840` but when I tried to run the `cat` flag command it didn't allow me to access it. So I viewed the group permissions for `/flag` and it showed `root`. So using the `chgrp` command I changed the group permissions and was then able to access the flag using the `cat` command.
```bash
hacker@permissions~fun-with-groups-names:~$ ls -l
total 40
-rw-r--r-- 1 hacker grp9840   4 Oct 10 12:25  COLLEGE
-rw-r--r-- 1 hacker grp9840   8 Oct 10 12:40  PWN
-rw-r--r-- 1 root   grp9840   0 Oct 10 13:18  SECRET_ARG
-rw-r--r-- 1 root   grp9840  77 Oct 10 13:21  cm1_0
-rw-r--r-- 1 root   grp9840  17 Oct 10 13:27  cm1_o
-rw-r--r-- 1 root   grp9840   0 Oct 10 13:25  cm1_output
-rw-r--r-- 1 root   grp9840   0 Oct 10 13:09  cmd1_output
lrwxrwxrwx 1 hacker grp9840   5 Oct  2 16:37  flag -> /flag
-rw-r--r-- 1 hacker grp9840 829 Oct 10 12:35  instructions
-rw-r--r-- 1 hacker grp9840  93 Oct 10 12:35  myflag
lrwxrwxrwx 1 hacker grp9840   5 Oct  3 15:14  not-the-flag -> /flag
lrwxrwxrwx 1 hacker grp9840   4 Oct  2 16:49  ourfile -> flag
-rw-r--r-- 1 root   grp9840   0 Oct 10 13:05  output
-rw-r--r-- 1 root   grp9840  77 Oct 10 13:03  pwn_output
-rw-r--r-- 1 root   grp9840   0 Oct 10 13:06  result
-rw-r--r-- 1 root   grp9840  77 Oct 10 13:24  temp_output
-rw-r--r-- 1 hacker grp9840 435 Oct 10 12:31  the-flag
-rw-r--r-- 1 root   grp9840  58 Oct  2 10:44 '~'
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp9840) groups=1000(grp9840)
hacker@permissions~fun-with-groups-names:~$ cat flag
cat: flag: Permission denied
hacker@permissions~fun-with-groups-names:~$ ls -l /flag
-r--r----- 1 root root 58 Oct 15 11:11 /flag
hacker@permissions~fun-with-groups-names:~$ chgrp grp9840 /flag
hacker@permissions~fun-with-groups-names:~$ cat flag
pwn.college{sWZG4OINMDoDHqFAyin1Sm65Uje.dJzNyUDL2AjN0czW}
```
Resource used was the pwn webiste.
