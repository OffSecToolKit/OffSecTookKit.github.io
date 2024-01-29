---
description: |
  IPMI (Intelligent Platform Management Interface) is a set of standardized specifications for hardware-based platform management systems that makes it possible to control and monitor servers centrally. The following command leverages the metasploit framework and will perform IPMI version detection.

command: |
  msfconsole
  use auxiliary/scanner/ipmi/ipmi_version
items:
  - No_Creds
services:
  - IPMI
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://github.com/rapid7/metasploit-framework/blob/master/documentation/modules/auxiliary/scanner/ipmi/ipmi_version.md
---
