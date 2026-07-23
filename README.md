# mitre-attack-purple-team-detection-pipeline
Purple team detection engineering project using Atomic Red Team, Sysmon and Splunk to simulate MITRE ATT&amp;CK techniques and validate endpoint detections.

# MITRE ATT&CK Purple Team Detection Pipeline

## Overview

This project demonstrates an end-to-end purple team detection engineering workflow using Atomic Red Team, Sysmon, and Splunk Enterprise. MITRE ATT&CK techniques were executed on a Windows 11 endpoint to simulate adversary behaviour, while Sysmon captured endpoint telemetry that was forwarded to Splunk for analysis.

Custom SPL detection queries were developed and validated against the generated Sysmon telemetry to detect simulated adversary activity. Each detection was mapped to the corresponding MITRE ATT&CK technique, demonstrating how adversary emulation can be used to improve defensive visibility and detection capabilities.


## Why I Built This

The purpose of this project was to gain practical experience in detection engineering beyond theoretical knowledge. Rather than only studying MITRE ATT&CK techniques, I wanted to simulate real attacker behaviour, understand the telemetry produced on a Windows endpoint, and develop validated detections within a SIEM.

This project demonstrates the complete detection engineering lifecycle from adversary simulation and telemetry collection to detection development, validation, and MITRE ATT&CK mapping.

## Skills Demonstrated

- Detection Engineering
- Purple Team Methodology
- MITRE ATT&CK Mapping
- Splunk Enterprise (SPL)
- Sysmon Configuration & Telemetry Analysis
- Atomic Red Team Adversary Simulation
- Windows Endpoint Monitoring
- Log Analysis & Event Correlation
- Threat Detection Validation
