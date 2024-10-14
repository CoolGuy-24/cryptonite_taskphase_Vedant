# Resuming Processes
I ran the `/challenge/run` command, then suspended it using `Ctrl+Z` and resumed it using the `fg` command.
```bash
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{M9fzwXq2WZV_TY5NTcXtGMSXJ5t.dZDN4QDL2AjN0czW}
Don't forget to press Enter to quit me!

Goodbye!
```
Resource used was the pwn website.
