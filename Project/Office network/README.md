DHCP Addressing (The "Automatic" IP)
The network is designed to eliminate manual configuration by using DHCP
(Dynamic Host Configuration Protocol).

Order,Action,Protocol,Target,Reason
Priority 1,DENY,IP,192.168.1.23,Specifically isolates the Laptop from the server.
Priority 2,ALLOW,IP,Any,Ensures the rest of the network remains functional.

When the Laptop tries to talk to the Server, 
it hits Rule 1 and is Dropped. 
When any other PC tries to talk, 
it fails to match Rule 1, moves to Rule 2, and is Permitted
