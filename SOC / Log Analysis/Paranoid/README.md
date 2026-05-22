
# Paranoid – Linux Audit Log Analysis

## Overview
Analysis of a Linux audit log to investigate a system compromise — Blue Team Labs Online.

## Tools Used
- Kali Linux
- aureport / auditd
- Linux CLI

## Key Findings

### Initial Access
- Brute Force SSH attack — 87 failed logins before successful login
- Compromised account: **btlo**
- Attacker IP: **192.168.4.155**

### Enumeration
- Attacker used **linpeas** for system enumeration
- Disguised as pulseaudio process

### Privilege Escalation
- Exploited **CVE-2021-3156** (Baron Samedit)
- Heap-based Buffer Overflow in sudo
- Custom binary **evil** compiled on target machine to gain root

### Exfiltration & Cleanup
- **/etc/shadow** exfiltrated after root access
- Attacker removed all files to cover tracks
- But **aureport saw everything** 👀

## MITRE ATT&CK Mapping
| Technique | ID |
|-----------|-----|
| Brute Force | T1110.001 |
| File and Directory Discovery | T1083 |
| Exploitation for Privilege Escalation | T1068 |
| Credentials from Password Files | T1552.003 |

## BTLO Profile
https://blueteamlabs.online/achievement/share/challenge/155436/30

<img width="630" height="479" alt="image" src="https://github.com/user-attachments/assets/2459af0b-6810-4276-a154-fe663c36e9aa" />

