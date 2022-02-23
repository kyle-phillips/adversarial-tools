# adversarial-tools

This is a working list of tools used by adversaries in a cyber attack.  The intent of this project is to provide a list of EXE names (and possibly file hashes one day) that can be used for querying logs as a threat hunting activity.  

These are not necessarily Living Off the Land binaries.   

Check this list for LOLBINS.


Executable    | Description | Used For    | MITRE ATT@ACK  |  
| ----------- | ----------- | ----------- | -----------    |  
|   7za.exe   | Compression app (command line) | Sometimes used for malicious activity. Also commonly used for legitimate activity, therefore, not effective for threat hunting | https://attack.mitre.org/techniques/T1027/ |  
| AdFind.exe    | Command line Active Directory tool | Used to enumerate domain users, groups, organizational units, etc. | https://attack.mitre.org/techniques/T1087  https://attack.mitre.org/techniques/T1482 https://attack.mitre.org/techniques/T1069 https://attack.mitre.org/techniques/T1018 https://attack.mitre.org/techniques/T1016    |

