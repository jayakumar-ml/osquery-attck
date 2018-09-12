# Osquery-ATT&CK

The goal of this repository is to try to map the MITRE ATT&CK with the Osquery for enterprise threat hunting.

Each conf file is a Query Pack that can be used enterprise threat hunting wit osquery. 

The folder **osquery-minimal-conf** contain a minimal subset of the conf files in the home directory.

Mapping the MITRE ATT&CK Matrix with Osquery


I try to create Osquery pack that can cover some elements of the ATT&CK
## Query Pack Descriprion

- **windows-registry-monitoring.conf** : Track all the change in the **registry** for malware persistency. The registry path are the path that can be find here:
    https://attack.mitre.org/wiki/Persistence. A second article that explain some presistency method https://www.countercept.com/our-thinking/hunting-for-application-shim-databases
- **windows-incorrect_parent_process.conf** : This check verify if some attackers or malware try to execute a legitim process in a malicious way

##  ATT&CK MAPPING
- **windows-registry-monitoring.conf**
    - ATT&CK T1015,T1138,T1131,T1037,T1128,T1060,T1180,T1004,T1058,T1103,T1112