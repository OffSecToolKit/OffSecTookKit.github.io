---
description: |
  Gobuster is a Directory/File, DNS and VHost busting tool written in Go. The following command performs bruteforcing on subdomains.

  Command Reference:

    Mode: DNS

    Nameserver IP: 10.10.10.1

    Domain: test.local

    Subdomain wordlist: /usr/share/wordlists/seclists/Discovery/DNS/fierce-hostlist.txt

    Pattern file: patterns.txt

    Output file: output.txt

command: |
  gobuster dns -q -r 10.10.10.1 -d test.local -w /usr/share/wordlists/seclists/Discovery/DNS/fierce-hostlist.txt -p ./patterns.txt -o output.txt
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
