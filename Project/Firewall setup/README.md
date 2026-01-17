🌐 Network Topology
Server (SRV-WEB-PROD): 192.168.1.2

Admin PC (PC-ADMIN-ALLOW): 192.168.1.3 (Whitelisted)

User PC (PC-USER-BLOCKED): 192.168.1.1 (Blacklisted)

Switch: Cisco 2960 Central Switch

🛡️ Firewall Configuration

The firewall on the server was configured with a Top-Down logic approach:

Rule 1 (Allow): ALLOW IP 192.168.1.3 0.0.0.0

Purpose: Permits full access for the Admin PC using a specific wildcard mask.

Rule 2 (Deny): DENY IP 0.0.0.0 255.255.255.255

Purpose: Implements a "Default Deny" policy to block all other traffic.
