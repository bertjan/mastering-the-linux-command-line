# mastering-the-linux-command-line
Material for talk "Mastering the Linux command line".  
Read along with `git clone https://github.com/bertjan/mastering-the-linux-command-line`

Opening slides
---

Title:
```
clear
printf "\n\n"; printf "Mastering\nthe\nLinux command line" | figlet -ctk; printf "\n\n"; printf '%0.1s' ' '{1..57} && printf "Bert Jan Schrijver\n\n" && printf '%0.1s' ' '{1..56} && printf "bertjan@openvalue.nl\n\n"
```

Intro:

```
(jp2a https://pbs.twimg.com/profile_images/1056994211499786240/qqhVN-Ur_400x400.jpg \
&& echo && echo \
&& wget -q -O - https://www.openvalue.nl/images/openvalue-white.png | convert - jpg:- | jp2a - \
&& echo && echo \
&& jp2a https://yt3.ggpht.com/a/AGF-l79fDOsea1hkt8MMeKetvpDDE7qSlRfsKNaJQw=s288-mo-c-c0xffffffff-rj-k-no -i) | less
```




Introduction
---
Assumption: you know the basics like `cd`, `ls`, `cp`, `mv`.

- Terminal session, shell, bash
- man, help, -h, --help
- pipes: intro

Navigating
---
- pwd
- cd -  
- tab completion  
- find
- locate

History
---
- up arrow
- history, !! and !<number>
- ctrl-r

File processing
---
- which, file
- diff
- vi

Networking
---
- ssh key authentication, ssh-copy-id, ssh tunneling
- ifconfig
- ping
- scp, sftp
- rsync
- telnet
- curl

Productivity
---
- cal
- bc
- .profile
- aliases
- ctrl-a ctrl-e ctrl-l ctrl-d ctrl-c
- less shift-g shift-f
- brace expansion
- screen
- watch

Pipes
---
- cat, grep, awk, cut
- sort, uniq
- tee 
- seq
- command substitution $(..)
- head, tail (-f)
- wc
- sed
- ; vs &&
- Output redirection > >> 2>&1

System analysis
---
- ps
- top (`dd if=/dev/urandom | bzip2 -9 >> /dev/null`)
- strace (`strace -p <vi pid> 2>&1 | grep read`)
- vmstat
- netstat
- lsof
- du 

Shell scripting
---
- intro, make executable
- variables
- Command line args
- If/then/else
- functions (`function test1 { echo test; }`)


Bonus
---
- Bats: Bash Automated Testing System
- What's this:  `:(){ :|:& };:`
- telnet towel.blinkenlights.nl

Questions?
---
Hit me!

Thanks!
---
'Slides' are at https://github.com/bertjan.
