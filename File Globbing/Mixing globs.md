# Mixing globs
I changed the directory using the `cd` command and then using the glob `[cep]*` I targeted the files which began with c,e and p and have susbsequent characters after them.
```bash
hacker@globbing~mixing-globs:/challenge/files$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls [cep]*
challenging  educational  pwning
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{own5StSutNY7WqS27TwJRJw8Yf0.dVjM4QDL2AjN0czW}
```
Resource used was the pwn website.
