# Networking-Project-1-
**Cisco Packet Tracer Project (School Network Design)**


Designed and implemented a small-scale enterprise network based on user and traffic requirements. Performed initial configuration of network infrastructure, including hostname assignment, administrative username and password configuration, SSH-based remote management, and basic device access security.

Developed an IP addressing plan and subnetted the network to efficiently allocate address space and establish distinct broadcast domains. Configured VLANs for Layer 2 network segmentation and deployed Switch Virtual Interfaces (SVIs) to provide Layer 3 inter-VLAN routing and gateway functionality. Configured local default gateways to facilitate communication between network segments and external networks. Implemented firewall rules and access controls to filter inbound and outbound traffic, restrict unauthorized external access, and improve the overall security posture of the network.


**Results:** The completed network implementation achieved 100% connectivity across all required network segments and devices. Connectivity testing confirmed 100% successful ping responses between authorized devices, firewalls, servers and VLANs, demonstrating that the configured SVIs and default gateways were functioning correctly for inter-VLAN communication.


**VLAN 10 (ADMIN)**
IP SCHEME (192.168.10.192/27)
Subnet Mask: 255.255.255.224
Host range .193 - .222
Broadcast .223
SVI Gateway 192.168.10.193
PC-1 IP: 192.168.10.222
Users requirement: 25 



**VLAN 20 (FACULTY)**
IP SCHEME (192.168.10.128/26)
Subnet Mask 255.255.255.192
Host Range .129 - .190
Broadcast .191
SVI Gateway 192.168.10.129
PC-2 IP: 192.168.10.190
User Requirment: 50

**VLAN 30 (STUDENTS)**
IP SCHEME (192.168.10.0/25)
Subnet Mask: 255.255.255.128
Host Range .1 - .126
Broadcast .127
SVI Gateway 192.168.10.1
PC-3 IP: 192.168.10.126
User Requirement: 100

**VLAN 40 (SERVERS)**
IP SCHEME (192.168.10.224/28)
Subnet Mask: 255.255.255.240
Host Range .225 - .238
Broadcast .239
SVI Gateway 192.168.10.225
DNS IP: 192.168.10.226
DHCP IP: 192.168.10.227
WEB/FILE IP: 192.168.10.228
PRINTER IP: 192.168.10.229
Device Requirment: 10



**Point 2 Point (P2P) Communication** 

CORE-SW to Edge Router 
Network 192.168.100.0/30
CORE-SW IP: 192.168.100.1 255.255.255.252
EDGE ROUTER IP: 192.168.100.2 255.255.255.252


EDGE ROUTER TO INTERNAL FIREWALL 
Network 192.168.101./30
EDGE ROUTER IP: 192.168.101.1 255.255.255.252
INTERNAL FIREWALL IP: 192.168.101.2 255.255.255.252

INTERNAL FIREWALL TO ISP 
Network 172.16.10.0/30
INTERNAL FIREWALL IP: 172.16.10.1 255.255.255.252
ISP IP: 172.16.10.2 255.255.255.252 (192.168.10.224/28)
Subnet Mask: 255.255.255.240
Host Range .225 - .238
Broadcast .239
SVI Gateway 192.168.10.225
DNS IP: 192.168.10.226
DHCP IP: 192.168.10.227
WEB/FILE IP: 192.168.10.228
PRINTER IP: 192.168.10.229
Device Requirment: 10
