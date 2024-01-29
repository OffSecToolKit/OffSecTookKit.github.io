---
description: |
  dig (domain information groper) is a flexible tool for interrogating DNS name servers. The following command will perform an NS request to the specified nameserver.

  Command Reference:

  	Domain: test.local

    Nameserver IP: 10.10.10.1

command: |
  dig ns test.local @10.10.10.1
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
  - https://linux.die.net/man/1/dig
---
