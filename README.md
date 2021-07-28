# Penetration-

All the useful tool and common lines

Nmap Tool
## Scan In the command below:

-sn – is the type of scan, which means a ping scan. By default, Nmap performs port scanning, **but this scan will disable port scanning.**
10.42.0.0/24 – is the target network, replace it with your actual network.   nmap -sn 192.168.1.1/24

TCP SYN (Stealth) Scan (-sS) SYN scan is the default and most popular scan option for good reason. It can be performed quickly, scanning thousands of ports per second on a fast network not hampered by intrusive firewalls. SYN scan is relatively unobtrusive and stealthy, since it never completes TCP connections. It also works against any compliant TCP stack rather than depending on idiosyncrasies of specific platforms **-T4 More faster scan** nmap -sS -T4 192.168.1.1

Nikto Tool
## Scan web server scanner which performs comprehensive tests against web servers for multiple items, including over 6700 potentially dangerous files/programs,
nikto -C all - host http:// 


Hydra
The next tool we will use is Hydra, a powerful login cracker which is very fast and supports a number of different protocols. To show the help and some basic usage options, simply type hydra in the terminal. 
hydra -L users.txt -P passwords.txt ssh://IP -t 4
The -L flag, which specifies a list of login names.
The -P flag, which specifies a list of passwords.
ssh://172.16.1.102 — our target and protocol.
The -t flag set to 4, which sets the number of parallel tasks to run.

hydra -l <username> -P /usr/share/wordlists/rockyou.txt -s 22 -f -vV <ip> ssh
