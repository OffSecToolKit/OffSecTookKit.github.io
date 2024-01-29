---
description: |
  The mount command serves to attach the filesystem found on some device to the big file tree. The following command creates a directory and mounts the target NFS share to the newly created directory.

  Command Reference:

  	Target: 10.10.10.1

    Share: public

command: |
  mkdir target-NFS
  sudo mount -t nfs 10.10.10.1:/public ./target-NFS/ -o nolock
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
  - https://linux.die.net/man/8/mount
---
