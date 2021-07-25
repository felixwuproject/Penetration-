# Penetration-

All the useful tool and common lines

Nmap Tool
## Scan In the command below:

-sn – is the type of scan, which means a ping scan. By default, Nmap performs port scanning, **but this scan will disable port scanning.**
10.42.0.0/24 – is the target network, replace it with your actual network.   nmap -sn 192.168.1.1/24

TCP SYN (Stealth) Scan (-sS) SYN scan is the default and most popular scan option for good reason. It can be performed quickly, scanning thousands of ports per second on a fast network not hampered by intrusive firewalls. SYN scan is relatively unobtrusive and stealthy, since it never completes TCP connections. It also works against any compliant TCP stack rather than depending on idiosyncrasies of specific platforms **-T4 More faster scan** nmap -sS -T4 192.168.1.1

