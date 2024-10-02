# Position yet elsewhere

Same as the previous task, I figured out the directory in which the flag is stored and hence accessed it by specifying its absolute path after changing my directory using the `cd` command.

```bash
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/doc directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /usr/share/doc
hacker@paths~position-yet-elsewhere:/usr/share/doc$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{o5CiPNb58CsUth_kZAXi9d1KLDk.dhDN1QDL2AjN0czW}
```
Resource used was the pwn website. 
