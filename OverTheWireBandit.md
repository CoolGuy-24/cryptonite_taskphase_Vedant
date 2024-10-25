# Level 0
I established a SSH connection to the website and entered the passowrd to gain access to the game.

![image](https://github.com/user-attachments/assets/dfce7c3d-5a55-4460-9db6-51da56d0aedc)

# Level 0-->1
I simply used the `cat` commmand to read the file `readme` and then used the password that I got to log onto the next level.

![image](https://github.com/user-attachments/assets/19db71cd-c4a7-4d98-bf92-103d60fc3eff)
![image](https://github.com/user-attachments/assets/d66490ad-c8dc-462e-9645-2c5cdf97adbd)

# Level 1-->2
By specifying the absolute path of the file I was able to read it and obtain the password.

![image](https://github.com/user-attachments/assets/43353a5a-0e12-4c38-bb0a-0066a74c1960)
![image](https://github.com/user-attachments/assets/162d8cc9-4cba-448e-863c-fe11229e0606)

# Level 2-->3
I understood and learnt that whenever there are spaces in a file name we should wrap the file number under double quotes and then use the `cat` command.

![image](https://github.com/user-attachments/assets/41aee1c4-f452-4c9e-96ed-d56c6dfee9ce)
![image](https://github.com/user-attachments/assets/a46809c8-e9e0-47c1-8208-ff5322101c8e)

# Level 3-->4
I switched to the `inhere` directory. 
Then used the `ls` command with the `-a` argument to view the hidden files.
Read the file using the `cat` command to obtain the password to the next level.

![image](https://github.com/user-attachments/assets/e2a88e3a-aecc-4ca0-b746-4b045f3ed447)
![image](https://github.com/user-attachments/assets/6e780c33-e929-4918-9b8b-86e5b2827ef6)

# Level 4-->5
Using the `cd` command I switched directories.
Then using `ls` command I viewed the files.
Since all file names started with `-` I knew we had to specify the absolute path when reading them.
I used `file` command with `*` (file globbing) to check the data type of each file and then I read `-file07`

![image](https://github.com/user-attachments/assets/cfb4b3d4-790a-42ce-82ca-9ee5c53b61a8)
![image](https://github.com/user-attachments/assets/89364dee-f90a-4956-a0f6-08bd304e7409)

# Level 5-->6
I know we had to use different arguments with the `find` command but I was nto sure which ones to use.
So using `find --help` I got the necessary arguments and with a bit of online searching I was able to come up with the command `find . -type f -size 1033c -readable ! -executable` which gave me the location of the file which I then simply `cat`

![image](https://github.com/user-attachments/assets/d00b9141-5c98-47f2-b389-101c7cb534b8)
![image](https://github.com/user-attachments/assets/53f2b529-d282-40eb-9103-5bc0788398cc)

# Level 6-->7
I used a similar technique to find the place of the password and this time used the command `find / -group bandit6 -user bandit7 -size 33c` and then I got a whole list of errors but looking closely I found the place of the passowrd and then used `cat`

![image](https://github.com/user-attachments/assets/ed9dc5a4-6ca8-4163-8779-f2edad3d7150)
![image](https://github.com/user-attachments/assets/591e9dab-9471-47a7-993c-95bde0b58140)
![image](https://github.com/user-attachments/assets/5aea67b8-6835-4606-a7e7-6c5d25488081)
