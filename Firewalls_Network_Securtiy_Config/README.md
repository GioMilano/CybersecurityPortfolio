# Firewalls and Network Security Configuration

## Overview

This project encompasses a series of activities aimed at securing an organization's network infrastructure through effective firewall configurations using both UFW and firewalld, alongside auditing the security posture with Nmap. These activities are part of a broader initiative to comply with PCI DSS requirements and to safeguard against unauthorized access and network reconnaissance.

## Objectives

- Configure UFW to restrict access to essential services, ensuring compliance with PCI DSS requirements.
- Utilize firewalld for multi-zone-based firewall filtering to segment network traffic and services effectively.
- Perform network scans using Nmap to identify open ports and test firewall rule efficacy.

## Tools Used

- UFW (Uncomplicated Firewall)
- firewalld
- Nmap

## Methodology

### UFW Configuration

- Reset UFW to default settings and configured default rules to deny incoming and allow outgoing connections.
- Specified rules to allow traffic on ports essential for the organization's operations, including HTTP (80), HTTPS (443), SSH (22), IMAP (143), SMTP (587), and POP (110).

### firewalld Configuration

- Transitioned from UFW to firewalld for its advanced multi-zone filtering capabilities.
- Created zones for specific services (HTTP, HTTPS, SSH) and a default zone for other traffic, applying targeted rules for each.

### Network Security Auditing with Nmap

- Conducted scans against the network to validate firewall configurations, using Nmap to enumerate open ports and service types, and to perform OS fingerprinting.
- Tested firewall rules for their effectiveness in blocking unauthorized access while allowing permitted connections.

## Challenges and Solutions

- **Challenge:** Ensuring minimal service disruption while implementing stringent firewall rules.
  - **Solution:** Carefully planned rule implementation during low-traffic periods and conducted thorough testing before deployment.

- **Challenge:** Balancing security with compliance requirements.
  - **Solution:** Configured firewall rules that comply with PCI DSS without compromising the network's security posture.

## Key Learnings

- Gained hands-on experience in configuring and managing firewalls using both UFW and firewalld.
- Learned the importance of regular security audits using tools like Nmap to identify potential vulnerabilities.
- Understood the critical balance between operational requirements and security measures in network administration.


