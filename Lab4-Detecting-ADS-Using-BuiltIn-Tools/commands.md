# Lab 4 – Detecting ADS with Built-In Tools

### Navigate to working directory
`cd C:\Users\danie\Documents\ADS-Project\Lab3`

## Basic ADS enumeration

### List files with ADS using Command Prompt <br>
`dir`<br>

### List files with ADS using Powershell <br>
`cmd /c dir /r` <br>

The `cmd /c` command is because PowerShell cannot display ADS without the cmd syntax.

### Using PowerShell to list ADS (limited view)
Syntax <br>
`Get-Item filename.txt -Stream *` <br>
For this lab; <br>
`Get-Item .\hostfile.txt -Stream *`

## Read specific ADS

### Command Prompt
Syntax <br>
`more < filename:streamname` <br>
For this lab <br>
`more < hostfile.txt:calc`

### Powershell
syntax <br>
`Get-Content filename -Stream streamname` <br>
For this lab; <br>
`Get-Content .\hostfile.txt -Stream calc`
