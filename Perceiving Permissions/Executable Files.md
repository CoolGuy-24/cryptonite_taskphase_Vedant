# Executable Files
Using the `ls -l` function I figured out that the `hacker` user (i.e is me) only had access to read the programa dn not excuete it so then using the `chmod` command and the `u+x` argument I changed the permissions and than ran the program to get the flag.
```bash
hacker@permissions~executable-files:~$ ls -l /challenge/run
-r--r--r-x 1 hacker hacker 32 Jul  4 06:37 /challenge/run
hacker@permissions~executable-files:~$ chmod u+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{4cPgz4RAVlXGB-qYWtUoW5DXf3p.dJTM2QDL2AjN0czW}
```
Resource used was the pwn website.
