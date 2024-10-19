# Adding Commands
Using `nano` command I created a shell script called `win` and then inside it I wrote the following commands: `#!/bin/bash` and `cat /flag`. The first command tells the file to use the `bash` interpreter to execute the file and the second command reads the flag. After giving permissions to execute the script, I updated the location of the `win.sh` script in the `PATH` variable. Running, `/challenge/run ` after that gave me the flag.
```
hacker@path~adding-commands:~$ nano /home/hacker/win
hacker@path~adding-commands:~$ chmod u+x /home/hacker/win
hacker@path~adding-commands:~$ export PATH=/home/hacker/:$PATH
hacker@path~adding-commands:~$ /challenge/run
Invoking 'win'....
pwn.college{wGpZ9gYHOkigki_ugplz5i46kAD.dZzNyUDL2AjN0czW}
```
Resource used was the pwn website.
