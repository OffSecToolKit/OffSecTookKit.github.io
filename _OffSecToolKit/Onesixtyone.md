---
description: |
  Onesixtyone is a fast SNMP scanner. The following command will bruteforce community strings of the SNMP service.

  Command Reference:

      Community strings wordlist: community-strings.list

      IP: 10.10.10.1

command: |
  onesixtyone -c community-strings.list 10.10.10.1
items:
  - No_Creds
services:
  - SNMP
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://github.com/trailofbits/onesixtyone
---
