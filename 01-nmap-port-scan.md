# Attack 1 — Nmap Port Scan

## Details
- Tool: Nmap
- Source: Kali Linux WSL2 (172.26.81.241)
- Target: Windows PC (172.26.80.1)
- MITRE: T1046 — Network Service Scanning

## Command Used
nmap -sV -A -T4 172.26.80.1

## Detection
- Wazuh Rule 40101 fired
- Multiple alerts generated within seconds

## Jira Ticket
INC-001 — Closed