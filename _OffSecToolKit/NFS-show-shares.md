---
description: |
  Showmount queries the mount daemon on a remote host for information about the state of the NFS server on that machine. The following command returns the available NFS shares on a target.

  Command Reference:

  	Target: 10.10.10.1

command: |
  showmount -e 10.10.10.1
items:
  - Username
  - Password
services:
  - NFS
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://linux.die.net/man/8/showmount
---
