<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# write 100 Networking interview questions with answers in detail. dont do citations and without emoji

Certainly! Here are **100 detailed Networking Interview Questions with Answers**, suitable for beginners to advanced networking professionals.

## BASIC NETWORKING CONCEPTS

### 1. What is a computer network?

A computer network is a group of interconnected devices (computers, servers, routers, etc.) that can share resources and communicate over a communication medium such as cables or wireless signals.

### 2. What are the types of networks?

- **LAN (Local Area Network)**: Limited to small area.
- **WAN (Wide Area Network)**: Covers large geographical area.
- **MAN (Metropolitan Area Network)**: Larger than LAN, smaller than WAN.
- **PAN (Personal Area Network)**: Typically for devices around a single user.


### 3. What is the OSI Model?

The OSI (Open Systems Interconnection) model is a seven-layer architecture that standardizes communication functions into layers:

1. Physical
2. Data Link
3. Network
4. Transport
5. Session
6. Presentation
7. Application

### 4. Explain the functions of each OSI layer.

- **Physical**: Transmits raw bits over a medium.
- **Data Link**: Handles error detection and framing.
- **Network**: Routes packets using IP.
- **Transport**: Ensures reliable data transfer (TCP).
- **Session**: Maintains session between applications.
- **Presentation**: Translates data formats (encryption, compression).
- **Application**: End-user interface (HTTP, FTP).


### 5. What is TCP/IP Model?

A conceptual model that maps to OSI and uses four layers:

1. Network Interface
2. Internet
3. Transport
4. Application

### 6. What is the difference between OSI and TCP/IP models?

- OSI has 7 layers, TCP/IP has 4.
- OSI is a theoretical model; TCP/IP is more practical and widely used.
- Layers differ in functionality and structure.


### 7. What is IP Address?

An IP address is a unique numeric identifier assigned to each device on a network, used to locate and communicate with other devices.

### 8. What are types of IP addresses?

- **IPv4 (32-bit)**: Example: 192.168.0.1
- **IPv6 (128-bit)**: Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334


### 9. What is a MAC address?

A MAC (Media Access Control) address is a hardware address that uniquely identifies each device on a network interface.

### 10. What is the difference between IP address and MAC address?

- **IP Address**: Logical, can change, used for routing.
- **MAC Address**: Physical, permanent, used for device identification.


## NETWORK DEVICES

### 11. What is a router?

A router connects multiple networks and forwards packets based on IP addresses.

### 12. What is a switch?

A switch connects devices within the same network and forwards data based on MAC addresses.

### 13. What is a hub?

A hub is a basic device that broadcasts data to all connected devices, without filtering.

### 14. What is a modem?

A modem modulates and demodulates digital and analog signals for transmitting over telephone lines.

### 15. What is a gateway?

A gateway connects different network architectures and protocols, such as LAN to internet.

### 16. What is a firewall?

A firewall is a security device or software that filters network traffic based on pre-defined rules.

## IP ADDRESSING AND SUBNETTING

### 17. What is Subnetting?

Subnetting divides a large network into smaller, manageable sub-networks or subnets.

### 18. What is the purpose of subnetting?

- Enhances performance
- Improves network management
- Efficient IP address utilization
- Improved Security


### 19. What is CIDR?

Classless Inter-Domain Routing (CIDR) replaces class-based IP addressing. It uses the format IP/mask, like 192.168.0.0/24.

### 20. What is the range of private IP addresses?

- Class A: 10.0.0.0 to 10.255.255.255
- Class B: 172.16.0.0 to 172.31.255.255
- Class C: 192.168.0.0 to 192.168.255.255


### 21. What is the difference between public and private IP?

- **Private IP**: Used within private networks; not routable on the internet.
- **Public IP**: Used on the internet.


### 22. What is the loopback IP address?

127.0.0.1 – Used for locally testing the network stack.

## PROTOCOLS

### 23. What is TCP?

Transmission Control Protocol provides reliable, ordered, and error-checked data delivery.

### 24. What is UDP?

User Datagram Protocol is connectionless and provides faster, but unreliable, communication.

### 25. Differences between TCP and UDP?

| Feature | TCP | UDP |
| :-- | :-- | :-- |
| Reliability | Yes | No |
| Speed | Slower | Faster |
| Connection | Connection-oriented | Connectionless |
| Use Cases | HTTP, FTP | DNS, VoIP |

