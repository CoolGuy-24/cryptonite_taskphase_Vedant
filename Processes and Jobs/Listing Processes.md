# Listing Processes
I used the `ps aux` command & argument to list down the processes currently running and found the filename and ran it to get the flag.
```bash
hacker@processes~listing-processes:~$ ps aux
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.3  0.0   1056   640 ?        Ss   10:44   0:00 /sbin/docker-init -- /nix/var/nix/profiles/default/bin/dojo-init
root           7  0.0  0.0   5052  2240 ?        S    10:44   0:00 /run/dojo/bin/sleep 6h
root          69  0.0  0.0   4132  2560 ?        S    10:44   0:00 /challenge/31464-run-5856
root          73  0.0  0.0   2744  1600 ?        S    10:44   0:00 sleep 6h
hacker        74  0.5  0.0   5376  3840 pts/0    Ss   10:44   0:00 /run/dojo/bin/ssh-entrypoint
hacker        91  0.0  0.0   7868  3520 pts/0    R+   10:44   0:00 ps aux
hacker@processes~listing-processes:~$ /challenge/31464-run-5856
Yahaha, you found me! Here is your flag:
pwn.college{kJCQFdUI3qGiXsVZdB0OUcpa4B1.dhzM4QDL2AjN0czW}
Now I will sleep for a while (so that you could find me with 'ps').
```
Resource used was the pwn website.
