# Attack 4 — File Integrity Violation

## Details
- Tool: PowerShell
- File: C:\Windows\System32\drivers\etc\hosts
- MITRE: T1565 — Data Manipulation

## Command Used
Add-Content -Path 'C:\Windows\System32\drivers\etc\hosts' -Value '# TEST FIM ALERT - SOC LAB'

## Detection
- Wazuh FIM Rule 550 fired
- MD5 checksum change detected
- Alert within 60 seconds

## Jira Ticket
INC-004 — Closed