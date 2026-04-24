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

### 1. Phishing Analysis 📧
* **Difficulty:** Easy
* Tools: Thunderbird, Sublime Text, URLScan, Whois.
* Skills: Email Header Analysis, Malicious URL Investigation, Artifact Extraction.
* Outcome: Analyzed a suspicious email, traced the attacker's infrastructure (IP: 103.9.171.10), and identified phishing indicators.
    
- **BTLO Profile:** My Investigations & Badges:
- https://blueteamlabs.online/home/user/4eb059f27d5254487a2a31

### 2. Phishing Analysis-2 📧

• Difficulty: Easy

• Tools: Thunderbird, Sublime Text, CyberChef, URLBox

• Skills: Email Header Analysis, URL Investigation, Base64 Decoding, Indicator Identification

• Outcome: Investigated a suspicious email, decoded obfuscated content, and identified a hidden phishing link to an external profile.

- **BTLO Profile:** My Investigations & Badges
  https://blueteamlabs.online/achievement/share/challenge/155436/24

### 3. Brute-force Attack Investigation 📊  
Difficulty:** Medium  

• **Tools:** Microsoft Excel, IP lookup services  
• **Skills:** Windows Event Log Analysis (Event ID 4625), Log Filtering, Source IP Identification, Port Range Analysis  
• **Outcome:** Analyzed Windows Security logs, identified repeated failed logon attempts, detected a brute-force attack, and determined the source IP and port range.  

BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/40

### 4. The Report II 📄  
Difficulty: Medium  

• **Tools:** MITRE Report (PDF), Web Browser  
• **Skills:** SOC Concepts, Incident Response Workflow, Threat Intelligence, Organizational Models, Log & Data Understanding  
• **Outcome:** Analyzed MITRE SOC report, identified key operational strategies, SOC structures, incident prioritization methods, and extracted actionable insights for improving SOC effectiveness.  

BTLO Profile: My Investigations & Badges:  
https://blueteamlabs.online/achievement/share/challenge/155436/44

### 5. Meta Investigation 📊

Difficulty: Medium

• **Tools:** ExifTool, Google Earth, TinEye

• **Skills:** Metadata Analysis, EXIF Data Extraction, GPS Coordinate Conversion, Geolocation, Reverse Image Search

• **Outcome:** Extracted metadata from images to identify camera model, capture time, and embedded comments, determined geographic location using GPS data and validated the findings through reverse image search to locate the suspect’s possible whereabouts.

BTLO Profile: My Investigations & Badges
https://blueteamlabs.online/achievement/share/challenge/155436/39

6. Spectrum Investigation 🎧

Difficulty: Easy

• Tools: PhotoRec, fcrackzip, steghide, Base58 Decoder, Google Maps

• Skills: Disk Forensics, File Recovery, Archive Password Cracking, Steganography Analysis, Data Decoding, Geolocation

• Outcome: Recovered files from a disk image, identified and cracked a password-protected archive, extracted hidden data from embedded files, decoded encoded information, and uncovered GPS coordinates hidden within an audio file, which were then mapped to a real-world location.

BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/26


7. Threat Report Analysis (SOC) 📊

Difficulty: Easy

• Tools: Threat Intelligence Reports, MITRE ATT&CK Framework, Web Research

• Skills: Threat Intelligence Analysis, Vulnerability Identification, MITRE Mapping, Ransomware TTPs, SOC Detection Use Cases

• Outcome: Analysed a 2022 threat report to extract actionable intelligence for SOC operations, identified major attacks such as Log4Shell, mapped techniques to MITRE ATT&CK, reviewed critical vulnerabilities (including Exchange exploits and zero-day RCE), analysed ransomware affiliate models (Conti), and defined detection and prevention measures (e.g., parent process monitoring, RDP hardening) to improve SOC readiness.

BTLO Profile: My Investigations & Badges:
https://blueteamlabs.online/achievement/share/challenge/155436/42


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

## 🛠️ Technical Skills
- **Cloud:** Azure Security (Sentinel, Defender).
- **Automation:** Python for Security (Custom DLP Agent project).
- **Analysis:** Wireshark, Splunk, Windows Event Logs.
- **Threat Intelligence:** MITRE ATT&CK, Ransomware TTPs, IOC Analysis



  

  
