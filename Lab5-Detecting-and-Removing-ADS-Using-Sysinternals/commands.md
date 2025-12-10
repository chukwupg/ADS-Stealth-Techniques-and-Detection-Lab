# Lab 5 – ADS Detection & Removal using Sysinternals 

## Download streams.exe (from SysinternalsSuite)
(Place streams.exe in working directory or add to PATH)

## Scan current directory
`.\streams.exe .`

## Recursive scan
`.\streams.exe -s .`

## Remove ADS from a file
`.\streams.exe -d filename` <br>

For this lab; <br>
`.\streams.exe -d hostfile.txt`

## Remove all ADS in a directory tree
`.\streams.exe -s -d .`
