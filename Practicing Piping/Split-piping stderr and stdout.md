# Split-piping stderr and stdout
The `>` operator sends stdout to the process substitution `>( /challenge/planet )`, which allows `/challenge/planet` to read the output.
The `2>` operator sends stderr to the process substitution `>( /challenge/the )`, allowing `/challenge/the` to receive the error messages.
This keeps stdout and stderr separate, as required.
```bash
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{0EawuvDuJBo8s7vyYTL-z_BtIjj.dFDNwYDL2AjN0czW}
```
Resource used was the pwn website.
