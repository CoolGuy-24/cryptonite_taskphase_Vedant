# Suspending Processes
I ran the `/challenge/run` program and then suspended it using the `Ctrl+Z` command. After running the `/challenge/run` command again I was able to obtain the flag.
```bash
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          83      65  0 10:57 pts/0    00:00:00 bash /challenge/run
root          85      83  0 10:57 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root          83      65  0 10:57 pts/0    00:00:00 bash /challenge/run
root          90      65  0 10:57 pts/0    00:00:00 bash /challenge/run
root          92      90  0 10:57 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{0nvT2R51RdQe3Plwt02DkAiQ_NW.dVDN4QDL2AjN0czW}
```
Resource used was the pwn website.
