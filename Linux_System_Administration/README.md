# Linux System Administration Module

## Overview

This project covers the comprehensive tasks involved in Linux system administration, including setting permissions on sensitive files, managing user accounts, and conducting system audits. These activities were part of a challenge that simulated real-world scenarios faced by Linux system administrators, aiming to secure and optimize Linux environments.

## Objectives

- Secure critical system files by setting appropriate permissions.
- Create and manage user accounts and groups.
- Implement system auditing and hardening using Lynis and chkrootkit.

## Tools Used

- Linux command line
- Bash scripting
- Lynis
- chkrootkit

## Methodology

### Ensuring System File Permissions

Verified and corrected permissions on crucial files such as `/etc/shadow`, `/etc/gshadow`, `/etc/group`, and `/etc/passwd` to prevent unauthorized access.

### User Account Management

Added user accounts for multiple users (`sam`, `joe`, `amy`, `sara`, `admin`) ensuring only `admin` has `sudo` access. Created an `engineers` group and a shared folder for collaborative work, setting correct ownership and permissions.

### System Auditing

Performed a system audit using Lynis to identify potential security issues. Installed and ran chkrootkit in expert mode for rootkit detection, further securing the system.

## Challenges and Solutions

- Encountered issues with incorrect file permissions leading to potential security vulnerabilities. Resolved by systematically reviewing and adjusting permissions as necessary.
- The process of manually checking each user and file permissions was time-consuming, highlighting the need for automation in system administration tasks.

## Key Learnings

- Gained a deep understanding of Linux file permissions and user account management, reinforcing the importance of securing a system from the ground up.
- Learned the value of regular system audits and familiarized myself with tools like Lynis and chkrootkit for monitoring and enhancing system security.
- Appreciated the necessity of clear documentation and systematic approaches in managing system security tasks.


