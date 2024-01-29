---
description: |
  Wget is a free utility for non-interactive download of files from the Web. It supports HTTP , HTTPS , and FTP protocols, as well as retrieval through HTTP proxies.

  Command Reference:

  	Enable recursion: -m

    Diable passive mode: --no-passive

    Service: ftp

    User & Password: anonymous:anonymous

    Target: 10.0.0.1

command: |
  wget -m --no-passive ftp://anonymous:anonymous@10.0.0.1
items:
  - No_Creds
  - Username
  - Password
services:
  - FTP
OS:
  - Linux
phases:
  - Enumeration
references:
  - https://linux.die.net/man/1/wget
---
