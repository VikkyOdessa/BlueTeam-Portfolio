



_____________________________________________________________________________________________________

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
