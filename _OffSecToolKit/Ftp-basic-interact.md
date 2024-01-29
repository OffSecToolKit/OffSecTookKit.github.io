---
description: |
  FTP (File Transfer Protocol) is a network protocol for transmitting files between computers over Transmission Control Protocol/Internet Protocol (TCP/IP) connections.

  Command Reference:

      Target: 10.0.0.1

command: |
  ftp 10.0.0.1
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
  - https://linux.die.net/man/1/ftp
---
