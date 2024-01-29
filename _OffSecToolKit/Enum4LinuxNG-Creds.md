---
description: |
  enum4linux-ng.py is a rewrite of Mark Lowe's (former Portcullis Labs now Cisco CX Security Labs) enum4linux.pl, a tool for enumerating information from Windows and Samba systems, aimed for security professionals and CTF players. The tool is mainly a wrapper around the Samba tools nmblookup, net, rpcclient and smbclient. The following command will attempt to enumerate information provided valid login credentials.

  Command Reference:

  	Target IP: 10.10.10.1

  	Username: john

  	Password: password123

command: |
  enum4linux-ng.py -u john -p password123 -a 10.10.10.1
items:
  - Username
  - Password
phases:
  - Enumeration
OS:
  - Linux
references:
  - https://github.com/cddmp/enum4linux-ng
---
