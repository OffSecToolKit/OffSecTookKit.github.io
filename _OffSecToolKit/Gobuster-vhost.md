---
description: |
  Gobuster is a Directory/File, DNS and VHost busting tool written in Go. The following command performs bruteforcing on virtual hosts.

  Command Reference:

      Mode: VHOST

      Target: 10.10.10.1

      VHOST wordlist: /usr/share/wordlists/seclists/Discovery/DNS/fierce-hostlist.txt

command: |
  gobuster vhost -u 10.10.10.1 -w /usr/share/wordlists/seclists/Discovery/DNS/fierce-hostlist.txt
items:
  - No_Creds
services:
  - Web
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://github.com/OJ/gobuster
---
