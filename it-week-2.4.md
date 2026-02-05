# Week 2.4: 2026-05-02

# Configuring Network Addresssing and Internet Connections

## 6.1 INTERNET CONNECTION TYPES

### Internet Connection Types and Modems

- IXP
- ISP (Internet Service Provider)
- Modem- Establish connection between router WAN interface and ISP


![flow diagram](/assets/flow.png)

`yellow`-lan | `blue`-wan

### Digital Subscriber Line Modems (DSL)

- Public switch telephone network (PSTN)
- Copper two-pair cabling
- Asymmetric- Faster download than upload
- Symmetric- Same upload and download speeds
- Filter/Splitter- Voice and data

### Cable Modems

- Cable TV network
- Coaxial cable with F-type connector
- DOCSIS

### Fiber to the Curb and Fiber to the Premises

- FTTC- copper cabling into facility or home
- FTTP- full fiber cable into facility or home
- Optical Network Terminal- ONT

### Fixed Wireless INternet Access

- Satellite- High latency connection
    1. Geostationary orbital satellite
    1. Low Earth Orbital (LEO) satellite
- Wireless Internet Service Provider (WISP)
    1. Long range Wi-Fi connectivity

### Cellular Radio Internet Connections

- 3G
    1. GSM 
    1. CDMA (phone comes with the provider)
- 4G
    1. LTE support GSM and CDMA
- 5G
    1. mMIMO (more antennas than usual)

### Routers

- IP address-based forwarding
- Broadcast domains

### Firewalls

- ACL- List of rules to allow/deny traffic
- Based on packet header information
    1. IP
    1. MAC
    1. Protocol
    1. Port

![firewall demo](/assets/firewall_interface.png)

## 6.2 TCP/IP CONCEPTS

- Suite of communication protocols

 ![Network stack](/assets/network_stack.png)

### Link or Network Interface Layer

- Local network segment communications (router <-> pc)
- MAC address used for forwarding
- PDU- Frame

![osi model](/assets/osi_model.webp)

### Internet layer

- Communication between network segments
- IP Address used for forwarding
- PDU- Packet

### Transport Layer

- TCP vs UDP protocols
- PDU- Segment

### Application Layer

- High level functionality for communications
- PDU- Data

### IPv4 Addressing

- 32-bit, dotted decimal notation
- 4 octets
- 0-255 in each octet

![ipv4 frame](/assets/ipv4_frame.png)

### Network Prefixes

- Network ID-network the node belongs to
- Host ID- individual node
- Network mask- Subnet mask (to know which IP addresses are available)
**as the number decreases the amount of available addresses increases**

![ipv4 breakdown](/assets/v4_breakdown.png)

### Public and Private Addressing

- Private Ranges- Used within a LAN environment
    1. 10.0.0.0 to 10.255.255.255 (Class A)
    1. 172.16.0.0 to 172.31.255.255 (Class B)
    1. 192.168.0.0 to 192.168.255.255 (Class C)
- Network Address Translation (NAT) (developed to combat the ipv4)
    1. Private to public
    1. Public to private

![subnet class](/assets/subnet_class.png)

### IPv4 Host Address Configuration

- IP assigned to node
- Subnet mask
- Default gateway
- DNS server IP

![ip config demo](/assets/ip_config_demo.png)

### Static Versus Dynamic Host Address Configuration

- Static- Manual configuration of NIC
- DHCP- Service is used to configure NIC
- APIPA- Automatic Private IP Addressing (to give an ip address from the range<sub>2</sub>)
    1. 169.254.0.1 to 169.254.255.254

![lan demo](/assets/lan_demo.png)

### SOHO Router Configuration

- Interfaces
    1. Multiple interfaces to connect various networks
- Console(text-based) vs. GUI/Web URL

### IPv6 Addressing

- 128-bit addressing; hex notation
- Eight 16-bit values separated by colons
- Prefixes
    1. Pre-determined address for special purposes
- Dual stacking
    1. IPv4 and IPv6

## 6.3 NETWORK COMMUNICATIONS

### Protocols and Ports

- Transport layer
- 65,536 ports (0-65535)
- Facilitate simultaneous communications


### Transmission Control Protocol (TCP)

- Connection-oriented, guaranteed delivery
- Flags to control
- Three-way handshake
    1. SYN - SYN/ACK - ACK
- Examples: HTTPS, SSH, FTP, etc.

### User Datagram Protocol (UDP)

- Connectionless, non-guaranteed delivery
- No sequencing or acknowledgments
- Examples: DHCP, DNS, TFTP, etc.

### Well-Known Ports

| Port | Protocol |
|---|---|
|20/21|FTP|
|22|SSH|
|23|Telnet|
|25|SMTP|
|53|DNS|
|67/68|DHCP|
|80|HTTP|
|110|POP3|
|137/139|NetBIOS|
|143|IMAP|
|389|LDAP|
|443|HTTPS|
|445|SMB|
|3389|RDP|

## 6.4 NETWORK CONFIGURATION CONCEPTS

### DHCP Functions

- Scope: range ie. how many ip addresses are available?
- Leases: how long?
- Reservations: MAC address needed
- DORA: **D**iscover **O**ffer **R**equest **A**cknowledge

### Domain Name System

- FQDN (fully qualified domain name) or Host Name to IP Address
- TLD

### DNS Queries

- Name resolution
    1. HOSTS
    1. Local server
    1. Authoritative server
    1. TLD server
    1. Root name server

### DNS Record Types

- SOA (Source of Authority)
- A (Assigning an IP address)
- AAAA (%ipv6)
- CNAME (different names for the same IP)
- MX (mail exchange)
- TXT (add text to messages)
- SRV (specifies the host name for ports and services)
- NS (lists the authoritative DNS server you'll be referencing)
- PTR- Reverse A/AAAA (`pointer` for nslookup)

![dns manager](/assets/dns_manager.png)


### DNS Spam Management Records
 
- Sender y Framework (SPF)
- Domain Keys Identified Mail (DKIM)
- DMARC

### Virtual LANs

- Increased performance
    1. Broadcast domain split
- Increased security
    1. Control of communication between networks and nodes
- Implemented on switch

### Virtual Private Networks

- Remote connection method for security
- Secure tunneled traffic over non-secure connections
    1. Public Wi-Fi

![vpn diagram](/assets/vpn_diagram.png)


