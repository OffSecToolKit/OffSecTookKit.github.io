---
description: |
  Dirsearch is a web path scanner written in Python. The following command performs directory bruteforcing.

  Command Reference:

      Target: http://10.10.10.1

command: |
  dirsearch -u http://10.10.10.1
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
  - https://github.com/maurosoria/dirsearch
---
