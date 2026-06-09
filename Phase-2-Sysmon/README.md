### \# Phase 2 - Sysmon Deployment



\## Objective



Deploy Sysmon on the Windows 10 virtual machine to improve visibility into system activity and generate detailed logs for threat hunting.



\## Tools Used



\* Windows 10

\* Sysmon

\* Event Viewer



\## Installation Process



1\. Downloaded Sysmon from Microsoft Sysinternals.

2\. Downloaded a Sysmon configuration file.

3\. Installed Sysmon using the configuration.

4\. Verified that the Sysmon service started successfully.



\## Verification



Sysmon events were successfully generated and observed in:



Applications and Services Logs → Microsoft → Windows → Sysmon → Operational



Process creation events (Event ID 1) were successfully logged and reviewed.



\## Screenshots



Screenshots related to installation and verification are stored in the screenshots folder.



\## Outcome



Sysmon was successfully deployed and configured. The lab now generates detailed endpoint telemetry that will be used for future threat hunting and attack simulation exercises.





### \## **Testing**



\### Nmap Scan



An Nmap scan was executed from the Kali Linux VM against the Windows 10 VM.



Source IP: 192.168.56.102



Target IP: 192.168.56.105



\### Results



The scan completed successfully and connectivity between the systems was confirmed.



Sysmon generated endpoint telemetry during testing. No Sysmon event was found that directly identified the Nmap scan, indicating that additional network-focused logging or detection tools will be required for reconnaissance detection.



\### Lesson Learned



Sysmon is effective for endpoint visibility, but network reconnaissance detection requires additional telemetry sources such as firewall logs, Wazuh, Zeek, or Suricata.





