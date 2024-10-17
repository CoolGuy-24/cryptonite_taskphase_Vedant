# Changing Permissions
Using the `ls -l` command I read the permissions of the `/flag` file. The `chmod` command allowed me to change the permissions of the `/flag`file and using the argument of `o+r` I gave other users read access and then finally using the `cat` command I read the flag.
```bash
hacker@permissions~changing-permissions:~$ ls -l /flag
-r-------- 1 root root 58 Oct 17 07:43 /flag
hacker@permissions~changing-permissions:~$ chmod o+r /flag
hacker@permissions~changing-permissions:~$ cat flag
pwn.college{4gmXfR2rQQy9y0grbhWPR3TI9eg.dNzNyUDL2AjN0czW}
```
Resource used was the pwn website.
