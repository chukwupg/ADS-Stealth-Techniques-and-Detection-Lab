# Lab 3 – Executing Payloads from ADS

## Create working directory
`mkdir Lab3`<br>
`cd Lab3`

## Store calc.exe in ADS
`copy C:\Windows\System32\calc.exe`
`type calc.exe > hostfile.txt:calcstream`

## Verify Payload
`dir /r`

## Execute payload from ADS using 'powershell'
`Start-Process "C:\Users\danie\Documents\ADS-Project\Lab3\hostfile.txt:calc"`
