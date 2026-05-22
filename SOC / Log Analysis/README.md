


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
