# Cybersecurity Internship Task 4: Setup and Use a Firewall

## Objective
Configure and test firewall rules to block and allow specific network ports, gaining practical skills in network traffic filtering.

## Tools Used
- **Windows Firewall** (Advanced Security)
- **UFW (Uncomplicated Firewall)** on Linux

## Steps Performed

### Step 1: Accessing Windows Defender Firewall
- Opened the Start Menu, searched for "Windows Defender Firewall with Advanced Security," and launched the application.
- Navigated to the left panel to view inbound and outbound rule sections.

### Step 2: Blocking Inbound Connections on Port 23 (Telnet)
- Clicked “Inbound Rules” > “New Rule...” on the right.
- Selected “Port” as the rule type; specified “TCP” and entered port 23.
- Chose the “Block the connection” option for all profiles (Domain, Private, Public).
- Named the rule “Block Telnet Port 23” before saving.

### Step 3: Allowing Inbound Connections on Port 22 (SSH)
- Created a new inbound rule, again selecting “Port,” then specified “TCP” and port 22.
- Selected “Allow the connection” and applied it to all profiles.
- Saved this as “Allow SSH Port 22.”

### Step 4: Reviewing and Testing Rules
- Confirmed both rules appeared under the Inbound Rules list.
- Used command-line tools such as `telnet` to check that port 23 was blocked, and verified that port 22 remained open (assuming an SSH server was running).
- Ensured the firewall behaved as expected for each test.

### Step 5: Rule Cleanup
- After testing, disabled or deleted the custom rule for port 23 to revert to default firewall settings.

## Lessons Learned
- Telnet on port 23 is considered insecure; blocking it helps reduce exposure to attacks.
- Allowing SSH (port 22) supports secure, encrypted remote management.
- Regular review and management of firewall rules are essential for robust system security on Windows 10.

## Conclusion
Configuring Windows 10 Firewall rules firsthand deepened my understanding of practical network security. I learned how custom rules help control system exposure and how to verify that protective measures work as intended.

---

*This README is submitted for Elevate Labs Cybersecurity Internship Task 4: Windows 10 Firewall Configuration.*
