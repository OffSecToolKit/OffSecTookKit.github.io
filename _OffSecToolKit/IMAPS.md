---
description: |
  The openssl s_client command implements a generic SSL/TLS client which connects to a remote host using SSL/TLS. It is a very useful diagnostic tool for SSL servers. The following command will connect to the IMAPS service.

  Command Reference:

      IP: 10.10.10.1

      Protocol: imaps

command: |
  openssl s_client -connect 10.10.10.1:imaps
items:
  - No_Creds
services:
  - IMAP
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://www.openssl.org/docs/manmaster/man1/openssl-s_client.html
  - https://tewarid.github.io/2011/05/10/access-imap-server-from-the-command-line-using-openssl.html
---
