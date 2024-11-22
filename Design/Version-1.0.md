# Version 1.0 of Anti-Evolved
Step one of this project is coming up with a UI, as it will give us an idea for what we want to add. 
For version 1.0 of the snapshot, we want to keep it simple.
1. Scan based on 1 signature type 
2. Give a result of either true or false 
3. Scans a file the user uploads

## Part 1: UI
- One window 
- Allows user to upload file 
- Software scans file 
- Returns whether or not it is possibly malware based on a preset database of signatures

###### **To do**
- learn what are malware signatures **Complex**
- learn how to allow a user to upload a file **Basic**
- learn how to scan a file **Basic**

## Malware Signature 
- Reactive
- Good against common attacks 
- Bad against new attacks, but saves the signature

### First Layer of Protection
- Signatures
	- Targeted
	- Generics
- Heuristics 
	- More Broad 
- Behavior 
	- Run time characteristics 
### Supporting Cast:
- White List
	- Prevents false positives from **Heuristics**

 Continue
https://youtu.be/7fgJvXwxFrs?si=D0s1ecelFquCn1Wh&t=247
#### Signature 
- Targeted 
- Generic 