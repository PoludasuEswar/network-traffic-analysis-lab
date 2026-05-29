# Network Traffic Analysis & Threat Detection Lab

## Objective

To build a small virtual network using a Windows Host and Kali Linux VM and perform packet analysis, reconnaissance detection, and service enumeration using Wireshark and Nmap.

## Lab Environment

* Windows 11 Host
* Kali Linux VM
* VirtualBox Host-Only Network
* Wireshark
* Nmap

## Network Topology

Windows Host (192.168.56.1)

|

Host-Only Network

|

Kali Linux VM (192.168.56.102)

## Activities Performed

### 1. ARP Analysis

Observed ARP requests and replies used for MAC address resolution.

### 2. ICMP Analysis

Captured Echo Request and Echo Reply packets to verify connectivity.

### 3. TCP Handshake Analysis

Observed SYN, SYN-ACK, and ACK packets during TCP session establishment.

### 4. HTTP Traffic Analysis

Hosted a Python HTTP server and analyzed HTTP GET requests and responses.

### 5. Reconnaissance Detection

Performed Nmap scans and identified filtered ports caused by firewall filtering.

### 6. Service Enumeration

Exposed a web service on TCP 8081 and used Nmap version detection to identify:

* HTTP Service
* SimpleHTTPServer 0.6
* Python 3.10.10

## Key Findings

* ARP is required before IP communication.
* TCP uses a three-way handshake.
* Firewalls can cause ports to appear filtered.
* Nmap SYN scans generate SYN → SYN-ACK → RST patterns.
* Service enumeration reveals software and version information useful to attackers.

## Skills Demonstrated

* Wireshark Packet Analysis
* TCP/IP Networking
* ARP Investigation
* ICMP Troubleshooting
* Nmap Reconnaissance
* Service Enumeration
* Security Documentation
