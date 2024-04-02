# Linux Systems Auditing and Hardening Project

## Overview

This project encapsulates the foundational steps in auditing a Linux system for security purposes, followed by investigating processes to identify and mitigate potential security threats. Conducted as part of a junior Linux system administrator role, these activities simulate real-world scenarios of system troubleshooting and hardening against malicious activities.

## Objectives

- Perform a basic audit of essential system files and directories.
- Investigate running processes for abnormalities or malicious activities.
- Apply hardening techniques to secure the system based on findings.

## Tools Used

- Linux command line
- Bash scripting

## Methodology

### Linux Landmarks

1. **System Audit:** Started with an exploration of critical system locations such as `/var/log` for audit logs, the home directory for unauthorized files, and `/bin` for essential binaries, to gather information for further analysis.

2. **Suspicious Activity Identification:** Checked for unusual scripts in temporary directories and unauthorized users in the `/home` directory.

### Process Investigation

1. **Process Snapshot:** Took real-time and static snapshots of all system processes to identify unusual or unauthorized activities.

2. **Script Investigation:** Analyzed a suspicious script found in an unusual location during the previous audit phase for characteristics of malicious activity.

3. **Memory and User Process Analysis:** Identified processes using significant memory and reviewed processes initiated by both system and unauthorized users.

4. **Process Termination:** Utilized the `kill` command to stop any suspicious processes identified during the investigation.

## Challenges and Solutions

- **Challenge:** Identifying malicious processes among legitimate ones.
  - **Solution:** Used command line tools to filter processes by user and memory usage, focusing on anomalies tied to known suspicious activities.

## Key Learnings

- **Importance of Regular Audits:** Continuous monitoring and auditing of system files and processes are crucial for early detection of potential security threats.
- **Hardening Practices:** Learned various system hardening techniques, such as restricting user permissions and removing unnecessary services or applications.
- **Command Line Proficiency:** Enhanced familiarity with Linux command line tools and their applications in system administration and security.

## Further Improvements

- Automate the auditing process with custom scripts to regularly check for anomalies.
- Implement more sophisticated monitoring tools for real-time threat detection.

