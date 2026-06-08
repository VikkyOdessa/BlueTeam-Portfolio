🔍 Gifted Crooks — Threat Intelligence Investigation with MISP

Practical Blue Team CTI lab — a real CERT-UA espionage campaign, dissected step by step.


📌 Overview
This lab investigates UAC-0226 / GIFTEDCROOK — a targeted espionage campaign against Ukrainian government institutions, law enforcement agencies, and innovation hubs, documented by CERT-UA.
The investigation was completed as part of the Security Blue Team training programme, using a live MISP event based on real threat intelligence.

🎯 Objectives

Analyze a MISP threat intelligence event tied to a real-world APT campaign
Extract and categorize IOCs (file hashes, filenames, scripts, office documents)
Map C2 infrastructure (IP addresses and ports)
Enrich IOCs using ICANN IP Lookup
Apply defanging techniques via CyberChef
Review TLP classification and event metadata
Map the attack to MITRE ATT&CK techniques


⚔️ Attack Chain
Phishing Email
    └── Malicious Excel (.xlsm) — social engineering lure
            
            └── Macro Execution → PowerShell Script
                   
                    └── C2 Connection established
                           
                            └── Browser data exfiltrated
                               
                                (passwords, cookies, browsing history)
Threat Actor: UAC-0226
Malware Family: GIFTEDCROOK (infostealer)
Target: Ukrainian government, law enforcement, innovation hubs
Source: CERT-UA advisory

🛠️ Tools Used
ToolPurposeMISPThreat intelligence platform — IOC analysis & event metadataICANN LookupIP/domain enrichment and registration dataCyberChefIOC defanging, encoding, and data transformationOSINT techniquesOpen-source intelligence gathering

📋 Key Findings
File-Based IOCs

Extracted and analyzed malicious file hashes (MD5 / SHA256)
Identified .xlsm phishing documents with embedded macros
Catalogued associated filenames and extensions used in the campaign

Infrastructure

Mapped C2 IP addresses and active ports
Performed IP enrichment via ICANN Lookup
Defanged all IOCs for safe documentation (e.g., hxxps://, [.])

MISP Event Analysis

Reviewed TLP classification (Traffic Light Protocol)
Examined event metadata, timestamps, and attribute tags
Correlated indicators across the attack lifecycle


🧩 MITRE ATT&CK Mapping
Technique IDNameDescriptionT1566.001Phishing: Spearphishing AttachmentMalicious .xlsm files delivered via emailT1059.005Command & Scripting: Visual BasicVBA macros triggering PowerShell executionT1071Application Layer ProtocolC2 communication over standard protocolsT1041Exfiltration Over C2 ChannelBrowser data exfiltrated through established C2


🧠 Skills Demonstrated

Threat Intelligence analysis using MISP
IOC extraction, classification, and enrichment
C2 infrastructure mapping
OSINT and open-source tooling (CyberChef, ICANN)
MITRE ATT&CK framework application
TLP-aware documentation practices
CTI reporting and defanging standards


📚 References

CERT-UA Advisory — UAC-0226 / GIFTEDCROOK campaign
MITRE ATT&CK — Technique reference
Security Blue Team — Training platform
CyberChef — IOC transformation tool


👩‍💻 About
Cyber Security Analyst in progress — breaking down real malware, hunting threats, and turning logs into stories.
Based in Ireland 🇮🇪 | Preparing for CySA+ | Open to SOC / Blue Team opportunities.
Making the complex simple — one investigation at a time.

🇺🇦 Wishing Ukraine the swiftest victory on all fronts — including the digital one.
<img width="1895" height="664" alt="lab 08 06" src="https://github.com/user-attachments/assets/c8e42368-da7a-4fcd-8fdc-66a94054b6b9" />
<img width="869" height="465" alt="lab 08 06-1" src="https://github.com/user-attachments/assets/ace96591-cf9f-4dbb-a821-adc8d62e8809" />
<img width="814" height="577" alt="lab 08 06-2" src="https://github.com/user-attachments/assets/ff54f07b-b543-47b0-b538-d6d2ea4e147e" />


