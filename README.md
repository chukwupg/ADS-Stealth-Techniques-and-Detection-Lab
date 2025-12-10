# ADS Stealth Techniques and Detection Lab

This repository contains a hands-on cybersecurity and digital forensics project focused on Windows NTFS Alternate Data Streams (ADS). 
The goal is to understand how ADS can be abused for covert storage, stealthy payload execution, malware persistence, and how defenders can detect and eliminate ADS-based threats.

This project includes six practical labs demonstrating red team techniques and blue team detection workflows. 
Each lab contains commands, notes, and screenshots for documentation.

## Labs Overview

### Lab 1 – Creating and Reading ADS  
Learn how NTFS Alternate Data Streams work, how to create them, and how to read their contents.

### Lab 2 – Hiding Executables in ADS  
Hide a Windows binary inside an ADS and verify that the content is hidden from normal file listings.

### Lab 3 – Executing Payloads from ADS  
Execute a hidden payload directly from an ADS using Windows built-in tools.

### Lab 4 – Detecting ADS Using Built-In Tools  
Identify ADS using native Windows commands such as `dir /r`, `fsutil`, and `more`.

### Lab 5 – Detecting and Removing ADS Using Sysinternals  
Use Sysinternals `streams.exe` to enumerate, investigate, and remove all ADS on the system.

### Lab 6 – Advanced Detection Using PowerShell  
Perform ADS enumerations, audits, and detection scans using custom PowerShell commands.

---

## Why ADS Matters in Security

Alternate Data Streams allow data to be attached to files without changing visible file size. 

Attackers frequently use ADS to:
- Hide malicious payloads  
- Store configuration files  
- Maintain persistence  
- Conceal encryption keys or staging data  
- Evade traditional file-based detection  

Understanding ADS is essential for red teams, blue teams, malware analysts, and digital forensics.

---

## Requirements

- Windows 10 or Windows 11  
- PowerShell or CMD  
- Sysinternals Suite (for Lab 5)  
- Administrative privileges recommended  

---

## Project Goal

To provide a complete offensive and defensive understanding of ADS techniques, empowering learners to identify, analyze, and mitigate ADS-based threats in real-world systems.

---

## Author

👩‍💻 **Chukwu PraiseGod**  
Follow my journey: [X](https://x.com/chukwupg) | [LinkedIn](https://linkedin.com/in/chukwupg)  
