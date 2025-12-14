# Lab 1 - Notes: Creating and Reading ADS

This lab demonstrates the fundamentals of Windows NTFS Alternate Data Streams.

## Key Points

- NTFS stores file data inside the $DATA attribute.
- Files can contain multiple data streams: one visible and others hidden.
- ADS are referenced using the syntax:
  
  filename:streamname

- File size does not reflect the size of any hidden ADS.

## Observations

- `dir` does NOT show ADS.
- `dir /r` reveals all streams attached to a file.
- PowerShell redirect (>) does not support ADS and throws an error.
- ADS must be created via CMD or PowerShell + cmd /c.

## Use Cases

### Legitimate:
- Storing file metadata
- Compatibility with older applications

### Malicious:
- Hiding payloads
- Concealing configuration files
- Maintaining stealth persistence
