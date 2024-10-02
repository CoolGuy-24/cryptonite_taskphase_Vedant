# Hidden Files
I used the `cd` command to swtich to the `/` directory as the flag was there. Then using `ls -a` , I was able to view the hidden files and therefore the flag as well. FInally using the `cat` command I read the flag and accessed it.
```bash
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-100961957312907  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ cat .flag-100961957312907
pwn.college{wDO3VoLVMKC5ge0Wdfo7-IEj3wz.dBTN4QDL2AjN0czW}
```
Resource used was the pwn website.
