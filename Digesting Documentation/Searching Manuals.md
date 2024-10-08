# Searching Manuals
Reading the manual page for the `challenge` command using the `man` command made me find out what argument to use to print the flag. I searched for the apporpriate argument by using `/` and then typed `flag` and moved to the next result using the `n` key. I found the argumen `--lqn` and used it to get the flag.
```bash
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --lqn
Initializing...
Correct usage! Your flag: pwn.college{IlPYg7bkhHW-D9OmEMKb3mP7Y5x.dVTM4QDL2AjN0czW}
```
Resource that was used was the pwn website.
