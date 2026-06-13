# Network Fundamentals for Cybersecurity
## Overview
Networking is one of the most important foundations in cybersecurity. Understanding how device communicate, exchange data, and access network services is essential before learning topics such as network scanning, penetration testing, web security, and incident response.
___
## Public and Private Networks
### Public Network
A private network is used for internal communication within homes or organizations.
Example of private IP ranges:
- 10.0.0.0/8
- 172.16.0.0/12
- 192.168.0.0/16
___
## IP Addressing
An IP adress identifies a device on a network.
### IPv4
IPv4 uses 32-bit addresses.
Example: 192.168.1.10
### IPv6
IPv6 uses 128-bit addresses and provides a significantly larger address space than IPv4.
___
## MAC Addressing
A MAC address is a unique hardware identifier assigned to a network interface card (NIC).
Characteristics:
- Unique to each device
- Operates at OSI Layer 2
- Used for local network communication
### MAC Spoofing
MAC Spoofing is the process of changing the MAC address presented to a network.
Common uses:
- Privacy enhancement
- Security testing
- Bypassing MAC-based restrictions
___
## ICMP and PING
ICMP (Internet Control Message Protocol) is used for diagnostics and error reporting.
The ping command uses ICMP to:
- Test connectivity
- Measure latency
- Troubleshoot network issues
Example: ping 8.8.8.8
___
## Network Topologies
### Star Topology
All devices connect to a central switch.
Advantages:
- Easy management
- Easy troubleshooting
- Failure of one device does not affect others
### Bus Topology
All devies are connected in a circular path.
___
## Switches and Routers
### Switch
A switch connects devices within the same LAN.
Functions:
- Uses MAC addresses
- Operates primarily at Layer 2
### Router 
A router connects different network.
Functions:
- Routes packets between networks
- Provides Internet access
- Uses IP addresses
___
## Subnetting
Subnetting divides a large network into smaller logical networks.
Benefits:
- Better network management
- Reduced broadcast traffic
- Improved security segmentation
Important concepts:
- Network Address
- Host Adress
- Default Gateway
___
## ARP (Address Resolution Protocol)
ARP translates IP addresses into MAC addresses within a local network.
Process:
1. ARP Request
2. ARP Reply
3. ARP Cache Update
___
## DHCP (Dynamic Host Configuration Protocol)
DHCP automatically provides network configuration to devices.
Assigned information:
- IP Address
- Subnet Mask
- Default Gatewat
- DNS Server
### DORA Process
1. Discover
2. Offer
3. Request
4. Acknowledge
___
## OSI Model
The OSI Model consists of seven layers:

| Layer | Function |
|---------|---------|
| 7 | Application |
| 6 | Presentation |
| 5 | Session |
| 4 | Transport |
| 3 | Network |
| 2 | Data Link |
| 1 | Physical |

### Practical Examples

| Layer | Example |
|---------|---------|
| 7 | HTTP, HTTPS |
| 4 | TCP, UDP |
| 3 | IP |
| 2 | MAC Address |
| 1 | Cables, Signals |

The OSI Model helps visualize how data moves accross a network.
___
## Packets, Frames, and Encapsulation
### Packet
A packet is the data unit used at Layer 3.
### Frame
A frame is the data unit used at Layer 2.
### Encapsulation
Encapsulation is the process of adding protocol information as data moves down the network stack.
___
## TCP and UDP
### TCP 
Characteristics:
- Connection-oriented
- Reliable
- Error checking
- Ordered delivery
Common use cases:
- HTTPS
- SSH
- FTP
### UDP
Characteristics:
- Connectionless
- Faster
- No delivery guarantee
Common use cases:
- Streaming
- VoIP
- Online gaming
### Choosing Between TCP and UDP
TCP is preffered when reliability is more important than speed.
UDP is preffered when speed is more important than reliablity.
___
## TCP Three-way Handshake
TCP establishes connections using:
1. SYN
2. SYN-ACK
3. ACK
This process ensures both devices are ready to communicate.
### Common TCP Flags
- SYN
- ACK
- FIN
- RST
These flags are essential for connection management and network analysis.
___
## Common Ports

| Port | Service |
|---------|---------|
| 21 | FTP |
| 22 | SSH |
| 80 | HTTP |
| 443 | HTTPS |
| 445 | SMB |
| 3389 | RDP |

Ports identify services running on a system.
___
## Port Forwarding
Port Forwarding allows traffic from the Internet to reach devices inside a private network.
Common uses:
- Self-hosted services
- Remote access
- Home servers
___
## Firewall
A firewall controls network traffic according to predefined rules.
### Stateful Firewall
- Tracks connection states
- Makes decisions based on session context
### Stateless Firewall
- Examines packets individually
- Does not track sessions
___
## VPN (Virtual Private Network)
A VPN creates an encrypted connection between a user and a network.
Benefits:
- Increased privacy
- Secure communication
- Protection on public networks
Common technologies:
- PPTP
- IPSec
___
## Cybersecurity Relevance
Understanding networking fundamentals is essential for cybersecurity because:
- IP addresses and ports are used during enumeration.
- TCP and UDP knowledge helps interpret Nmap scan results.
- ARP knowledge is important for understanding ARP Spoofing attacks.
- DHCP knowledge helps analyze internal networks.
- Firewall knowledge helps understand access control and traffic filtering.
- VPN knowledge helps secure remote communications.
___
## Key Takeaway
Networking fundamentals provide the foundation for understanding how systems communicate and how attackers interact with networks. These concepts are essential for future topics such as Nmap, Wireshark, Active Directory, Web Security, and Penetration Testing.

