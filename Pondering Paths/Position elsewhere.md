# Position elsewhere
Same as the previous task, I figured out the directory in which the flag is stored and hence accessed it by specifying its absolute path after changing my directory using the `cd` command.
```bash
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the / directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /
hacker@paths~position-elsewhere:/$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{4YFYexWNzsho4Hij2hdmUE1dLSM.ddDN1QDL2AjN0czW}
```
Resource used was the pwn website.
