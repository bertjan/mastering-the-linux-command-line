# mastering-the-linux-command-line
Material for presentation "Mastering the Linux command line".  
Read along with `git clone https://github.com/bertjan/mastering-the-linux-command-line`

Opening slides
---

Title:
```
clear
printf "\n\n"; printf "Mastering\nthe\nLinux command line" | figlet -ctk; printf "\n\n"; printf '%0.1s' ' '{1..57} && printf "Bert Jan Schrijver\n\n" && printf '%0.1s' ' '{1..56} && printf "bertjan@openvalue.nl\n\n"
```

Profile picture:
```
jp2a https://pbs.twimg.com/profile_images/1056994211499786240/qqhVN-Ur_400x400.jpg
```

OpenValue logo:
```
wget -q -O - https://www.openvalue.nl/images/openvalue-white.png | convert - jpg:- | jp2a -
```

NLJUG logo:
```
jp2a https://yt3.ggpht.com/a/AGF-l79fDOsea1hkt8MMeKetvpDDE7qSlRfsKNaJQw=s288-mo-c-c0xffffffff-rj-k-no -i
```

Outline
---
- Introduction
- Navigating
- History
- File processing
- Networking
- Productivity
- Pipes
- System analysis
- Shell scripting
- Questions


Introduction
---
- What’s Linux?
- Kernel vs distro
- Terminal session vs shell

Navigating
---
- pwd
- cd, ls, cd -  
- File system structure (folders, dot file)
- Tab completion  
- find & find - exec
- locate

History
---
- up arrow
- history, !! and !<number>
- ctrl-r

File processing
---
- cp, mv, ln
- mkdir, mkdir -p
- type, which, file
- diff
- tar, gzip
- vi


Networking
---
- Ssh, Ssh keys, ssh-copy-id, ssh tunneling
```
ssh 192.168.1.32 -L8080:www.google.nl:80
wget -O - localhost:8080/ --header "Host: www.google.nl"
```
- ifconfig
- ping
- scp, sftp
- telnet
- wget / curl
- rsync

Productivity
---
- cal
- bc
- .profile / .bash_profile
- aliases
- ctrl-a ctrl-e ctrl-l ctrl-d ctrl-c
- env vars, export
- more, less
- screen
- zcat, zless 
- man -h —help
- Brace expansion
- Watch

Pipes
---
- cat, cut, grep
- xargs
- tee 
- for (…) 
- seq
- sort, uniq
- command substitution $(..)
- head, tail (-f)
- wc
- awk, sed
- ; & &&
- Output redirection > >> 2>&1

System analysis
---
- ps
- top (`dd if=/dev/urandom | bzip2 -9 >> /dev/null`)
- strace (`strace -p <vi pid> 2>&1 | grep read`)
- vmstat
- netstat
- lsof
- du en df

Shell scripting
---
- intro
- variables
- If/then/else
- functions (`function test1 { echo test; }`)
- Command line args

Bonus
---
- Bats: Bash Automated Testing System
- telnet towel.blinkenlights.nl
- What's this:  `:(){ :|:& };:`

Questions?
---
Hit me!
