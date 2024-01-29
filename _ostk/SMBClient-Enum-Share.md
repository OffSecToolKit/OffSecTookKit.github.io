---
description: |
  Smbclient is a tool used to communicate with SMB servers. The following command will connect to an SMB share `C$` using valid credentials.

  Command Reference:

  	Target IP: 10.10.10.1

  	SMB Share: public

  	Username: john

  	Password: password123

command: |
  smbclient ////10.10.10.1//public -U john password123
items:
  - Username
  - Password
services:
  - SMB
OS:
  - Linux
phases:
  - Enumeration
references:
  - https://www.samba.org/samba/docs/current/man-html/smbclient.1.html
  - https://www.madirish.net/59
---
