---
description: |
  The openssl s_client command implements a generic SSL/TLS client which connects to a remote host using SSL/TLS. It is a very useful diagnostic tool for SSL servers.

  Command Reference:

  	Target: 10.0.0.1

      Port: 21

command: |
  openssl s_client -connect 10.0.0.1:21 -starttls ftp
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
  - https://www.openssl.org/docs/manmaster/man1/openssl-s_client.html
---
