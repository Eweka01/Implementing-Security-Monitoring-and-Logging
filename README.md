# Implementing Security Monitoring and Logging

**Author**: Osamudiamen Eweka  
**Course**: CYB-605-Z2 Principles of Cybersecurity  
**Institution**: Utica University

## Overview

This lab focuses on the implementation of security monitoring and logging across both Windows and Linux environments. Participants gain hands-on experience using tools like the Windows Event Viewer, Snort for intrusion detection and prevention, and Tripwire for file integrity monitoring. The lab emphasizes the importance of security event logging, monitoring, and responding to potential security incidents to maintain a robust security infrastructure.

## Objectives

- Understand the significance of security monitoring and logging in maintaining a secure infrastructure.
- Learn how to identify failed login attempts using the Windows Event Viewer and Linux logging mechanisms.
- Configure Snort as an Intrusion Detection System (IDS) and transition it to an Intrusion Prevention System (IPS).
- Utilize Tripwire for monitoring file integrity on a Linux system.
- Analyze security events, including Audit Failure events with Event ID 5061, to understand their impact on system security.

## Lab Setup

### Lab Environment Details

The lab setup includes the following tools and software:

- **Windows Event Viewer**: A utility for monitoring system and application events, crucial for incident response and forensic analysis.
- **Snort**: A network intrusion detection and prevention system (IDS/IPS) used for monitoring network traffic and detecting potential threats.
- **Tripwire**: A file integrity monitoring tool used on Linux systems to detect unauthorized changes to files.
- **PuTTY**: A terminal emulator for secure remote access to Linux systems.

## Hands-On Demonstrations

### 1. Identify Failed Logon Attempts on Windows Systems
Participants used the Windows Event Viewer to identify failed login attempts by filtering for Event ID 4625. This exercise emphasized the importance of analyzing failed logon events to detect potential security threats, such as brute force attacks. Detailed information, including the target username, source IP address, and communication port, was extracted and analyzed.

### 2. Monitor Network Activity with Snort
Participants configured Snort to monitor network traffic on a local area network (LAN) and detect potential intrusions. The lab demonstrated how to configure Snort, apply detection rules, and log ICMP traffic. Snort's transition from an Intrusion Detection System (IDS) to an Intrusion Prevention System (IPS) was also explored by enabling Legacy Blocking Mode.

### 3. Identify Failed Logon Attempts on Linux Systems
Participants used PuTTY to connect to a Linux-based network switch (Switch01) and configured it to send logs to a remote server. The lab involved simulating brute force attacks and using Linux commands like `sudo lastb` and `sudo tail` to analyze failed login attempts and recent log activity.

### 4. Monitor File Integrity with Tripwire
Participants configured Tripwire on a Linux system to monitor file integrity. The lab demonstrated how to initialize Tripwire's database, simulate file changes, and generate a Tripwire report to identify unauthorized modifications. This exercise highlighted the importance of file integrity monitoring in maintaining a secure system.

## Challenge and Analysis

### 1. Identify Additional Event Types in the Event Viewer
Participants analyzed Audit Failure events, particularly Event ID 5061, which is related to cryptographic operations in Windows. This exercise emphasized the need for monitoring cryptographic operations to ensure security and compliance within an IT environment.

### 2. Configure Snort as an Intrusion Prevention System (IPS)
Participants configured Snort to operate as an Intrusion Prevention System (IPS) by enabling Legacy Blocking Mode on the LAN interface. This transition allowed Snort to not only detect potential intrusions but also actively prevent and block them, enhancing the security posture of the network.

## Conclusion

This lab provided a comprehensive exploration of security monitoring and logging techniques across both Windows and Linux environments. Participants gained practical experience in detecting and responding to potential security incidents using tools like the Windows Event Viewer, Snort, and Tripwire. The lab emphasized the importance of security event logging, monitoring, and prevention in maintaining a robust cybersecurity defense.

## References

- ControlCase. (2023). *Security Event Logging and Monitoring Services*. https://www.controlcase.com/services/log-monitoring/
- Jones & Bartlett (2024). *Implementing Security Monitoring and Logging (Figures)*. Jones and Bartlett Learning Virtual Lab. URL: https://jbl-lti.hatsize.com/startlab
- Vinaypamnani-Msft. (2021). *5061(S F) Cryptographic Operation - Windows 10*. Microsoft Learn. https://learn.microsoft.com/en-us/windows/security/threat-protection/auditing/event-5061

For a complete list of references, please refer to the full lab report.
