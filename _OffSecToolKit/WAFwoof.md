---
description: |
  WAFW00F allows one to identify and fingerprint Web Application Firewall (WAF) products protecting a website. The following command identifies the WAFs protecting a site.

  Command Reference:

    Target: https://test.local

command: |
  wafw00f -v https://test.local
items:
  - No_Creds
services:
  - Web
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://github.com/EnableSecurity/wafw00f
---
