# MITRE ATT&CK Purple Team Detection Pipeline
Purple team detection engineering project using Atomic Red Team, Sysmon and Splunk to simulate MITRE ATT&amp;CK techniques and validate endpoint detections.

## Architecture
<img width="2048" height="2011" alt="image" src="https://github.com/user-attachments/assets/093e142d-7dd7-44fe-9192-dd51ad42088d" />

## Detection Workflow

1. Simulate adversary techniques using Atomic Red Team.
2. Capture endpoint telemetry with Sysmon.
3. Forward logs to Splunk Enterprise using the Universal Forwarder.
4. Develop SPL detection queries.
5. Validate detections against generated telemetry.
6. Map detections to MITRE ATT&CK techniques.

## Overview

This project demonstrates an end-to-end purple team detection engineering workflow using Atomic Red Team, Sysmon, and Splunk Enterprise. MITRE ATT&CK techniques were executed on a Windows 11 endpoint to simulate adversary behaviour, while Sysmon captured endpoint telemetry that was forwarded to Splunk for analysis.

Custom SPL detection queries were developed and validated against the generated Sysmon telemetry to detect simulated adversary activity. Each detection was mapped to the corresponding MITRE ATT&CK technique, demonstrating how adversary emulation can be used to improve defensive visibility and detection capabilities.


## Why I Built This

The purpose of this project was to gain practical experience in detection engineering beyond theoretical knowledge. Rather than only studying MITRE ATT&CK techniques, I wanted to simulate real attacker behaviour, understand the telemetry produced on a Windows endpoint, and develop validated detections within a SIEM.

This project demonstrates the complete detection engineering lifecycle from adversary simulation and telemetry collection to detection development, validation, and MITRE ATT&CK mapping.

## MITRE ATT&CK Coverage

| Technique | Description |
|-----------|-------------|
| [T1059.001 – PowerShell](T1059.001-PowerShell.md) | Command and Scripting Interpreter: PowerShell |
| [T1082 – System Information Discovery](T1082-System-Information-Discovery.md) | System Information Discovery |
| [T1033 – System Owner/User Discovery](T1033-System-Owner-User-Discovery.md) | System Owner/User Discovery |
| [T1057 – Process Discovery](T1057-Process-Discovery.md) | Process Discovery |
| [T1016 – System Network Configuration Discovery](T1016-System-Network-Configuration-Discovery.md) | System Network Configuration Discovery |

## Skills Demonstrated

- Detection Engineering
- Purple Team Methodology
- MITRE ATT&CK Mapping
- Splunk Enterprise (SPL)
- Sysmon Configuration & Telemetry Analysis
- Atomic Red Team Adversary Simulation
- Windows Endpoint Monitoring

## Lessons Learned

- Built and validated SPL detections using Sysmon process creation telemetry.
- Learned to manually extract XML fields using `rex` when the Sysmon Technology Add-on did not automatically parse events.
- Validated detections against generated telemetry rather than relying solely on query results.
- Improved understanding of Windows process creation, parent-child relationships, and MITRE ATT&CK mapping.

- Log Analysis & Event Correlation
- Threat Detection Validation
