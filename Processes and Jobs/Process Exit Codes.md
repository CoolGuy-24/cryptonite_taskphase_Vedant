# Process Exit Codes
I ran the `/challenge/get-code` program and then read its exit code through `echo $?` and used that code as an argument for the `/challenge/submit-code` command to get the flag.
```bash
hacker@processes~process-exit-codes:~$ /challenge/get-code
Exiting with an error code!
hacker@processes~process-exit-codes:~$ echo $?
240
hacker@processes~process-exit-codes:~$ /challenge/submit-code 240
CORRECT! Here is your flag:
pwn.college{AFeO_9pAxJjWnHBXMGPmKP1QD9g.dljN4UDL2AjN0czW}
```
Resource used was the pwn website.
