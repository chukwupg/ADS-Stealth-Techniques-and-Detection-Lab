# Lab 6 – Advanced ADS Detection Using PowerShell

## List ADS for a single file
`Get-Item filename.txt -Stream *` <br>
For this lab; <br>
`Get-Item hostfile.txt -Stream *`


## List ADS for all files in directory
`Get-ChildItem -Recurse | ForEach-Object {
    Get-Item $_.FullName -Stream * 2>$null
}`

## Export ADS findings to CSV
`Get-ChildItem -Recurse | ForEach-Object {
    Get-Item $_.FullName -Stream * 2>$null
} | Export-Csv ADS_Report.csv -NoTypeInformation`
