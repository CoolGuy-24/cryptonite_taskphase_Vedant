# Finding Files
First I searched the whole filesystem to find the directories which have `flag` in it. Then switched to the directories using the `ls` command and when I found the flag I read it using the `cat` command.

```bash
hacker@commands~finding-files:~$ find / -name flag
find: ‘/root’: Permission denied
find: ‘/proc/1/task/1/fd’: Permission denied
find: ‘/proc/1/task/1/fdinfo’: Permission denied
find: ‘/proc/1/task/1/ns’: Permission denied
find: ‘/proc/1/fd’: Permission denied
find: ‘/proc/1/map_files’: Permission denied
find: ‘/proc/1/fdinfo’: Permission denied
find: ‘/proc/1/ns’: Permission denied
find: ‘/proc/7/task/7/fd’: Permission denied
find: ‘/proc/7/task/7/fdinfo’: Permission denied
find: ‘/proc/7/task/7/ns’: Permission denied
find: ‘/proc/7/fd’: Permission denied
find: ‘/proc/7/map_files’: Permission denied
find: ‘/proc/7/fdinfo’: Permission denied
find: ‘/proc/7/ns’: Permission denied
find: ‘/var/log/private’: Permission denied
find: ‘/var/log/apache2’: Permission denied
find: ‘/var/log/mysql’: Permission denied
find: ‘/var/cache/ldconfig’: Permission denied
find: ‘/var/cache/apt/archives/partial’: Permission denied
find: ‘/var/cache/private’: Permission denied
find: ‘/var/lib/apt/lists/partial’: Permission denied
find: ‘/var/lib/php/sessions’: Permission denied
find: ‘/var/lib/mysql-files’: Permission denied
find: ‘/var/lib/private’: Permission denied
find: ‘/var/lib/mysql-keyring’: Permission denied
find: ‘/var/lib/mysql’: Permission denied
find: ‘/tmp/tmp.XvrUsDZh8M’: Permission denied
find: ‘/run/mysqld’: Permission denied
find: ‘/run/sudo’: Permission denied
find: ‘/etc/ssl/private’: Permission denied
/usr/local/lib/python3.8/dist-packages/pwnlib/flag
/usr/local/share/radare2/5.9.5/flag
/opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn/flag
/opt/pwndbg/.venv/lib/python3.8/site-packages/pwnlib/flag
/opt/radare2/libr/flag
/nix/store/pmvk2bk4p550w182rjfm529kfqddnvh3-python3.11-pwntools-4.12.0/lib/python3.11/site-packages/pwnlib/flag
/nix/store/1yagn5s8sf7kcs2hkccgf8d0wxlrv5sz-radare2-5.9.0/share/radare2/5.9.0/flag
hacker@commands~finding-files:~$ cd /usr/local/share/radare2/5.9.5/flag
hacker@commands~finding-files:/usr/local/share/radare2/5.9.5/flag$ ls
tags.r2
hacker@commands~finding-files:/usr/local/share/radare2/5.9.5/flag$ cd /opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn/flag
ssh-entrypoint: cd: /opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn/flag: Not a directory
hacker@commands~finding-files:/usr/local/share/radare2/5.9.5/flag$ cd /opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn
hacker@commands~finding-files:/opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn$ ls
flag  vcn_1_0_offset.h  vcn_1_0_sh_mask.h  vcn_2_0_0_offset.h  vcn_2_0_0_sh_mask.h  vcn_2_5_offset.h  vcn_2_5_sh_mask.h
hacker@commands~finding-files:/opt/linux/linux-5.4/drivers/gpu/drm/amd/include/asic_reg/vcn$ cat flag
pwn.college{kmduY4qJfsRiQ20PxeNAhVLyOGL.dJzM4QDL2AjN0czW}
```
Resource used was the pwn website.
