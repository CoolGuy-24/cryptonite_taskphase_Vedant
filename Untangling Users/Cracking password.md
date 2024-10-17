# Cracking passwords
Running the `John the Ripper` algorithm/program on the leaked file `/challenge/shadow-leak` I cracked the password and used that to switch users to `zardus` using `su` and finally got the flag by running `/challenge/run`
```bash
hacker@users~cracking-passwords:~$ john /challenge/shadow-leak
Loaded 1 password hash (crypt, generic crypt(3) [?/64])
Press 'q' or Ctrl-C to abort, almost any other key for status
aardvark         (zardus)
1g 0:00:00:21 100% 2/3 0.04668g/s 271.8p/s 271.8c/s 271.8C/s Johnson..buzz
Use the "--show" option to display all of the cracked passwords reliably
Session completed
hacker@users~cracking-passwords:~$ su zardus
Password:
zardus@users~cracking-passwords:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{8SBclrFMu1ibbl0vU9w-LrACEZC.ddTN0UDL2AjN0czW}
```
Resource used was the pwn wesbite.
