# Firewall-Configuration-Windows-Linux-Task4
Configured and tested basic firewall rules using Windows Firewall / UFW on Linux. Blocked inbound traffic on port 23 (Telnet), allowed SSH (port 22), verified rules, and documented commands and screenshots. Demonstrates understanding of firewall configuration and network traffic filtering.

Overview
This project demonstrates how to configure and test basic firewall rules on a Windows system using Windows Defender Firewall with Advanced Security. The objective is to block traffic on a specific port, test the rule using PowerShell, and restore the original configuration.

🎯 Objective
Configure a firewall rule to block inbound TCP traffic.
Test connectivity to verify rule enforcement.
Remove the rule to restore original settings.

🧰 Tools Used
Windows Defender Firewall with Advanced Security

Windows PowerShell
🚀 Steps Performed

1️⃣ Open Firewall Configuration Tool
Opened Windows Defender Firewall with Advanced Security from the Start menu.

2️⃣ Reviewed Existing Rules
Viewed Inbound Rules list to understand current configurations.

3️⃣ Created a Block Rule
Blocked TCP Port 23 (Telnet) by creating a new inbound rule:

Rule Type: Port
Protocol: TCP
Port: 23
Action: Block the connection
Profiles: Domain, Private, Public

4️⃣ Tested the Rule Using PowerShell
Command used to test connectivity:

Test-NetConnection -ComputerName 127.0.0.1 -Port 23