### 26. What is HTTP and HTTPS?

HTTP is the protocol for transferring web pages. HTTPS is HTTP with encryption using SSL/TLS.

### 27. What is FTP?

File Transfer Protocol enables transfer of files between computers.

### 28. What is DHCP?

Dynamic Host Configuration Protocol assigns IP addresses dynamically to devices.

### 29. What is DNS?

Domain Name System translates domain names (example.com) into IP addresses.

### 30. What is ARP?

Address Resolution Protocol maps IP addresses to MAC addresses.

## NETWORK TOPOLOGIES

### 31. What is a network topology?

The layout pattern of interconnections between devices in a network.

### 32. Types of network topologies?

- Star
- Bus
- Ring
- Mesh
- Hybrid


### 33. What is a Mesh topology?

In mesh, every device connects to every other. Offers redundancy but is complex.

## NETWORK TROUBLESHOOTING

### 34. What tools are used for troubleshooting?

- ping
- traceroute/tracert
- netstat
- nslookup
- ipconfig/ifconfig
- arp


### 35. What is ping used for?

Checks connection status to another device.

### 36. What does traceroute do?

Shows the path and delays of packets reaching the destination.

### 37. What is netstat?

Displays network connections, routing tables, interface statistics.

## ADVANCED NETWORKING

### 38. What is NAT?

Network Address Translation translates private IP addresses to a public IP for access to the Internet.

### 39. What are types of NAT?

- Static NAT
- Dynamic NAT
- PAT (Port Address Translation)


### 40. What is VPN?

A Virtual Private Network extends a private network over a public one using encryption for security.

### 41. What is VLAN?

A Virtual LAN logically segments networks based on function, not location.

### 42. What is Port Forwarding?

It allows access to a specific internal service over the public network using router configuration.

## NETWORK SECURITY

### 43. What is a DMZ in networking?

A demilitarized zone is a subnetwork that exposes external-facing services to the outside while protecting internal LAN.

### 44. What is SSL/TLS?

Security protocols that encrypt data in transit on the web.

### 45. What is SSH?

Secure Shell provides encrypted command-line access to a remote system.

### 46. What is a proxy server?

Acts as an intermediary between user and the internet; used for access control, anonymity, and caching.

## WIRELESS NETWORKING

### 47. What is Wi-Fi?

A wireless networking technology using radio waves to provide high-speed internet and network connections.

### 48. What are Wi-Fi standards?

- 802.11a/b/g/n/ac/ax
Each offers different speeds and frequencies.


### 49. What is SSID?

The network name of a wireless network.

### 50. What is WEP/WPA/WPA2/WPA3?

Wireless encryption protocols. WPA3 is the most secure.

## NETWORK CONFIGURATION AND COMMANDS

### 51. What does ipconfig do?

Displays IP address, subnet mask, and default gateway (Windows).

### 52. What does ifconfig do?

Linux equivalent to ipconfig.

### 53. How to release and renew IP using command?

`ipconfig /release` and `ipconfig /renew` (Windows)

### 54. What is a default gateway?

The IP address where hosts send traffic that goes outside the local network.

## NETWORK COMMUNICATION

### 55. What is Unicast?

One-to-one communication.

### 56. What is Broadcast?

One-to-all communication in the same network.

### 57. What is Multicast?

One-to-group communication using special IP ranges.

## FIREWALLS AND ACCESS LISTS

### 58. What is an ACL?

Access Control List filters traffic based on rules involving IPs, ports, protocols.

### 59. Types of firewalls?

- Packet Filtering Firewall
- Stateful Inspection
- Proxy Firewall
- Next-gen Firewall


## NETWORK PERFORMANCE

### 60. What is bandwidth?

Maximum data transfer rate of a network.

### 61. What is latency?

Time delay in transmitting data from source to destination.

### 62. What is jitter?

Variation in packet arrival times.

### 63. What is throughput?

Actual rate at which data is transferred.

## CLOUD AND VIRTUAL NETWORKING

### 64. What is SDN?

Software-Defined Networking separates the control and data plane to enable centralized control.

### 65. What is CDN?

Content Delivery Network distributes content across multiple locations for faster delivery.

### 66. What is cloud computing?

Delivering network services over the internet with scalable resources.

## NETWORK CABLING

### 67. What are common networking cables?

