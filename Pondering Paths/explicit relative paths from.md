# Explicit relative paths, from /
First I changed the directory to `/` using the `cd` command and then put a relative path to access the flag.

```bash
hacker@paths~explicit-relative-paths-from-:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{s0Ux2JakGeVoe2tMFFsXQlH3Sev.dBTN1QDL2AjN0czW}
```
Resource used was the pwn website.
