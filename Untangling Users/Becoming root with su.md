# Becoming root with su
I used the `su` command to switch users and provided the appropriate password to get access and then using `cat` I read the flag.
```bash
hacker@users~becoming-root-with-su:~$ su
Password:
root@users~becoming-root-with-su:/home/hacker# cat flag
pwn.college{sE54s6G-8UE4Ei4LbgwT6g_pyk6.dVTN0UDL2AjN0czW}
```
Resource used was the pwn website.
