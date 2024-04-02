# Windows Privilege Escalation Project

## Overview
This project was conducted as part of the Cybersecurity Bootcamp at the University of Pennsylvania. It focuses on gaining SYSTEM privileges on a Windows machine using Metasploit.

## Objectives
- Understand and recognize privilege-escalation paths in Windows.
- Implement privilege escalation using Metasploit.

## Tools Used
- Metasploit
- Windows VM

## Process
- Initial Foothold: Gained initial access to the Windows machine as the tstark user through password spraying techniques.
- Meterpreter Session: Established a Meterpreter session using Metasploit, which served as the base for further exploitation.
- Background Session: Backgrounded the Meterpreter session using the background command to multitask within the Metasploit console.
- Local Exploitation Module: Selected the windows/local/persistence_service module within Metasploit to create a persistent backdoor. This module was chosen because services in Windows often run with SYSTEM privileges, providing an avenue for privilege escalation.
- Configuration: Configured the module with the necessary parameters, including setting the session to the previously backgrounded Meterpreter session and adjusting LHOST to match our attacking machine's IP address.
- Execution: Executed the module to create a service that runs a malicious payload, achieving privilege escalation.
- Verification: Confirmed the elevation of privileges by checking the user ID post-exploitation, ensuring we had achieved SYSTEM level access.

## Key Learnings
-Understanding of Windows Privileges: This activity deepened the understanding of Windows user privilege levels and how certain misconfigurations or vulnerabilities can be exploited to escalate privileges.
-Metasploit's Power and Flexibility: Learned to effectively use Metasploit's suite of tools for penetration testing, particularly for local exploitation and persistence.
-The Importance of System Hardening: Realized the significance of regularly auditing and hardening systems against such exploits. This includes ensuring services and applications run with the least privileges necessary and keeping systems updated.
-Security Awareness: Gained insights into the mindset of an attacker, which is invaluable for defending against similar attacks. Understanding the tools and methods used by attackers can guide more effective defensive strategies.
-Ethical Considerations: Reinforced the ethical responsibilities that come with cybersecurity skills. Such techniques should only be used in controlled environments for educational purposes or authorized penetration testing.

## Further Improvements
Change the executable name it assigns such as "REMOTE_EXE_NAME to something more stealthy such as "explorer.exe" so it looks like a regular service being ran. 
