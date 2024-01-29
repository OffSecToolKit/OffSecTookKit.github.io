---
description: |
  Smbclient is a tool used to communicate with SMB servers. The following command will list out all available shares on the target server using anonymous login.

  Command Reference:

  	Target: 10.10.10.1

command: |
  smbclient -N -L //10.10.10.1
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
---
