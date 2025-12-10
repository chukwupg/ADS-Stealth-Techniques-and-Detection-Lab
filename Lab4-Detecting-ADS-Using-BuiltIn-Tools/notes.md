# Lab 4 – Notes: Built-In ADS Detection

The following Windows-native tools help reveal ADS:

---

## Detecting ADS

### Command Prompt
`dir /r` <br>
Shows all ADS attached to a file.

### PowerShell 
`cmd /c dir /r` <br>
Shows all ADS attached to a file<br>

`Get-Item filename -Stream *` <br>
Lists stream names but does not show sizes on older versions.

---

## Reading Contents of an ADS

### Command Prompt<br>
`more < filename:streamname`<br>

### Powershell<br>
`Get-Content filename -Stream streamname` <br>

This allows reading the content of a hidden stream without modifying the file.

---

### Extract ADS to a New Normal File
`Get-Content filename -Stream streamname -Raw | Set-Content new_filename.txt`

This is used in:
- Malware analysis
- Incident response
- Evidence preservation

---

## Limitations

- Does not recursively scan directories.
- Does not show deep threat details.
- Cannot remove ADS automatically.
