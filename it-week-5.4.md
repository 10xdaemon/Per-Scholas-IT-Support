# Week 5: 2026-02-26

# SECURITY WINDOWS

## 15.1 Logical Security Concepts

### Logical Security Controls

- IAM
    - Identification, Authentication, Authorization, Access Control
- Access control lists
- Implicit deny
    - Deny everything unless a rule says to allow it
- Least privilege
    - Provide the right access for each user or system 
    - Nothing more, nothing less

### Information Security

- Vulnerability
    - Any weakness that, if exploited, could cause damage or a security breach
- Threat
    - Potential to exploit a vulnerability and breach the system
- Risk
    - Likelihood and impact of threat actor exercising vulnerability

![Threat Chart](/assets/threat_chart.png)

### Hashing and Encryption Conecpts

- Symmetric
    - Single key
- Asymmetric
    - Key pair
- Hash
    - Function takes any amount of data and produces a fixed length output (digest)
    - Does NOT contain the actual data
    - Used primarily for integrity checks

### Digital Signatures and Key Exchange

- Digital signature
    - Proves a message or digital certificate has not been altered or spoofed
- Key exchange
    - Allows two systems to exchange a key used for encryption
    - Asymmetric algorithm keys used to encrypt symmetric keys for the exchange

### User and Group Accounts

- Local
    - Only used for accessing a single system or entity
- Microsoft account 
    - Profile can sync through an online portal
- Security groups
    - Collection of accounts that will be assigned similar permissions
        1. Administrator group: All files and objects in system
        1. Guest group: Legacy group with same permissions as User group
        1. Power user group: Between Users group and full administrator
- Local Users and Groups
- net user commands (manages accounts)
    - Manage accounts using command line utility

### User Account Control

- Just-in-Time access
- Privileged Access Management
    - UAC provides implementation of JIT and PAM in Windows 
    - User must confirm UAC pop up for change to be made

### Authentication Methods

- Proving you are what you say you are
- Zero trust framework
    - No automatic trust of user or device
- Multifactor authentication
    - Something you know, something you have, something you are, something you do, somewhere you are/aren't
- 2-step verification
- One-time passwords
- Authenticator applications
- Hard token authentication

## 15.2 WINDOWS SECURITY SETTINGS

### Windows Login Options

- Local, Windows network, remote login
- Username and password
- Windows Hello
    - Pin
    - Fingerprint
    - Facial recognition
    - Security key
- Single sign-on
- Security Assertions Markup Language (SAML)

### Windows Domains and Active Directory

- Domain controllers
    - Server that stores a copy of the network information for Active Directory
- Member servers
    - Servers that are members of the domain but do not store a copy of Active Directory info
- Security groups
- Organizational units (OUs) `refers to the folders`

### Group Policy and Login Scripts

- Group Policy Management console
- Update policy
    - gpupdate command `admin`
    - gpresult command
- Login scripts

## 15.3 WINDOWS SHARES

### Workgroup Setup

- Join a workgroup
    - System Properties menu
- Network discovery and advanced sharing
    - File sharing
    - Printer sharing

### File Share Configuration

- Right-click item and select Give access to 
    - Select account, and then permissions
- Customize permissions 
    - Properties menu: Share tab

### Permissions Inheritance

- Parent folder permissions trickle down to child subfolders and files
- Share permissions for across network access
    - NTFS permissions enforced for network and local access
- Most restrictive permission becomes effective permission
    - If one permission not allowed, the other allow, then not allow will be effective

![Permissions Inheretance](/assets/perm_inher.png)

### Network Browsing and Mapping Drives

- Network object in File Explorer `Z: Drive`
    - Shows any networked device connected to the same network
- Mapped Drives
    - Network shares that can be reconnected every time a user logs in
- net and net use command

### NTFS versus Share Permissions

- Share permissions only apply when accessed over a network
- NTFS permissions are applied to the resource on local and network access
- NTFS permissions are set on Security tab of Properties dialog
    - Read, write, execute
- Explicit vs implicit deny or allow

### Domain Setup

- Control and permissions set through group policy and domain security policy
- Account settings app
    - Access work or school option
- Can also use System Properties menu

### Home Folder

- Store files on server rather than local workstation: Centralized storage allows monitoring and regular back up
- Can be mapped using the profile settings of user account

### Roaming Profiles and Folder Redirection

- Allows users to log in anywhere on network and have access to their files, applications, and settings
- Redirect profile folders to server-based storage for resiliency
