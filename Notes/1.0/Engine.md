# Threat Detection Technique
- Signature based only for 1.0
- Add the most common signatures 
	- import data from external sources
	- API like attachmentAV
- scan a single file 

## What do look for in files
- Strings 
- Assembly patterns 
- Hex patterns
- etc..

## Example Virus Scanners
- [SimpleVirusDetector](https://github.com/ThejanRupasinghe/SimpleVirusDetector/tree/master)
	- Has a preset dictionary of virus definitions
	- If file scan has a virus that's in there, its flagged as a virus 
	- Pros 
		- Simple
		- Quick
		- Yes or no guaranteed 
	- Cons
		- Limited to manually set dictionary 
		- Does not do any actual scanning or provide reports
- [Python-Antivirus](https://github.com/Len-Stevens/Python-Antivirus/tree/main)
	- Preset of hard signatures
	- Checks OS
	- Scans and delete files
	- Uses MD5, SHA1, and SHA256 malware hashes
		- Gets hash, and checks if its **EQUAL** to any hash dictionary 
# Engine Method
1. TBD