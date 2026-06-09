\# Phase 2 - Sysmon Deployment



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



