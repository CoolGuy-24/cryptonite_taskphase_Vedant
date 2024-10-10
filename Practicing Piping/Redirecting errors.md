# Redirecting errors
Using the `1>` character I directed the outputs to `myflag` file and the errors were directed to `instructions` using `2>` . Using the cat command I read the `myflag` file to obtain the flag.
```bash
hacker@piping~redirecting-errors:~$ /challenge/run 1> myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{oE4NCqnxq6MaWURcsxqvRlUF5m6.ddjN1QDL2AjN0czW}
```
Resource used was the pwn website.
