# Writing to multiple programs
`/challenge/hack` command generates the output, `tee` command duplicates the output it receives, `>(/challenge/the)` part uses process substitution to send the output of tee to `/challenge/the` as its input.
`| /challenge/planet` part pipes the output of tee directly to /challenge/planet
```bash
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >( /challenge/the ) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{kESTrIQBVw5J5FkTspXbSK-HR9v.dBDO0UDL2AjN0czW}
```
Resource used was the pwn website.
