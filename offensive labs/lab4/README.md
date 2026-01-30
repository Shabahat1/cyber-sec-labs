This lab focuses on the exploitation phase of a penetration test. After identifying open ports (139/445) on the target system, I utilized Metasploit's auxiliary scanner modules to launch a dictionary attack against the SMB service. This demonstrates how weak passwords (leo1234) can lead to immediate unauthorized access to file shares."

Technical Highlights:

Service Enumeration: Identified webfs/1.21 on port 8000 and the NetBIOS name ACME IT SUPPORT.

Automated Brute-Force: Configured the Metasploit scanner to test credentials against the penny user account.

Successful Compromise: Validated the credentials penny:leo1234, confirming access to the system.

2. Post-Exploitation with Meterpreter
Based on the screenshot showing file searches and reading 'secrets.txt'.

A walkthrough of "living off the land" after compromising a Windows host. Demonstrates the use of the Meterpreter payload to navigate the filesystem, search for sensitive artifacts (secrets.txt), and exfiltrate data without triggering basic alerts.
