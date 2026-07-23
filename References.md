# References

This project was built using publicly available security frameworks, documentation, and tooling. The following resources were referenced throughout the implementation, configuration, and validation of the detection engineering workflow.

---

## MITRE ATT&CK Framework

The MITRE ATT&CK framework was used to select adversary techniques, map detections, and document ATT&CK IDs throughout this project.

- https://attack.mitre.org/

---

## Atomic Red Team

Atomic Red Team was used to safely simulate adversary techniques on the Windows endpoint for detection validation.

- https://github.com/redcanaryco/atomic-red-team
- https://atomicredteam.io/

---

## Sysmon

Microsoft Sysmon was used to generate endpoint telemetry, including process creation events and other Windows activity.

- https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon

---

## Splunk Enterprise

Splunk Enterprise was used to ingest Sysmon telemetry, develop SPL detection queries, and validate detections.

- https://www.splunk.com/
- https://docs.splunk.com/

---

## Splunk Search Processing Language (SPL)

Official SPL documentation used for query syntax and search commands.

- https://docs.splunk.com/Documentation/Splunk/latest/SearchReference/SearchReference

---

## Splunk Universal Forwarder

The Splunk Universal Forwarder was used to collect Sysmon logs from the Windows endpoint and forward them to Splunk Enterprise.

- https://www.splunk.com/en_us/download/universal-forwarder.html

---

## Windows Event Logging

Microsoft Windows Event Logging documentation used to understand Windows event collection and telemetry.

- https://learn.microsoft.com/en-us/windows/security/

---

## Sysinternals Suite

Microsoft Sysinternals tools and documentation.

- https://learn.microsoft.com/en-us/sysinternals/

---

## Microsoft Windows Documentation

Official Microsoft documentation referenced for Windows commands and endpoint behavior.

- https://learn.microsoft.com/en-us/windows/

---

## Acknowledgements

This project was developed as a hands-on detection engineering exercise to better understand adversary emulation, endpoint telemetry, and SIEM-based detection validation using industry-standard defensive security tools.
