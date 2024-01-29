---
description: |
  The umount command detaches the file system(s) mentioned from the file hierarchy. The following command unmounts the specified NFS share.

  Command Reference:

  	Target: 10.10.10.1

    Share: public

command: |
  umount ./target-NFS
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
  - https://linux.die.net/man/8/umount
---
