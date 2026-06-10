#### \# Phase 3 - Wazuh Deployment \& Monitoring



\## Objective



Deploy Wazuh SIEM and establish centralized monitoring across the Home SOC Lab environment.



\## Technologies Used



\* Wazuh 4.14.5

\* Sysmon

\* Windows 10 vm

\* Kali Linux

\* VirtualBox

\* windows host





##### \## Lab Architecture



Windows Endpoint → Wazuh Agent → Wazuh Server → Dashboard



\## Progress



##### \### Infrastructure



\* Imported and configured the Wazuh OVA appliance.

\* Configured NAT and Host-Only networking.

\* Verified communication between lab systems.

\* Accessed and configured the Wazuh dashboard.

\* Established API connectivity.



##### \### Endpoint Monitoring



\* Installed and configured the Wazuh agent on the Windows endpoint.

\* Connected the endpoint to the Wazuh manager.

\* Verified agent communication.

\* Confirmed event ingestion into the dashboard.



##### \## Current Results



\* Centralized monitoring operational.

\* Windows endpoint successfully connected.

\* Security events visible in Wazuh.

\* Environment ready for detection and threat hunting activities.



##### \## Ongoing Work



\* PowerShell Monitoring

\* Threat Hunting

\* Event Analysis

\* Detection Rule Validation

\* Attack Simulation Testing



###### \## Screenshots



\### Wazuh Dashboard



!\[Dashboard](samples/wazuh-dashboard.png)



\### Connected Endpoint

&#x20;   (samples/wazuh-started.png)



!### Security Events



!\[Event Detection](samples/event-detected.png)



\## Notes



This phase is currently in progress and will continue to be updated as additional detections, alerts, and monitoring scenarios are implemented.



