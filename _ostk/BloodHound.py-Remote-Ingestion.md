---
description: |
  BloodHound is a monolithic web application composed of an embedded React frontend with Sigma.js and a Go based REST API backend. It is deployed with a Postgresql application database and a Neo4j graph database, and is fed by the SharpHound and AzureHound data collectors.

  BloodHound uses graph theory to reveal the hidden and often unintended relationships within an Active Directory or Azure environment. Attackers can use BloodHound to easily identify highly complex attack paths that would otherwise be impossible to quickly identify. Defenders can use BloodHound to identify and eliminate those same attack paths. Both blue and red teams can use BloodHound to easily gain a deeper understanding of privilege relationships in an Active Directory or Azure environment.

  BloodHound.py is a Python based ingestor for BloodHound, based on Impacket. It allows you to remotely collect data for bloodhound by querying LDAP

  Command Reference:

  	Target IP: 10.10.10.1

  	Domain: test.local

command: |
  bloodhound.py -d test.local -v --zip -c All -dc test.local -ns 10.10.10.1
items:
  - No_Creds
services:
  - LDAP
phases:
  - Enumeration
OS:
  - Linux
  - Windows
references:
  - https://github.com/SpecterOps/BloodHound
  - https://github.com/dirkjanm/BloodHound.py/tree/bloodhound-ce
---
