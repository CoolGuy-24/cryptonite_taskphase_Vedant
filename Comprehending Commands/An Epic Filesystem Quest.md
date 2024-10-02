# An Epic Filesystem Quest
First I went into the directory `/` using the `cd` command. Then I read the clues using the `cat` command.
The clues that were trapped couldn't be accessed by using the `cd` command so I used the `ls` command to view the files in it and select an appropriate file and using the `cat` command I read the file by putting the absolute path of the file after the `cat` command.
The clues that were delyaed required me to enter the directory so I entered the directory using the `cd` command.
The clues that were hidden required  me to use `ls -a` to view them. 
```bash
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
BRIEF  boot       dev  flag  lib    lib64   media  nix  proc  run   srv  tmp  var
bin    challenge  etc  home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~an-epic-filesystem-quest:/$ cat BRIEF
Lucky listing!
The next clue is in: /usr/share/racket/pkgs/redex-doc/redex/scribblings/ref

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/$ ls /usr/share/racket/pkgs/redex-doc/redex/scribblings/ref
NUGGET-TRAPPED                        gui.scrbl              reduction-relations.scrbl     typesetting.scrbl
common.rkt                            languages.scrbl        terms.scrbl
compiled                              other-relations.scrbl  testing.scrbl
dynamic-typesetting-and-macros.scrbl  patterns.scrbl         typesetting-and-macros.scrbl
hacker@commands~an-epic-filesystem-quest:/$ cat /usr/share/racket/pkgs/redex-doc/redex/scribblings/ref/NUGGET-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/share/zoneinfo/posix/Australia

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/$ cd /usr/share/zoneinfo/posix/Australia
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ ls
ACT       Brisbane     Canberra  Darwin  Hobart  Lindeman   Melbourne  North  Queensland  South   Tasmania  West
Adelaide  Broken_Hill  Currie    Eucla   LHI     Lord_Howe  NSW        Perth  README      Sydney  Victoria  Yancowinna
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ cat README
Congratulations, you found the clue!
The next clue is in: /opt/linux/linux-5.4/drivers/usb/musb

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ ls /opt/linux/linux-5.4/drivers/usb/musb
CLUE-TRAPPED  da8xx.c        musb_core.h     musb_gadget.c      musb_regs.h     omap2430.h       ux500_dma.c
Kconfig       davinci.c      musb_cppi41.c   musb_gadget.h      musb_trace.c    sunxi.c
Makefile      davinci.h      musb_debug.h    musb_gadget_ep0.c  musb_trace.h    tusb6010.c
am35x.c       jz4740.c       musb_debugfs.c  musb_host.c        musb_virthub.c  tusb6010.h
cppi_dma.c    musb_am335x.c  musb_dma.h      musb_host.h        musbhsdma.c     tusb6010_omap.c
cppi_dma.h    musb_core.c    musb_dsps.c     musb_io.h          omap2430.c      ux500.c
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ cat /opt/linux/linux-5.4/drivers/usb/musb/
CLUE-TRAPPED
Lucky listing!
The next clue is in: /usr/lib/debug/.build-id/24

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ ls /usr/lib/debug/.build-id/24
1c25696d2fe0ec49f6ef1e950d202ebb1ba8eb.debug  5265480bab195b493e8d062231aedb3f211d42.debug
4c5140c0521c81914afe5d92ad5ccc954857d5.debug  TIP-TRAPPED
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ cat /usr/lib/debug/.build-id/24/TIP-TRAPPED
Yahaha, you found me!
The next clue is in: /usr/share/perl5/Dpkg/Build

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ ls -a /usr/share/perl5/Dpkg/Build
.  ..  .LEAD  Env.pm  Info.pm  Types.pm
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ cat /usr/share/perl5/Dpkg/Build/.LEAD
Great sleuthing!
The next clue is in: /usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/File/Glob

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/share/zoneinfo/posix/Australia$ cd /usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/File/Glob
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/File/Glob$ ls -a
.  ..  .SECRET  Glob.so
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/File/Glob$ cat .SECRET
Great sleuthing!
The next clue is in: /usr/share/racket/pkgs/compatibility-doc
hacker@commands~an-epic-filesystem-quest:/usr/lib/x86_64-linux-gnu/perl/5.30.0/auto/File/Glob$ cd /usr/share/racket/pkgs/compatibility-doc
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/compatibility-doc$ ls
LICENSE.txt  MEMO  info.rkt  mzlib
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/compatibility-doc$ cat MEMO
Lucky listing!
The next clue is in: /opt/aflplusplus/.git/modules/nyx_mode/packer/logs/refs/heads
hacker@commands~an-epic-filesystem-quest:/usr/share/racket/pkgs/compatibility-doc$ cd /opt/aflplusplus/.git/modules/nyx_
mode/packer/logs/refs/heads
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/packer/logs/refs/heads$ ls
GIST  main
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/packer/logs/refs/heads$ cat main
0000000000000000000000000000000000000000 bcf3e248b660764f48af54232a3388389a2dfc22 root <root@buildkitsandbox.(none)> 1725641052 +0000   clone: from https://github.com/nyx-fuzz/packer.git
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/packer/logs/refs/heads$ ls -a
.  ..  GIST  main
hacker@commands~an-epic-filesystem-quest:/opt/aflplusplus/.git/modules/nyx_mode/packer/logs/refs/heads$ cat GIST
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{wZEothwGV-jL1H3Ii-mT9Q_yRTN.dljM4QDL2AjN0czW}
```
Resource used was the pwn website.
