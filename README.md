# Building a SOC Honeynet in Azure Live Traffic  (Live Traffic)
---
![CYBERSECURITY_LAB8](https://github.com/user-attachments/assets/d651f3be-ec3c-40a6-a5c9-d644b6728e63)
---
# Introduction

In this project, I build a mini honeynet in Azure and ingest logs from various resources into a Log Analytics Workspace, which is then used by Microsoft Sentinel to build attack maps, trigger alerts, and create incidents. I measured some security metrics in the insecure environment for 24 hours, applied security controls to harden the environment, measured metrics for another 24 hours, and then shared the results below. The metrics we will collect are:

- SecurityEvent (Windows Event Logs)
- Syslog (Linux Event Logs)
- SecurityAlert (Log Analytics Alerts Triggered)
- SecurityIncident (Incidents created by Sentinel)
- AzureNetworkAnalytics_CL (Malicious Flows allowed into our honeynet)
# Architecture Before Hardening / Security Controls
---
![322926658-efa182b3-afe3-46d6-b431-84fe61c1daff](https://github.com/user-attachments/assets/ccf16eef-010d-4cad-9fb8-b0368d427c42)

# Architecture After Hardening / Security Controls
---
![322926807-bda2d085-3471-4d51-8373-404e5dbd3371](https://github.com/user-attachments/assets/860205d6-649d-4358-85c3-08759355b5ac)

The architecture of the mini honeynet in Azure consists of the following components:

- Virtual Network (VNet)
- Network Security Group (NSG)
- Virtual Machines (2 windows, 1 linux)
- Log Analytics Workspace
- Azure Key Vault
- Azure Storage Account
- Microsoft Sentinel
  
# Attack Maps Before Hardening / Security Controls

<img width="986" alt="CYBERSECURITY_LAB14" src="https://github.com/user-attachments/assets/2f1edf85-0011-467f-9d84-0324600323f9" />




<img width="949" alt="CYBERSECURITY_LAB15" src="https://github.com/user-attachments/assets/59953863-7e7a-4e48-893f-cad9bf73eefb" />


<img width="1057" alt="CYBERSECURITY_LAB16" src="https://github.com/user-attachments/assets/eac5af4e-8664-453c-82d9-b788fb5893fc" />



