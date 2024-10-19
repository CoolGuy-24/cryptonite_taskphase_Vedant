# Redirecting Script Output
Using `nano` I created a shell called `x.sh` and inside it used the commands `/challenge/pwn;/challenge/college` and then piped its output to `/challenge/solve` using the `|` character.
```bash
hacker@chaining~redirecting-script-output:~$ nano x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{U4oMNw9g5TylF3fqMz5kMYGLA-r.dhTM5QDL2AjN0czW}
```
Resource used was pwn website.
