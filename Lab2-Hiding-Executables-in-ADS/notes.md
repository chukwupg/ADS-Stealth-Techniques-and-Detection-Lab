# Lab 2 – Notes: Hiding Executables in ADS

This lab hides a Windows executable (calc.exe) inside an ADS to demonstrate how attackers store malicious files covertly.

## Key Outcomes

- The executable does not appear in the directory listing.
- The host file (hostfile.txt) remains 0 bytes.
- ADS is only visible with dir /r which also displays the actual size.
- Binary data confirms the executable is successfully hidden.
- When the ADS is called, it runs directly in CMD which could be exploited by attackers to run malicious payloads.

## Security Implications

- Malware can hide C2 payloads or stages inside ADS.
- Antivirus solutions may miss ADS-based storage if they scan only primary streams.