- Twisted Pair (Cat5, Cat6)
- Coaxial
- Fiber optic


### 68. What is the difference between Cat5 and Cat6?

Cat6 supports higher data rates and less interference.

## IPV6

### 69. What is IPv6?

128-bit addressing that replaces IPv4 due to exhaustion.

### 70. Benefits of IPv6?

- Larger address space
- Improved header format
- Enhanced security


## DNS

### 71. What is a DNS zone?

Portion of the DNS namespace governed by a specific authority.

### 72. What are record types in DNS?

- A: Address record
- MX: Mail exchange
- CNAME: Alias
- PTR: Reverse lookup


## EMAIL PROTOCOLS

### 73. What is SMTP?

Simple Mail Transfer Protocol used to send emails.

### 74. What is POP3 and IMAP?

- **POP3**: Downloads and deletes mail from the server.
- **IMAP**: Keeps emails on the server and syncs across clients.


## INTERVIEW SCENARIOS

### 75. How does data travel from browser to server?

1. DNS lookup for IP.
2. TCP connection established.
3. HTTP request sent.
4. Server processes and responds.

### 76. How does ARP work in LAN communication?

ARP broadcasts to find MAC address corresponding to a known IP.

## LOAD BALANCING AND REDUNDANCY

### 77. What is Load Balancing?

Distributes traffic across multiple servers to ensure availability and scalability.

### 78. What is fault tolerance?

Ensures network remains operational even if one component fails.

## QOS AND TRAFFIC SHAPING

### 79. What is QoS?

Quality of Service prioritizes network traffic to ensure performance for critical services.

### 80. What is traffic shaping?

Controls data flow to ensure steady and efficient transmission rates.

## NETWORK MONITORING

### 81. What are popular network monitoring tools?

- Wireshark
- Nagios
- Zabbix
- SolarWinds


## VIRTUALIZATION

### 82. What is Hypervisor?

Software that creates and runs virtual machines.

## COMMON PORTS

### 83. What ports do common protocols use?

- HTTP: 80
- HTTPS: 443
- FTP: 21
- SSH: 22
- DNS: 53
- SMTP: 25


## SECURITY

### 84. What is MITM attack?

Man-in-the-middle intercepts communication between two parties.

### 85. What is packet sniffing?

Capturing and analyzing network packets.

## TROUBLESHOOTING ISSUES

### 86. Can ping work if DNS is down?

Yes, if the IP is known; DNS is only used for name resolution.

### 87. What does “destination host unreachable” mean?

The route to the destination is inaccessible.

## VIRTUAL PRIVATE NETWORK

### 88. How does a VPN work?

Encrypts data before sending it over the internet to a private server.

## CLOUD NETWORKING

### 89. What is VPC?

Virtual Private Cloud is an isolated network hosted on cloud infrastructure.

## WIRELESS SECURITY

### 90. What is MAC filtering?

Network administrator allows or denies devices based on MAC addresses.

## PRACTICAL INTERVIEW QUESTIONS

### 91. What is the MTU?

Maximum Transmission Unit defines the largest packet size that can be sent.

### 92. What happens when MTU is exceeded?

Packets are fragmented or dropped if DF (Don't Fragment) flag is set.

## IPV6 ADDRESSING

### 93. What is link-local address in IPv6?

Starts with FE80:: and is usable only in local network.

## NETWORK ADDRESSING

### 94. How to calculate subnet mask?

Based on number of hosts needed; examples:

- /24 = 255.255.255.0 = 256 addresses


## STATIC VS DYNAMIC

### 95. What is a static IP?

Manually configured IP on a device.

### 96. What is a dynamic IP?

Assigned by DHCP server.

## PERFORMANCE

### 97. How to check for port availability?

Use `telnet`, `nc` (netcat), or `nmap`.

## FIREWALL RULES

### 98. What is a stateless firewall?

Filters packets independently without context.

### 99. What is a stateful firewall?

Keeps track of connection status and context.

## FINAL QUESTION

### 100. Explain how DNS works.

1. User types URL in browser.
2. Query to local DNS resolver.
3. Resolver checks cache or queries root servers.
4. Travels through TLD and authoritative DNS to get IP.
5. Returns IP to client. Browser connects to web server.

Let me know if you'd like these compiled into a PDF or categorized by difficulty (beginner, intermediate, advanced).

