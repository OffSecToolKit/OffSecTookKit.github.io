---
description: |
  Smbclient is a tool used to communicate with SMB servers. The following command will connect to an SMB share `public` using anonymous login.

  Command Reference:

  	Target IP: 10.10.10.1

  	SMB Share: public

command: |
  smbclient ////10.10.10.1//public -N
items:
  - No_Creds
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
