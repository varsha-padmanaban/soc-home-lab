# Attack 3 — Backdoor User Creation

## Details
- Tool: Windows CMD
- Target: Local Windows PC
- MITRE: T1136.001 + T1098

## Commands Used
net user hacker P@ssw0rd123 /add
net localgroup administrators hacker /add
net user hacker /delete

## Detection
- Custom Rule 100001 fired (Level 12)
- Custom Rule 100002 fired (Level 14)
- Both rules written by me in XML

## Jira Ticket
INC-003 — Closed — Critical