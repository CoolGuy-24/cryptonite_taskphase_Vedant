# Killing Processes
The `ps aux` command listed all the processes running and the `grep` command helped me search for the `/challenge/dont_run` program. Using the `kill` command I then terminated the process and ran `/challenge/run` to get the flag.
```bash
hacker@processes~killing-processes:~$ ps aux | grep /challenge/dont_run
hacker        73  0.0  0.0   4976  3200 ?        Ss   10:50   0:00 /challenge/dont_run
hacker        93  0.0  0.0   4140  2240 pts/0    S+   10:50   0:00 grep --color=auto /challenge/dont_run
hacker@processes~killing-processes:~$ kill 73
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{QWqqnRX7VJ3EQ0CD6ANPur1pn-c.dJDN4QDL2AjN0czW}
```
Resource used was the pwn wesbite.
