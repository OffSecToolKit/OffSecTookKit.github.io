---
description: |
  Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The following command performs subdomain bruteforcing.

  Command Reference:

      Nameserver IP: 10.10.10.1

      Domain: test.local

      Output file: found_subdomains.txt

      Subdomains wordlist: ~/subdomains.list

command: |
  dnsenum --dnsserver 10.10.10.1 --enum -p 0 -s 0 -o found_subdomains.txt -f ~/subdomains.list test.local
items:
  - No_Creds
services:
  - DNS
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://github.com/SparrowOchon/dnsenum2
  - https://www.kali.org/tools/dnsenum/
---
