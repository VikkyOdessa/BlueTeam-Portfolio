# 🔍 Digital Forensics & Cryptography – Veriarty

**Platform:** Blue Team Labs Online (BTLO)
**Difficulty:** Medium
**Tools:** Hashcat | VeraCrypt | GPG | Thunderbird | CyberChef

---

## 📋 Scenario

A cryptographic investigation requiring hash cracking, encrypted container analysis, email decryption, and hidden directory discovery.

---

## 🎬 Investigation Flow

### Step 1 — Hash Cracking
Identified the hash type of the encrypted container and recovered the password using a dictionary attack with Hashcat.

<img width="792" height="606" alt="image" src="https://github.com/user-attachments/assets/0299449e-ffd0-466f-a6c8-e6957116f9f1" />


### Step 2 — Container Mounting
Mounted the encrypted volume and discovered hidden files — including an encrypted email and a cryptographic key.

> ⚠️ VeraCrypt 1.26.24 no longer supports the old container format. Had to install legacy version 1.25.9 — and that's how I learned to manage tool versions in Kali via terminal for the first time.

### Step 3 — Email Decryption
Used the recovered GPG key to decrypt the email and opened it in Thunderbird.

### Step 4 — Message Decoding
The email subject line itself was the hint to the decoding method. Two steps in CyberChef — and the hidden communication was revealed.

<img width="1913" height="908" alt="image" src="https://github.com/user-attachments/assets/99b57e65-2b2d-4c7a-bb76-2cc8fcc27f62" />


### Step 5 — Hidden Directories
Mounted a second volume using a keyfile instead of a password. Discovered deeply nested hidden folders disguised as system directories — containing evidence of the meeting location.
<img width="592" height="482" alt="image" src="https://github.com/user-attachments/assets/76615aaf-7b5b-4fba-8a7e-5d5788b90d37" />


<img width="732" height="492" alt="image" src="https://github.com/user-attachments/assets/ff3c89e3-9650-42fc-b0b2-1ff08d7b8485" />
<img width="605" height="799" alt="image" src="https://github.com/user-attachments/assets/e64f60ea-fa44-4da5-a059-4e0c677882c7" />


### Step 6 — Binary Clock
Decoded a visual binary clock to extract the final piece of evidence.
<img width="585" height="780" alt="image" src="https://github.com/user-attachments/assets/7a5ebb1a-7d18-4c3f-940a-a9a245efd081" />


---

## 🎯 MITRE ATT&CK Mapping

| Technique | ID |
|---|---|
| Obfuscated Files or Information | T1027 |

https://blueteamlabs.online/achievement/share/challenge/155436/36
