# Position thy self
Initially, I tried to access the flag by trying to access the challenge directory but it was stored under the `/usr/include` directory so I used the `cd` commmand to change my directory and then accessed the flag.
```bash
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/include directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/include
hacker@paths~position-thy-self:/usr/include$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{g-tBCRphMoasiatQeM8YUaSQ47c.dZDN1QDL2AjN0czW}
```

Resource used was the pwn webiste.
