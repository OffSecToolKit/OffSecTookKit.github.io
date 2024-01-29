---
description: |
  The openssl s_client command implements a generic SSL/TLS client which connects to a remote host using SSL/TLS. It is a very useful diagnostic tool for SSL servers. The following command will connect to the POP3S service.

  Command Reference:

      IP: 10.10.10.1

      Protocol: pop3s

command: |
  openssl s_client -connect 10.10.10.1:pop3s
items:
  - No_Creds
services:
  - POP3
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://www.openssl.org/docs/manmaster/man1/openssl-s_client.html
  - https://www.plesk.com/kb/support/how-to-verify-that-ssl-for-imap-pop3-smtp-works-and-a-proper-ssl-certificate-is-in-use/
---
