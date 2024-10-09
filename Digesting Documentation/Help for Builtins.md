# Help for Builtins
Using the `help` command I figured out what what argument I need to give for the `challenge` command and that's how I obtained the flag.
```bash
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "sA25OMz0".
hacker@man~help-for-builtins:~$ challenge --secret sA25OMz0
Correct! Here is your flag!
pwn.college{sA25OMz0hte2c7JkAJSVH7Xz7qR.dRTM5QDL2AjN0czW}
```

Resource used was the pwn website.
