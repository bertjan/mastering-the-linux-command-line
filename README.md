# mastering-the-linux-command-line
Material for talk "Mastering the Linux command line".  
Read along with `git clone https://github.com/bertjan/mastering-the-linux-command-line`

Opening slides
---

Title:
```
clear
printf "\n\n"; printf "Mastering\nthe\nLinux command line" | figlet -ctk; printf "\n\n"; printf '%0.1s' ' '{1..49} && printf "Bert Jan Schrijver\n\n" && printf '%0.1s' ' '{1..48} && printf "bertjan@openvalue.nl\n" && printf '%0.1s' ' '{1..52} && printf "@bjschrijver\n\n"
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
- tab completion  
- cd -  
- find
- locate
- which

History
---
- up arrow
- history, !! and !<number>
- ctrl-r

File processing
---
- file
- diff
- vi

Networking
---
- ssh key authentication, ssh-copy-id, ssh tunneling
- ifconfig
- ping
- telnet
- curl
- scp, sftp
- rsync

Productivity
---
- cal
- bc
- .profile
- aliases
- ctrl-a ctrl-e ctrl-l ctrl-d ctrl-c
- less shift-g shift-f
- brace expansion
- watch
- screen

Pipes
---
- tee
- head, tail (-f)
- cat, grep, awk, cut
- sort, uniq
(`cat demo-app.log | grep "Received \[GET " | awk {'print $11'} | sort | uniq -c`)
- command substitution $(..)
- wc
- sed
- ; vs &&
- Output redirection > >>

System analysis
---
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
Questions? @bjschrijver on Twitter.
