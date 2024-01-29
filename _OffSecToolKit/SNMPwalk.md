---
description: |
  snmpwalk is an SNMP application that uses SNMP GETNEXT requests to query a network entity for a tree of information. The following command will query for object identifiers(OIDs).

  Command Reference:

  	Community string: public

    IP: 10.10.10.1

command: |
  snmpwalk -v2c -c public 10.10.10.1
items:
  - No_Creds
services:
  - SNMP
OS:
  - Linux
  - Windows
phases:
  - Enumeration
references:
  - https://linux.die.net/man/1/dig
---
