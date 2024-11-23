Source: https://robots.net/tech/how-to-make-an-antivirus/
# What is an Antivirus Software?
An Antivirus software is a program designed to **detect, prevent, and remove malicious software from a computer or device**. It does this by *scanning files, documents, and applications for known treats and neutralizes them*, ensuring the security and integrity of the system.
# Pre-Requisites 
- Deep understanding of **malware behavior**
- Strong **programming skills**
- **Security Practices** knowledge
# Understanding Antivirus Software
- Designed to protect a system from **malware, viruses, worms, Trojans, ransomware, adware, and other malicious threats**.
- One of the most common techniques Antivirus software uses is **signature-based detection**. Where the antivirus software scans files and compares them against a **database of known malware signatures**. If a match is found, the Antivirus takes appropriate action by usually removing the file.
- In todays ever evolving world, **signature-based detection** is not enough anymore, so they have some other techniques, like **behaviors-based analysis and machine learning**. This uses algorithms to analysis patterns and sorts files based on the likelihood that they are malware.
- Other tools within Antiviruses is **real-time scanning**. Where the Antivirus continually scans the computer for possible threats. They also tend to have **quarantine systems**, where they isolate the malware to prevent it from spreading.
- Some other features include **schedules scans, a white list, and an exclusive system**. Allowing periodic scanning, and setting trusted files to prevent false positives.
- **Updating the Antivirus** is crucial in order for it to stay effective, just as malware continuously evolves, so must the Antivirus.
# Setting Up the Development Environment
Before working on making a Antivirus, you have have a development environment to work with.
**Programming Language:** Java 
**IDE:** IntelliJ
**Version Control System:** Git
**Dependency Management:** [Maven](https://www.geeksforgeeks.org/what-is-maven/)
**Testing Tools:** [JUnit](https://www.geeksforgeeks.org/introduction-of-junit/)
**Build & Deployment:** [Ant](https://www.codejava.net/tools/ant/introduction-to-ant-for-beginner)
# Creating a User Interface
- User requirements 
- Design layout and Navigation 
- Visual Theme 
- Intuitive Controls 
- Real-Time Status Updates
- Customization Options 
- Responsiveness 
# Designing The Antivirus Engine 
- **Threat Detection Techniques** (Signature Based, Behavior Based & Algorithms)
- **Scanning Mechanism** (Scan files quick, but efficiently to prevent false positives)
- **Heuristics** (Able to scan new types of malware based on file behavior, code structure, etc.)
- **Quarantine & Removal** (Be able to properly isolate or remove the malware, Test on VMs)
- **Virus Definitions** (Regular update the antivirus and definitions for new viruses and malware)
- **Optimization and Performance** (Maximize efficiency by utilizing effective *Data Structures & Algorithms*)
### Designing The Antivirus Engine p.2
- Conduct **extensive research** and stay updated on latest advancements in malware 
- Keep your engine **modular** & **scalable**
- Incorporate **logging** and **error handling** for debugging and troubleshooting 

# Developing the Real-Time Scanner
- **Monitoring System Activities** 
	- Identify file accesses 
	- Process launches 
	- network communication 
- **File and Process Scanning**
	- Find an efficient way to scan files and processes (based on **Designing The Antivirus Engine**)
	- Balance between speed and accuracy 
	- Avoid false positives 
- **Memory Scanning**
	- Incorporate memory scanning abilities to see if the malware resides in the systems RAM
	- Include process memory scanning & code injection detection
- **Behavior Analysis**
	- Add behavior analysis techniques 
	- Develop heuristics that analyze file behavior, code execution patterns, and network communications
- **Real-Time Notifications**
	- Alert user when a potential threat is detected in real-time. 
	- Convey the type of threat, the severity level, and recommended actions.
	- Give users a chance to take immediate actions 
- **Performance and Resource Optimization**
	- Minimize resource consumption 
	- multi-threading or background processing 
- **Integrate with systems**
	- Integrate with specific OS for smooth protection 
- **Regular Updates**
	- Update regularly to keep up with continuously updating malware 
## Testing and Quality Assurance
- Due to the complexity of this project, constant tests are required 
- Test different scenarios, OSs, malware, files, system processes, and network environments 
- Ensure **accuracy, reliability, and compatibility**
# Implementing Quarantine System 
- Isolating potential malicious software is important 
- **Quarantine Action** 
	- Decide what action to take with the potential malware 
	- moving the file to a quarantine folder, or a specific location 
	- Must be careful in case it is a false positive
- **Secure Location**
	- Secure and isolate the malware properly
	- File permissions, encryption
- **Quarantine Management**
	- UI to view and manage quarantines items 
	- Restore, permanently delete, submit for further analysis
- **False Positive Handling**
	- Allow users to exclude files, directories, applications
- **Quarantine Reporting**
	- Give reports on quarantines files 
	- file name, detection date, threat information
- **Periodic Scans and Release**
	- Scan quarantined files regularly to see for updates or evolving
	- Add auto release on files that no longer seem like a threat
## Security & Reliability 
- Encryption, access control, secure storage
- Consider performance on system storing malware 
# Adding Scheduled Scans 
- Periodic scans are good for actively checking the computer for malicious activity but then sitting in the background for saving resources
- **Scan Frequency**
	- Based on user preferences and system usage patters 
	- daily, weekly, or custom
- **Scanning Scope**
	- Different types of scans 
	- Specific drives, folders, or file types 
	- Full system scans, quick scans, custom scans 
- **Customization Options**
	- Specific scan times 
	- exclude files/folders 
	- adjust level of scan 
	- Provide clear instructions 
- **Idle Time Scans:** 
	- Scan system while its idle to utilize resources more efficiently
	- Don't interrupt user
- **Automatic Updates**
	- Update to keep software and virus definitions up to date
- **Logging and notifications**
	- Record logs very clearly
	- Provide detailed reports 
- **Performance Optimization**
	- Balance speed, efficiency, and resource management
### Seamless user experience 
- Easily modifiable 
- Add recommendations 
- Regular tests 
# Building a Whitelist and Exclusion System 
- Help prevent false positives, and exclude files that are safe
- **User-Defined Exclusions**
	- Allow user to exclude certain files easily and clearly 
- **Default Exclusions**
	- Add default exclusions for certain OS, applications, etc...
- **Exclusion Criteria**
	- Allow exclusion based on file type, paths, regex, etc...
- **Scan Customization**
	- Whitelist/exclusion system should be connected to both scheduled scans and real-time scans
	- Allow different exclusions based on the scan 
- **Exclusion Persistence**
	- Ensure exclusion persists after applications update, system reboots, etc..
- **Validation and Auditing**
	- Verify what files are being excluded to prevent security holes, need admin/root to exclude/whitelist certain files
	- Add reports and logs for all changes 
- **Education and Best Practices**
	- Provide clear instructions on what to allow/deny in the list to make sure they are adhering to the latest security policies 
### Seamless UX
- Allows users to tailor the antivirus to their specific needs, making it more versatile for multiple people
# Designing the Update Mechanism 
- As malware evolves, so much the antivirus
- **Automatic Updates**
	- Antivirus automatically checks for updates in the database of malware so make sure its updated 
- **Secure Communication**
	- Ensure secure connection between the antivirus and the update server 
	- Encryption and digital signatures
- **Update Frequency**
	- Balance timely updates and network congestion/resource consumption
- **Incremental Updates**
	- Rather than 1 big update, do multiple smaller updates to maintain resource consumption
- **Offline Update Support**
	- Allow uses to manually input updates from a trusted source and allow them to update the software without the needed for an internet connection
- **Update Notifications**
	- Notify users when updates are available and allow users to update when ready
- **Rollback Mechanism**
	- Allow users to roll back to previous versions in case of compatibility issues
	- Include LTS for certain versions 
- **Reporting and logging**
	- Log the update process to see for any issues and include and audit trail
### UX & Reliability 
- Ensure users are able to use it well
- Ensure updates happen in a efficient manner 
# Testing and Debugging the Antivirus 
- Longest phase of the project, making sure the Antivirus works in multiple scenarios, OS, malware, etc... 
- Identify and fix bugs
- Ensure accuracy and performance
- Proper use of data structures & algorithms 
- speed tests 
- unit testing 
- **Test Plan**
	- Create a full test outline to test multiple different scenarios, both positive and negative tests 
	- Cover different files, sizes, and different malware types 
	- Make sure all tools above are working as intended (scanning, real-time protection, quarantine, and update mechanisms.)
- **Test Environment**
	- Create a controlled environment to test the antivirus, isolate a VM and download the antivirus, then run different types of malware
- **Functional Testing**
	- Check that every component is testing and handling files properly, isolating files, and logging as intended
- **Performance Testing**
	- Test it against high volume scans 
	- Check speed, resource management, and the impact on the system
- **Compatibility testing**
	- Test against different OSs, Hardware, software, etc...
	- Test with different versions 
- **Regression Testing**
	- After bug fixes and updates ensure the changes do not impact current working components 
	- Set a baseline for best resource management, and test against to see if its worth the trade
- **Security Testing**
	- Check the antivirus itself for any vulnerabilities someone may be able to take advantage of
	- Pen test the program 
	- Code review 
	- Use vulnerability scanning tools 
- **Debugging and Issue Tracking**
	- Track and log all issues, to be able to have an efficient form of communication and quickly resolve problems 
### Documentation
- Logs 
- Audits 
- Previous versions 
- Keep track of everything
# Conclusion
- Constantly evolving
- Keep in mind UX & UI
- Security is key 



# Other malware video
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
	- popular files
- Heuristics 
	- More Broad 
- Behavior 
	- Run time characteristics 
### Supporting Cast:
- White List
	- Prevents false positives from **Heuristics**
- spectrum / reputation 
	- leverage data from the field 
- Sandboxing 