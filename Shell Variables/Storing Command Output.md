# Storing Command Output
Using a command substiution of `$(/challenge/run)` I stored the output in the `PWN` variable then using the `echo` command I read the flag.
```bash
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{U2JBkbcOaHWJkVgXdE4M6rRD_5m.dVzN0UDL2AjN0czW}
```
Resource used was the pwn website.
