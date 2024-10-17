# Other users with su
Using the `su` command and specifying the user `zardus` in the argument and providing the appropriate password I was able to switch users and then get the flag by running `/challenge/run`.
```bash
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{IsM9CxglQvJy-mtDaM3YX2vijja.dZTN0UDL2AjN0czW}
```
Resource used was the pwn website
