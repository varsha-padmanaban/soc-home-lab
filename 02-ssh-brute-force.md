# Attack 2 — SSH Brute Force

## Details
- Tool: Hydra
- Source: Kali Linux WSL2
- Target: Wazuh VM (192.168.56.101) port 22
- MITRE: T1110.001 — Password Guessing

## Command Used
hydra -l root -P /usr/share/wordlists/rockyou.txt ssh://192.168.56.101 -t 4 -V

## Detection
- Wazuh Rule 5763 fired
- 100+ alerts in under 2 minutes
- Alert Level: 10 (High)

## Jira Ticket
INC-002 — Closed