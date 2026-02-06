# Week 2.5: 2026-02-06

# SUPPORTING NETWORK SERVICES

## 7.1 NETWORKED HOST SERVICES

### File/Print Servers
 
- SMB/Samba (Server Message Block `445`)
- NetBIOS 
- FTP (File Transfer Protocol `20/21`)
    1. FTPS- TLS (Trnasport Layer Security)
    1. SFTP- SSH (Secure Shell)

### Database Servers
 
- Flat File (txt doc) vs Database (excel sheets)
- Relational (fixed format)
    1. Oracle, MySQL, MariaDB
- Non-Relational (free formed)
    1. MongoDB, CouchDB

### Web Servers
- Hosts webpages and websites
- HTTP
    1. Port `80`
- HTTPS
    1. Port `443`
    1. Security through TLS certificates
- URL: Protocol -> FQDN -> File Path

### Hypertext Transfer Protocol Secure

- Transport Layer Security
- Certificate
    1. Certificate Authority (CA)
    1. Lock icon

### Mail Servers `sending`

- Simple(Sending) Mail Transfer Protocol (SMTP)
    1. Port `25`
- SMTPS
    1. TLS certificate security
    1. Port `587` (465)

### Mailbox Servers `receiving`

- Post Office Protocol 3 (POP3): deletes from the server
    1. Port `110`
    1. POP3S: TLS certificate security | Port `995`
- Internet Message Access Protocol (IMAP): keeps on the server
    1. Port `143`
    1. IMAPS: TLS certificate security | Port `993`

### Directory and Authentication Servers

- Lightweight Directory Access Protocol (LDAP)
    1. `389`
    1. LDAPS: TLS certificate security | Port `636`
- Authentication, Authorization, and Accounting (AAA)
    1. Supplicant, Network Access Server (NAS), AAA server
    1. RADIUS: Radius* (Port `1812/1813`) and TACACS+: Terminal* (Port `49`)

### Remote Terminal Access Servers

- SSH(linux/mac)- Secure Shell: Port `22`
- Telnet(dosen't encrypt): Port `23`
- Terminal Emulation Software: PuTTY (Protocol interface)
- RDP(windows)- Remote Desktop Protocol: Port `3389`

### Time Servers

- NTP- Network Time Protocol: Port `123` | NTS- secure port `4460`
- Stratum levels of accuracy: 1, 2, 3, etc.

### Network Monitoring Servers

- SNMP- Simple Network Management Protocol
    1. Port `161`
    1. Port `162`- TRAP messages
    1. v1, v2, v3
- Syslog: Port `514`

## 7.2 INTERNET AND EMBEDDED APPLIANCES

### Proxy Servers

- Translates full HTTP requests on behalf of network client nodes
- Content filtering

### Spam Gateways and Unified Threat Management

- Firewall
- SPF, DKIM, DMARC to verify email authenticity (to filter out spam)
- UTM(Unified Treat Management)- Single appliance to manage aspects of network security
    1. Firewall, antivirus, anti-malware, IDP/IPS, etc.

### Load Balancers

- Balance workload across multiple systems

### Legacy Systems

- EOL (End of Life) / EOSL (End of Service Life): No longer supported by OEM or developer

### Embedded Systems and SCADA

- Specific task functions
- ICS- Industrial Control System
    1. Power
    1. HVAC
    1. Cooling pumps
- OT(Operational Technology) networks
- SCADA(Software made to manage more than one ICS)- Supervisory Control and Data Acquisition
    1. Monitoring two or more ICSs

### Internet of Things Devices (more attack vectors)

- Global network
    1. Wearable devices
    1. Home appliances
    1. Vehicles
- Hub/control system
- Smart device
- Communication
**low power devices**
    1. Zigbee
    1. Z-Wave

## 7.3 TROUBLESHOOT NETWORKS

### Troubleshoot Wired Connectivity

- Cable and NIC Issues
    1. Physical damage and connectivity
    1. Wall port to patch panel to switch
- Port Flapping Issues: Up/down state continuous transition

### Troubleshoot Network Speed Issues

- Speed can be limited by:
    1. Configuration of port
    1. Limitations of NIC and switch port
    1. Limitations of cabling
    1. Interference
    1. Malware

### Troubleshoot Wireless Issues

- Intermittent connectivity
- Configuration
    1. Band selection
    1. Mismatch of standards
- Signal strength(wifi tester): RSSI (received signal strength indicator)
- Wi-Fi analyzer

### Troubleshoot VoIP Issues

- Latency- delay
- Jitter- variation in delay over time
- QoS(Quality of Service): Prioritization of traffic

### Troubleshoot Limited Connectivity

- Scope of issue
- Configuration of cables
- VLAN configuration
