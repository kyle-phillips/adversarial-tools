# adversarial-tools

This is a working list of tools that would potentially be used by adversaries in a cyber attack.  

The creation of this list was born out of a desire to know if certain executables are being used within a network that would not normally be seen or not normally ran by a user account.  

The intent of this project is to provide a list of EXE names (and possibly file hashes one day) that can be used for querying logs as a threat hunting activity.  

Information for this list gained from various sources.

Similiar resources to this one:  https://lolbas-project.github.io/,  
or Mitre's Software list for additional information, https://attack.mitre.org/techniques/T1518/001/

.  

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
| plink.exe | Command line SSH client (PuTTy link) | APT28, UNC757, UNC2448 | |
| psexec.exe | A free Microsoft tool that can be used to execute a program on another computer | | https://attack.mitre.org/techniques/T1136  https://attack.mitre.org/techniques/T1543  https://attack.mitre.org/techniques/T1570  https://attack.mitre.org/techniques/T1021  https://attack.mitre.org/techniques/T1569 | 
| putty.exe | SSH client | | | 
| radmin.exe | Remote software | Used by various threat actors for remote access | https://attack.mitre.org/techniques/T1072/ |
| rclone.exe | Command line tool - used to manage cloud storage | Darkside | |
| sharphound.exe | Active Directory collector for Bloodhound | https://bloodhound.readthedocs.io/en/latest/data-collection/sharphound.html | |
| vnc.exe | Remote desktop software | Common adversarial tool | https://attack.mitre.org/techniques/T1021/  https://attack.mitre.org/techniques/T1133/  https://attack.mitre.org/techniques/T1219/  |
| wmic.exe | Windows Management Instrumentation (command line) | Commonly used by machine accounts; threat hunting should focus on user activity | https://attack.mitre.org/techniques/T1047/  | 
 
