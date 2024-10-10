# Exporting variables
I set the `PWN` variable and `COLLEGE` variable to their apporpriate values and then also exported the `PWN` variable using `export`. By using the `sh` command I invoked another shell inside my shell and excuted the `/challenge/run` command to obtain the flag.

```bash
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{42TXbcRyajSLE8m7bTUs1NC0IgV.dJjN1QDL2AjN0czW}
```
Resource used was pwn website.
