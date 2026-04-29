# BlueTeam-Portfolio
Practical Blue Team investigations, incident response labs, and cybersecurity projects


# Blue Team Investigations & Cyber Defense Portfolio 🛡️

Welcome! I am a Cyber Security Analyst focused on incident response, cloud security, and automation. This repository documents my practical labs and security projects.

## 👤 Professional Profile
- **Location:** Ireland
- **Certifications:** 
  - ✅ CompTIA Security+
  - ✅ Microsoft Azure Fundamentals (AZ-900)
  - ✅ IT Specialist: Python
  - ⏳ CompTIA CySA+ (In Progress)


## 🔬 Practical Investigations (Blue Team Labs Online)



### 4. The Report II 📄  
Difficulty: Medium  

• **Tools:** MITRE Report (PDF), Web Browser  
• **Skills:** SOC Concepts, Incident Response Workflow, Threat Intelligence, Organizational Models, Log & Data Understanding  
• **Outcome:** Analyzed MITRE SOC report, identified key operational strategies, SOC structures, incident prioritization methods, and extracted actionable insights for improving SOC effectiveness.  

BTLO Profile: My Investigations & Badges:  
https://blueteamlabs.online/achievement/share/challenge/155436/44

______________________________________________________________________________________________________




7. Threat Report Analysis (SOC) 📊

Difficulty: Easy

• Tools: Threat Intelligence Reports, MITRE ATT&CK Framework, Web Research

• Skills: Threat Intelligence Analysis, Vulnerability Identification, MITRE Mapping, Ransomware TTPs, SOC Detection Use Cases

• Outcome: Analysed a 2022 threat report to extract actionable intelligence for SOC operations, identified major attacks such as Log4Shell, mapped techniques to MITRE ATT&CK, reviewed critical vulnerabilities (including Exchange exploits and zero-day RCE), analysed ransomware affiliate models (Conti), and defined detection and prevention measures (e.g., parent process monitoring, RDP hardening) to improve SOC readiness.

BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/42

______________________________________________________________________________________________________

8.🔍 Log Analysis: Sysmon (SOC)

Difficulty: Medium 🟠

🛠️ Tools: VS Code, JSON parsing, Sysmon logs
💡 Skills: Log Analysis, Threat Hunting, Incident Reconstruction, Privilege Escalation Detection, C2 Identification, MITRE ATT&CK Mapping

<img width="685" height="509" alt="Снимок экрана 2026-04-24 182308" src="https://github.com/user-attachments/assets/878f545e-552e-4d34-b0d6-a3f9255d12c9" />


🎯 Outcome:

Analysed Sysmon logs from a compromised endpoint to reconstruct a full attack chain:

📂 Identified initial access via a malicious updater.hta file executed by mshta.exe

💾 Tracked PowerShell Invoke-WebRequest activity used to download malware

📡 Identified C2 communication on port 6969

🔐 Detected privilege escalation via JuicyPotato

🔎 Uncovered a reverse shell established on port 9898 using nc.exe

🧠💥 Traced the full attack by manually analysing parent-child process relationships and CommandLines in VS Code.

It's all about connecting the dots!

<img width="1885" height="509" alt="Снимок экрана 2026-04-24 183359" src="https://github.com/user-attachments/assets/d3e2dc0f-c4c5-4368-ad7d-461a6de02894" />

BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/18

______________________________________________________________________________________________________

9. 🔍 Secrets — JWT Analysis (SOC)
    
Difficulty: Easy 🟢
🛠️ Tools: CyberChef, jwt.io, Hashcat
💡 Skills: JWT Analysis, Token Decoding, Privilege Escalation Detection, Secret Cracking, Token Forging

🎯 Outcome:

Analysed a suspicious JWT token to identify and fix a privilege escalation vulnerability:

🔐 Identified a high-privilege JWT token with admin: true

🧩 Decoded the token structure: Header.Payload.Signature

🕵️ Extracted a hidden hint from the payload: _4_Eyes

<img width="1916" height="883" alt="image" src="https://github.com/user-attachments/assets/b5bb383c-b884-47f5-a2fb-35f03667235a" />


⚡ Cracked the JWT signing secret using Hashcat (-m 16500) in under 1 second

✅ Generated a new verified low-privilege token with admin: false

It's all about the strength of your secret!

<img width="1101" height="584" alt="Снимок экрана 2026-04-24 224206" src="https://github.com/user-attachments/assets/9fbc225b-3d46-4879-b6f3-328036487faa" />

🏆 BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/35

______________________________________________________________________________________________________

10. MITRE ATT&CK Framework Challenge 🛡️
Difficulty: Easy

Tools: MITRE ATT&CK Navigator, attack.mitre.org
Skills: Tactic Identification, Technique Mapping, APT Group Research, Cloud Security, Threat Detection
Outcome: Identified techniques by tactic ID, mapped APT group G0099 to uncommon port activity, identified T1538 (Cloud Service Dashboard) as mitigation for cloud Discovery attacks, and determined detection methods for Pass the Hash technique in enterprise environments.

BTLO Profile: My Investigations & Badges
https://blueteamlabs.online/achievement/share/challenge/155436/15

______________________________________________________________________________________________________

11. Shiba Insider (BTLO) 🐕
Difficulty: Easy

Tools: Wireshark, Steghide, Command Line, Exiftool

Skills: Network traffic analysis (PCAP), file forensics, steganography, metadata extraction, password cracking

Outcome: Analysed a PCAP file to extract a response message and ZIP password, used Exiftool to find hidden metadata in an image file, identified steganography tool from metadata clues, extracted a hidden ID using Steghide, and traced the attacker's profile name — completing a full forensic chain from network capture to hidden data extraction.

<img width="1313" height="831" alt="logs" src="https://github.com/user-attachments/assets/7ef6e14a-8d32-4242-8177-1a5d6c2ed888" />

BTLO Profile: My Investigations & Badges
https://blueteamlabs.online/achievement/share/challenge/155436/29

______________________________________________________________________________________________________

12. D3FEND (BTLO) 🛡️
Difficulty: Easy

Tools: D3FEND Framework

Skills: Defensive cybersecurity frameworks, mapping defensive techniques to offensive techniques, threat modelling, MITRE D3FEND navigation, Azure Sentinel integration

Outcome: Explored the MITRE D3FEND framework to identify defensive technique IDs and names, mapped five general defensive tactics, investigated open-source projects that connect Azure Sentinel rules to MITRE ATT&CK and D3FEND, and defined key concepts such as File Access Pattern Analysis and Local Resource Access artifacts — building practical knowledge of defensive countermeasures for SOC operations.

BTLO Profile: My Investigations & Badges
https://blueteamlabs.online/achievement/share/challenge/155436/27



## 🛠️ Technical Skills
- **Cloud:** Azure Security (Sentinel, Defender).
- **Automation:** Python for Security (Custom DLP Agent project).
- **Analysis:** Wireshark, Splunk, Windows Event Logs.
- **Threat Intelligence:** MITRE ATT&CK, Ransomware TTPs, IOC Analysis



  

  
