# Exclusionary globbing
I used the `cd` command to go to the necessary directory and then used the glob `[!pwn]*` as the files were not supposed to begin with p,w or n.
```bash
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{ALtuRRAiWOhTPTSNNI9yhXf2Z_K.dZjM4QDL2AjN0czW}\
```
Resource used was the pwn website.
