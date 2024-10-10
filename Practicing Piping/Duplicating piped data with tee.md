# Duplicating piped data with tee
I used `tee` to store the output in `cm1_0` and then preat the output of the `/challenge/pwn` command and figured out how to use the command to get the flag. I passed the output to `/challenge/college` and then got the flag.
```bash
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee cm1_o | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat cm1_o
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "0Mywu9Jm"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 0Mywu9Jm | tee cm1_o | /challenge/college
Processing...
WARNING: you are overwriting file cm1_o with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{0Mywu9Jm-FZSZ0ih_n7fXWXjKXb.dFjM5QDL2AjN0czW}
```
Resource used was the pwn website.
