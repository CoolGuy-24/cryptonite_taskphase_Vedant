# Redirecting input
I sotred the word `COLLEGE ` into the `PWN` file using the `>` character and then put the input into the `/challenge/run` command using the `<` character. 
```bash
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{4WtgPlQZUxocJUN6p1nC--TIScO.dBzN1QDL2AjN0czW}
```
Resoruce used was the pwn website.
