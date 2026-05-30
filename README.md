# soc-home-lab
# SOC Home Lab — Wazuh Threat Detection Project

![Status](https://img.shields.io/badge/Phase_1-Complete-brightgreen)
![Tool](https://img.shields.io/badge/Tool-Wazuh_SIEM-blue)
![Cost](https://img.shields.io/badge/Cost-Free-success)
![RAM](https://img.shields.io/badge/RAM-4GB_Optimised-orange)

## Overview
Built a SOC home lab using Wazuh SIEM/HIDS to monitor
a Windows endpoint, simulate real attacks from Kali Linux,
write custom detection rules, and manage incidents in Jira.

## Architecture
- Wazuh Manager (Ubuntu VM, 2GB RAM) — central SIEM
- Windows PC with Wazuh Agent — monitored endpoint
- Kali Linux WSL2 — attack simulation

## Attacks Simulated
| # | Attack | Tool | MITRE | Detected |
|---|--------|------|-------|----------|
| 1 | Port Scan | Nmap | T1046 | Rule 40101 ✅ |
| 2 | SSH Brute Force | Hydra | T1110 | Rule 5763 ✅ |
| 3 | Backdoor User | CMD | T1136.001 | Custom Rule 100001 ✅ |
| 4 | File Integrity | PowerShell | T1565 | FIM Rule 550 ✅ |

## Custom Rules Written
- Rule 100001 (Level 12): New user account — T1136.001
- Rule 100002 (Level 14): Admin group change — T1098

## Incident Response
6 incidents tracked in Jira with full investigation
and remediation documented.

## Screenshots
All attack evidence in /screenshots folder.

## Skills Used
Wazuh | SIEM | HIDS | MITRE ATT&CK | Kali Linux |
Nmap | Hydra | Incident Response | Jira | Git | GitHub
