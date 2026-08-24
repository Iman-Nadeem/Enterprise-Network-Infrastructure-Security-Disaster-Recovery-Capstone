# Enterprise-Network-Infrastructure-Security-Disaster-Recovery-Capstone
**Enterprise Network Design & Configuration – GNS3**
📌 **Project Overview**

This project is an enterprise network design and configuration assignment developed using GNS3. The network represents a large organization with multiple branch offices, Headquarters, a Data Center, a DMZ, firewalls, VLANs, WAN connectivity, enterprise services, and centralized network management.

The project focuses on designing a secure, scalable, reliable, and manageable enterprise network.

🏢**Network Sites**

The topology includes:

LHR – Lahore Branch
KHR – Karachi Branch
ISB – Islamabad Branch
PSH – Peshawar Branch
HQ – Headquarters
Data Center
DMZ
Network Operations Center (NOC)
🌐 **VLAN Structure**
VLAN	Purpose
10	Management
20	Finance
30	Sales
40	IT
50	Voice / VoIP
60	Printers
70	Guest
80	Servers
90	Network Management
100	DMZ / Public Services
📡 IP Addressing

Each branch uses a dedicated IP address range:

Site	Network
LHR	10.10.0.0/16
KHR	20.10.0.0/16
ISB	30.10.0.0/16
PSH	40.10.0.0/16
HQ	50.10.0.0/16
WAN	10.255.0.0/16
Data Center	10.100.0.0/24
DMZ	10.200.0.0/24
🔗 WAN Connectivity

Dedicated /30 networks are used for router-to-router and router-to-firewall connections.

LHR: 10.255.10.0/30 and 10.255.10.4/30
KHR: 10.255.20.0/30 and 10.255.20.4/30
ISB: 10.255.30.0/30 and 10.255.30.4/30
PSH: 10.255.40.0/30 and 10.255.40.4/30
🔥 Firewall & DMZ

Firewalls are implemented to control traffic between internal networks and external networks.

The DMZ contains public-facing services:

Web Server
DNS Server
FTP Server
Mail Server
Application Server

DMZ network:

10.200.0.0/24

🖥️ Data Center

The Data Center provides centralized enterprise services, including:

Web Server – 10.100.0.11
DNS Server – 10.100.0.12
Application Server – 10.100.0.13
File Server – 10.100.0.14
Database Server – 10.100.0.15
🛡️ Security Features

The project includes:

VLAN segmentation
Access Control Lists (ACLs)
Firewall protection
DMZ isolation
SSH-based device management
Port security
Guest network isolation
Secure management VLAN
Disabled unused ports
Network monitoring
Configuration backups
📊 **Network Management**

A Network Operations Center (NOC) is used for centralized monitoring and management.

The NOC is responsible for:

Network monitoring
Fault detection
Troubleshooting
Device management
Performance monitoring
Configuration management
Security monitoring
🧪 **Troubleshooting**

Major troubleshooting scenarios include:

Incorrect IP addressing
VLAN configuration errors
Trunking problems
OSPF adjacency issues
Routing failures
WAN connectivity problems
Firewall and ACL issues
DNS/DHCP problems
Port security issues
DMZ connectivity problems
Duplicate IP addresses

Common troubleshooting commands include:

show ip interface brief
show running-config
show vlan brief
show interfaces trunk
show ip route
show ip ospf neighbor
ping
traceroute
🚨 **Disaster Recovery**

The project considers different disaster scenarios, including:

Router failure
Firewall failure
WAN link failure
Switch failure
Server failure
Power failure
Configuration failure
Cybersecurity incidents

Backup configurations and recovery procedures are considered to reduce network downtime.

🎯 **Learning Outcomes**

Through this project, the following skills were developed:

Enterprise network design
Cisco router and switch configuration
VLAN implementation
IP addressing and subnetting
OSPF routing
WAN configuration
Firewall and DMZ implementation
Network security
Network troubleshooting
Enterprise service configuration
NOC and network management
Disaster recovery planning
🛠️ Technologies & Tools
GNS3
Cisco IOS
Virtual Network Devices
Wireshark
Ping / Traceroute
CLI-based Network Configuration
