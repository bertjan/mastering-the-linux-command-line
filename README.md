# mastering-the-linux-command-line
Material for presentation "Mastering the Linux command line".


Opening slides
---

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
- System administration
- Shell scripting
- Questions


Introduction
---
- What’s Linux?
- Kernel vs Distro
- Terminal session vs shell
- File system structure (folders, dot file)

Navigating
---
- pwd
- cd, ls, cd -  
- Tab completion  
- mkdir, mkdir -p
- touch
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
- ln
- touch
- type
- file
- diff
- tar, gzip, bzip
- vi


Networking
---
- Ssh, Ssh keys, ssh-copy-id, ssh tunneling
- ifconfig
- ping
- scp, sftp
- telnet
- traceroute, host  
- curl, wget
- nc
- telnet (telnet towel.blinkenlights.nl)
- redir
- ifconfig  
- rsync

Productivity
---
- cal
- bc
- Profile / .bash_profile
- aliases
- diff
- ctrl-a ctrl-e ctrl-l ctrl-d
- Env vars, functions, export
- More, less, shift-f
- screen
- zcat, zless 
- man -h —help
- Ctrl-z, bg fg
- Brace expansion
- Watch

Pipes
---
- cat,  cut, grep
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
- pstree
- top
- strace
- vmstat
- netstat
- lsof
- du en df
- Which process uses: this file, this port
- dd if=/dev/urandom | bzip2 -9 >> /dev/null

System administration
---
- sudo vs su
- apt / yum
- permissions, chmod, chown
- wall
- rc.local & startup scripts

Shell scripting
---
- hashbang / shebang
- variables
- If/then/else
- functions - function test1 { echo test; }
- command line args
- Bats: Bash Automated Testing System

Bonus
---
- What's this:  `:(){ :|:& };:`

Questions?
---
Hit me!
