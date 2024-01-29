---
description: |
  The telnet command is used to communicate with another host using the TELNET protocol. The following command will connect to the target SMTP server.

  Command Reference:

    Target: 10.10.10.1

    Port: 25

command: |
  telnet 10.10.10.1 25
items:
  - No_Creds
services:
  - SMTP
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://linux.die.net/man/1/telnet
---
