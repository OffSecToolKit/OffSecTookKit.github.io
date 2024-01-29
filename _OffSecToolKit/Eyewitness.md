---
description: |
  EyeWitness is designed to take screenshots of websites, provide some server header info, and identify default credentials if possible. The following command takes screenshots of the target websites.

  Command Reference:

      Target: https://test.local

command: |
  eyewitness.py -f urls.txt --single https://test.local
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
  - https://github.com/RedSiege/EyeWitness
---
