# The SUID Bit
I viewed the permissions of the `challenge/getroot` program and added a suid bit to it using the `chmod` command and `u+s` argument and ran it again to get the `root` shell and then simply used `cat` to read the flag.
```bash
hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwxr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ ls -l /challenge/getroot
-rwsr-xr-x 1 root root 155 Jul 12 10:30 /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat flag
pwn.college{gFBXHbp2PkSL_h_78J61EBFdsWq.dNTM2QDL2AjN0czW}
```
Resource used was the pwn website
