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





### \## **## Testing and Validation**

### 

**### Nmap Scan Test**



**To validate connectivity between the Kali Linux and Windows 10 virtual machines, an Nmap scan was performed from the Kali system against the Windows host.**



**\*\*Source System:\*\* Kali Linux**



**\*\*Source IP:\*\* 192.168.56.102**



**\*\*Target System:\*\* Windows 10**



**\*\*Target IP:\*\* 192.168.56.105**



**### Evidence**



**#### Nmap Scan Results**



**!\[Nmap Scan](screenshots/nmap-scan-results.png)**



**The scan completed successfully and confirmed communication between both systems on the Host-Only network.**



**#### Sysmon Operational Log**



**!\[Sysmon Operational Log](screenshots/sysmon-operational-log.png)**



**Sysmon successfully generated and stored endpoint telemetry in the Operational log.**



**#### Process Creation Event**



**!\[Process Create Event](screenshots/process-create-event.png)**



**Process creation events (Event ID 1) were successfully recorded, confirming that Sysmon monitoring is active.**



**### Findings**



**\* Communication between Kali Linux and Windows 10 was successfully established.**

**\* Sysmon was verified to be operational and collecting endpoint telemetry.**

**\* Process creation events were successfully logged and reviewed.**

**\* The Nmap scan itself did not generate a clearly identifiable Sysmon event, highlighting the need for additional network-focused monitoring solutions in future phases.**



**### Conclusion**



**Phase 2 successfully deployed and validated Sysmon within the Home SOC Lab environment. The Windows endpoint is now capable of generating enhanced telemetry that will be used for future detection engineering, threat hunting, and incident investigation exercises.**



