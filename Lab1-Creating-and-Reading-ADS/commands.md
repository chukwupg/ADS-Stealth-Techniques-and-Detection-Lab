# Lab 1 - Creating and Reading Alternate Data Streams (ADS)

### Create a working folder
`mkdir ADS-Project`<br>
`cd ADS-Project`

### Create a visible text file
`echo Hello BasedOnBelieve > visible.txt`

## Create an ADS using CMD syntax (PowerShell cannot write ADS directly)
`echo Hidden content inside ADS > visible.txt:hidden`

### Verify visible.txt exists
`dir`

### Read the ADS contents
`more < visible.txt:hidden`

### List streams using /r flag to verify presence of an ADS
`dir /r`
