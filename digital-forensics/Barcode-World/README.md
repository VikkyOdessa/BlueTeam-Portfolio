# Barcode World Challenge

## Overview
Analysis of 9,374 barcode images to extract a hidden message — Blue Team Labs Online.

## Tools Used
- Kali Linux
- Python (opencv, pyzbar)
- CyberChef

## Approach
Wrote a Python script to decode all barcode images sequentially, collect the bytes and convert to ASCII. The output was then decoded from decimal in CyberChef to reveal the hidden message.

## Key Steps
1. Decoded 9,374 barcode images using pyzbar
2. Collected all bytes and converted to ASCII numbers
3. Used CyberChef → From Decimal to get the final text
4. Found the flag hidden inside the barcode history text

## BTLO Profile
https://blueteamlabs.online/achievement/share/challenge/155436/34

<img width="653" height="530" alt="image" src="https://github.com/user-attachments/assets/29dc949d-c9ae-4e6c-a896-a5ea243bec4a" />

<img width="1919" height="882" alt="image" src="https://github.com/user-attachments/assets/59339371-48ca-4f6b-9860-467e01545ee3" />

