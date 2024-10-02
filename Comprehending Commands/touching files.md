# Touching files
First I changed the directory to `tmp` using the `cd` command as I had to create the two blank files there. Using the `ls` command I checked for the files present and then using the `touch` command I created two blank files called `pwn` an `college`. Finally, I accessed the flag.
```bash
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  tmp.XvrUsDZh8M
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.XvrUsDZh8M
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{cqCW6AIV5_v3R4LWFLhwPwvKyDe.dBzM4QDL2AjN0czW}
```
Resource used was the pwn website.
