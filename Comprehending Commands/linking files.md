# Linking Files
I created a symbolic link that points `/home/hacker/not-the-flag` to `/flag`. This way, when `/challenge/catflag` tries to read `/home/hacker/not-the-flag`, it will actually follow the symlink and read `/flag` instead
```bash
hacker@commands~linking-files:~$ ln -s /flag /home/hacker/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{8zHQJhR1E_mBgY9KgZXVMfiEk_k.dlTM1UDL2AjN0czW}
```
Resource used was the pwn website.
