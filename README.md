# Task 4: Firewall Configuration Report

## Tool Used:
- Windows Defender Firewall (Advanced Settings)
- Windows Command Prompt (netstat)

##  What I Did:

1. Opened **Windows Firewall (Advanced Settings)**.
2. Checked existing **Inbound Rules**.
3. Created a **new rule** to block traffic on **Port 23 (Telnet)**.
4. Used the command `netstat -an | find ":23"` to check if the port was open.
5. Verified that **port 23 was not active**, so the rule acts as a preventive security step.
6. Deleted the custom rule after testing.

## Why Block Port 23?

- Port 23 is used by **Telnet**, a **legacy protocol** that transmits data in **plaintext**.
- It is **highly insecure** and vulnerable to eavesdropping.
- Blocking this port helps in reducing attack surface.

## How a Firewall Filters Traffic
- A firewall filters traffic by inspecting incoming and outgoing network packets and deciding whether to allow or block them based on predefined rules.
- These rules can be based on: Port numbers (e.g., block port 23), IP addresses, Protocols (TCP/UDP), Traffic direction (inbound or outbound)
- By controlling this traffic, a firewall protects the system from unauthorized access, malware, and data leaks. In this task, I used a firewall rule to block inbound traffic on port 23 (Telnet) — an example of filtering based on port and direction.

## What I Learned:

- How to open and manage Windows Firewall settings.
- How to add and delete firewall rules.
- The importance of blocking unused or insecure ports.
- How to check open ports using `netstat` command.
- Basic concepts of **network traffic filtering**.

##  Screenshots Included:

- Inbound rules in Windows Firewall
- Rule created for blocking port 23
- Command Prompt output for port check (`netstat`)
