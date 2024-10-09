# Helpful Programs
In this task, I used the `--help` argument for the `/challenge/challenge` program, which provided options like `-p` to print the value for the flag and `-g` to retrieve it. I successfully followed these commands to obtain the hidden flag.
```bash
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge --p
The secret value is: 233
hacker@man~helpful-programs:~$ /challenge/challenge --g 233
Correct usage! Your flag: pwn.college{gZr-kqZKvOkWtjPL2KFS3bpJW3_.ddjM4QDL2AjN0czW}
```

Resource used was the pwn website.
