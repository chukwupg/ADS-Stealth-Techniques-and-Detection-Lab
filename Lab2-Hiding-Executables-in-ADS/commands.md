# Lab 2 – Hiding Executables in ADS

## Create a working directory
`mkdir Lab2`<br>
`cd Lab2`

## Copy a Windows binary to the directory for testing
`copy C:\Windows\System32\calc.exe`

## Hide calc.exe inside an ADS
`type calc.exe > hostfile.txt:calcstream`

## Confirm hostfile.txt still shows 0 bytes
`dir`

## Confirm ADS presence and size using /r flag
`dir /r`

## Validate ADS contains binary data
`more < hostfile.txt:calcstream`
