# Reading Manuals
First I read the manual for the `challenge` command using the `man` command. From that I understood that I need to use the `--oyfcxx` argument with `935` as the argument to get the flag.
```bash
hacker@man~reading-manuals:~$ man challenge

CHALLENGE(1)                                           Challenge Commands                                          CHALLENGE(1)

NAME
       /challenge/challenge - print the flag!

SYNOPSIS
       challenge OPTION

DESCRIPTION
       Output the flag when called with the right arguments.

       --fortune
              read a fortune

       --version
              output version information and exit

       --oyfcxx NUM
              print the flag if NUM is 935

AUTHOR
       Written by Zardus.

REPORTING BUGS
       The repository for this dojo: <https://github.com/pwncollege/linux-luminarium/>

SEE ALSO
       man(1) bash-builtins(7)

pwn.college                                                 May 2024                                               CHALLENGE(1)
hacker@man~reading-manuals:~$ /challenge/challenge --oyfcxx 935
Correct usage! Your flag: pwn.college{IR9XB3oyfcxxB5rDDYw4-MvJ3pn.dRTM4QDL2AjN0czW}
```
Resource that was the pwn website.
