# SOC Attack Detection & Incident Response using Microsoft Sentinel

## Objective
To build a cloud-based SIEM lab using Microsoft Sentinel and detect real-world attack scenarios such as brute-force login attempts.

## Architecture
- Windows Virtual Machine
- Azure Log Analytics Workspace
- Microsoft Sentinel (SIEM)

Security event logs from the Windows VM are ingested into Sentinel for detection and investigation.

## Attack Simulated
- Multiple failed login attempts (Brute Force)
- Generated Windows Security Event ID 4625

## Detection Logic
A KQL query was created to detect multiple failed login attempts within a short time window.

## Incident Investigation
- Analyzed source IP address and targeted account
- Reviewed authentication patterns
- Mapped activity to MITRE ATT&CK technique T1110 (Brute Force)

## Tools Used
- Microsoft Sentinel
- Azure Monitor
- KQL
- Windows Security Event Logs

## Learnings
- Hands-on experience with SIEM log ingestion
- Writing detection rules using KQL
- Understanding SOC alert triage and investigation workflow
