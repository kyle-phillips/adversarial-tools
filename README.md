# adversarial-tools

This is a working list of tools that would potentially be used by adversaries in a cyber attack.  

The creation of this list was born out of a desire to know if certain executables are being used within a network that would not normally be seen or not normally ran by a user account.  

The intent of this project is to provide a list of EXE names (and possibly file hashes one day) that can be used for querying logs as a threat hunting activity.  

Information for this list gained from various sources.

Please check this list for LOL bins, or Mitre's Software list for additional information.


Executable    | Description   | Used For    | MITRE ATT@ACK  |  
| ----------- | -----------   | ----------- | -----------    |  
|   7za.exe   | Compression app (command line) | Sometimes used for malicious activity. Also commonly used for legitimate activity, therefore, not effective for threat hunting | https://attack.mitre.org/techniques/T1027/ |  
| adFind.exe    | Command line Active Directory tool | Used to enumerate domain users, groups, organizational units, etc. | https://attack.mitre.org/techniques/T1087  https://attack.mitre.org/techniques/T1482 https://attack.mitre.org/techniques/T1069 https://attack.mitre.org/techniques/T1018 https://attack.mitre.org/techniques/T1016    |
| arp.exe | Display info about Address Resolution Protocol | Commonly used by Windows OS, mostly under "machine" account type. User use is unusual. | |
| eqnedt.exe | Microsoft Equation Editor | | | 
| mimikatz.exe | Credential dumper | Execution likely to be noticed by EDR | numerous |  
| ngrok.exe | Scan/recon for a network | Network and host discovery | https://attack.mitre.org/techniques/T1046  https://attack.mitre.org/techniques/T1040  https://attack.mitre.org/techniques/T1018  https://attack.mitre.org/techniques/T1016  https://attack.mitre.org/techniques/T1033  |
| nbtscan.exe | Scan/recon for a network | Network and host discovery | |
| netscan.exe | Scan/recon for a network | Network and host discovery | |
| netstat.exe | View network connections for a local host | Not useful for threat hunting because used for too many legit purposes |
| nmap.exe | Network mapper | Network discovery, host discovery, open ports, etc. | |
