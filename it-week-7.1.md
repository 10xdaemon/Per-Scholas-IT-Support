# Week 7: 2026-03-09

# Configuring SOHO Network Security

## 18.1 ATTACKS, THREATS AND VULNERABILITIES

### Vulnerabilities

- Non-compliant systems
    - Deviations from baselines
- Unprotected systems
    - Missing or improperly configured security controls
- Software
    - Application code issues
- Zero-Day vulnerabilities `holes present from day one`
- Unpatched and End of Life OS's
    - No updates or no longer supported by developer
- Bring Your Own Device
    - Personal devices may not be maintained by owner

### Social Engineering

- Hacking the human
    - Manipulation or intimidation of users to reveal confidential info
- Impersonation
- Dumpster diving
- Shoulder surfing
- Tailgating/piggybacking

### Phishing and Evil Twins

- Phishing
    - Spear phishing- targeted phishing campaign
    - Whaling- executives and those with influence within the organization
    - Vishing- voice call to illicit confidential information
    - SMiShing- use of SMS or text messages
    - Quishing- use of fake QR codes to trick targets
- Evil Twin- similar SSID for wi-fi network that allows attacker to snoop on network traffic

### Threat Types

- External
- Internal
- Footprinting
    - Gathering information about the organization
- Spoofing
    - Masquerade as a trusted user or system
    - IP and MAC spoofing
- On-path attacks `man in the middle`
- DoS(denial of service)/DDoS(distributed denial of service)botnet attacks

![Threat Demo](/assets/threat_demo.png)

### Password Attacks

- Plaintext passwords
    - Services like Telnet do NOT encrypt traffic
- Dictionary- use of a dictionary list to crack passwords
    - RockYou.txt file contains over 14 million passwords
    - New "RockYou2024" contains over 10 billion passwords
- Brute force
    - Any means necessary; every possible combination and substitution

![password attack](/assets/password_attack.png)

### Cross-site Scripting Attacks

- Exploits trust of scripts that appear to originate from website being visited
- Malicious script is inserted into the site and is executed by the browser, as it thinks the malicious script originated from the trusted website

### SQL Injection Attacks

- Structured Query Language used to query database systems
- SELECT, INSERT, DELETE, UPDATE
- Manipulates database into an undesired operation
- Prevention
    - Input validation and sanitization
    - Parameterized queries
    - Stored procedures- precompiled SQL code

## 18.2 WIRELESS SECURITY PROTOCOLS

### Wi-Fi Protected Access

- TKIP- Temporal Key Integrity Protocol
    - RC4 encryption of traffic; replaced by AES in WPA2
- AES- Advanced Encryption Standard
    - Symmetric encryption algorithm
- WPA2-
    - Uses AES vice RC4; CCMP replaced TKIP
- WPA3 `most secure`
    - SAE authentication
    - AES CCMP replaced by AES GCMP encryption

### Wi-FI Authentication Methods

- WPA2 pre-shared key (PSK)
    - Passphrase is used to securely join network
- WPA3 personal
    - Passphrase is still used
    - Perfect forward secrecy
        - Compromised keys cannot be used to crack previously encrypted traffic as keys change with every transmission

### Enterprise Authentication Protocols

- ENT or Enterprise
- Uses IEEE 802.1x Extensible Authentication Protocol (EAP)
- AAA server can be used to authenticate users or devices before allowing connection to network
- RADIUS and TACACS+ are popular solutions
- Multifactor authentication can also be implemented

### RADIUS, TACACS+, and Kerberos

- Remote Access Dial In User Service
    - Uses UDP port 1812 to forward user credentials to server for authentication
- Terminal Access Controller Access Control System Plus
    - Uses TCP port 49 to authenticate users
    - Primarily used for device remote access authentication
- Kerberos `sso microsoft`
    - Proprietary Microsoft user authentication service
    - UDP port 88, but can be implemented using TCP, if necessary

## 18.3 SOHO ROUTER SECURITY

### Home Router Setup

- Physical placement
    - Highest elevation to avoid furniture and human interference
    - Centralized in office or home to provide best coverage
- ISP connection to WAN port, then plug in power
- Login portal
    - Web-based utility or wizard to aide in setup
    - Change the default password after login

### Firmware Update

- Firmware and driver should be kept updated
- You can manually download and apply the update; otherwise, there may be a menu option to update it through the web GUI
- Power to device should be maintained throughout the process

### Home Router LAN and WLAN Configuration

- SSID- network name
- Encryption Selection
    - WPA2 or WPA3 should be used
- Strong passphrase
- Disable guest access
- Select channels to minimize interference, or leave on auto

### Home Router Firewall Configuration

- Inbound and outbound ACL's
- Rules may be based on:
    - IP source or destination
    - Port source or destination
    - Content filtering

### Home Router Port Forwarding Configuration

- Static vs DHCP reservations
- Port forwarding
    - Traffic from an internet facing port directed to specific host on internal network
    - Can also forward traffic to specific internal port
- Disable all unused ports

### Universal Plug-and-Play

- Allows devices the ability to configure ACL rules for their own communications traffic
- If not required, disable this option

### Screened Subnets

- Formally known as DMZ's
- Allows administrators to direct traffic to specific logical segments of the network
- Can be used to isolate web facing hosts on network, while preventing internal network access from the internet

## 18.4 ADDITIONAL SECURITY MEASURES

### Physical Access Control

- Perimeter security
- Access control vestibule
    - Two door access system, only one door can be opened at a time
- Magnetometers
    - Metal detectors
- Security Guards

### Lock Types

- Key
- Electronic
- Badge reader
    - NFC, RFID, magnetic
- Mobile digital key
    - Commonly seen in hotel apps
- Biometric
    - Fingerprint, Palm, Retina, Facial, Voice
    - Type 1 vs Type 2 errors
- Kensington lock, chassis lock, lockable equipment racks

### Alarms and Surveillance

- Circuit
- Motion
- Proximity
- Duress
    - Panic button
- Video
    - CCTV, Wireless, or cabled IP cameras
- Lighting
    - Illuminates' area for better surveillance
