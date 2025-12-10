# Lab 3 – Notes: Executing Payloads from ADS

This lab demonstrates direct execution of a payload stored inside an ADS.

## Key Lessons

- Windows can execute a program from ADS despite the file being hidden.
- Attackers use ADS execution for stealthy lateral movement.
- Command prompt restrict execution of a program from ADS due to Windows security features.
- Execution via powershell `Start-process` command bypasses naive detection and windows security features.

## Red Team application

- Payload staging
- Antivirus evasion
- Security/Defense evasion

## Blue Team coutermeasures

- Detect suspicious ADS execution via Sysmon Event ID 1 (Process Creation)
- Monitor command-line arguments containing colon syntax (filename:stream)
