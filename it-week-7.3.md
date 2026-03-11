# Week 7: 2026-03-11

# Managing Security Settings

## 19.1 Account Security

### Password Best Practices

- Make password sufficiently long
- Use passphrase, rather than password
- NO personal info
- Expiration requirements

### End User Best Practices

- Log off when not using system
    - START+ L keys
- Secure critical systems from theft
- Secure PII and passwords
- Use password manager

### Restrict User Permissions

- Least privilege principle
- Fewest number of accounts with administrative rights as possible
- Ensure UAC or sudo features are enabled

### Change Default Administrator Account and Password

- "Administrator" in WINDOWS and root in Linux/Unix; accounts should be changed and disabled from use
    - If not possible, change the default password
- Create unique accounts with administrative access for admin use
- Separation of duties

### Disable Guest Account

- Guest accounts do not require authentication
- Disable all guest account use
    - Accountability for all users with unique accounts for each user

### Account Policies

- Restrict login times
    - Working hours/logon hours
- Account expiration
- Failed login attempt lockout
- Concurrent logins
- Use timeout/screen locks

### Unused Services

- Disable all unused services
- Includes wi-fi, Bluetooth, and NFC connections
- Disable file and print services not necessary to operation of the system

## 19.2 Workstation Security

### Execution Control

- Restrict use of elevated permissions
- "Run As administrator"
    - UAC warning
    - Asmin account login requirement

### Trusted/Untrusted Software Sources

- Download from trusted sources
- Scan all downloads
- Verify digital signatures and/or file hash
- Remove all unnecessary software applications

### AutoRun and AutoPlay

- Disable Autorun and AutoPlay
    - Autorun.inf `script`
- Configured under a drive's property dialog box

### Windows Defender Antivirus

- Detect and prevent execution of malware
- Host-based system
    - Settings and rules are only for that single node, unless managed through group policy

### Windows Defender Antivirus Updated Definitions

- Definitions {library of all known viruses}
    - Identify malware using signatures and heuristic models
    - Daily and sometimes hourly updates
- Scan engine
    - Improves software performance

### Activating and Deactivating Windows Defender Antivirus

- Temporary disable
- Real-time protection slider
- Third-party antivirus/ antimalware software installed

### Windows Defender Firewall

- Inbound/outbound Rules
- Port security
- Application security
- Triggers {setup a flag in the antivirus}
`intrusion detection and preventition`

### Encrypting File System

- Built into Windows to protect data at rest
    - Not available on Home Edition
- Advanced button of file's property dialog box

![efs_demo](/assets/efs_demo.png)

![efs_demo](/assets/efs_denied.png)

### Windows Bitlocker and BitLocker To Go

- Included with all versions of Windows except Home edition
- Full disk encryption software
    - Password protected
    - Recovery Key backup- safe location outside of the disk being protected: TPM can be used
- To Go- removable drive version

## 19.3 Browser Security

### Browser Selection and Installation

- Trusted sources
    - Verify download using hash or digital signature
- Untrusted sources
    - May expose system to malware including advertising spam
    - Should not be used

### Browser Settings

- Sign-in and data sync
    - Cross platform and device sync
- Password manager
    - Holds passwords securely and can sync across devices

### Browser Extensions and Plug-ins

- Extension- Add or change a feature
- Plug-in- Support various types of content
- Trusted sources
    - Browser web store
- Only enable when needed

### Browser Patching

- Updates- processed through OS updates or separately
- Auto update upon launch
- About menu

### Secure Connections and Valid Certificates

- SSL/TLS certificate
- Certificate Authority (CA)
- Validity
- Asymmetric Algorithm
    - RSA
    - ECC

### Browser Privacy Settings

- Cookies
- Pop-up blockers
- Ad blockers
- Proxy settings
- Clearing cache
- Private browsing
    - Does not hide your web browsing from your ISP!

## 19.4 Troubleshoot Workstation Security

### Malware Vectors

- Virus
- Boot sector virus
- Trojan
- Worm
- Fileless malware
    - Lives in memory, not within a file

### Malware Payloads

- Actions does the malware accomplish
- Backdoor
    - Ports, services, accounts
- Adware
- Spyware and keyloggers
- Rootkits

### Ransomware and Cryptominers

- Hold data "hostage" until ransom is paid
- Mine cryptocurrency using host resources such as CPU and GPU

### Troubleshoot PC Security Symptoms

- Performance symptoms
- Application crashes
- Service issues
- File system errors and anomalies

### Desktop Alerts and Notifications

- Push notifications to the OS
- False or fake alerts that confuse user

### Endpoint Monitoring Solutions

- Monitor for changes on endpoint nodes
- Provide early alerts that something may be wrong
- EDR/MDR/XDR

### Troubleshoot Browser Symptoms

- Redirection to another webpage or website
- Certificate warnings
    - Not necessarily an indication of malicious website, but should be looked at closely before proceeding

### Best Practices for Malware Removal

1. Investigate and verify malware symptoms.
1. Quarantine infected systems.
1. Disable System Restore in Windows.
1. Remediate infected systems:
    - Update anti-malware software.
    - Scanning and removal techniques (e.g., safe mode, Reimage/ Reinstall environment).
1. Schedule scans and run updates.
1. Enable System Restore and create a restore point in Windows.
    - Newer Windows OS prefer that a user use the File History or Reset Windows options instead of using system restore.
1. Educate the end user.
-   Most malware is discovered via on-access scanning by an antivirus product. If the malware is sophisticated enough to evade automated detection, the symptoms listed above may lead you to suspect infection.

### Infected Systems Quarantine

- Quarantine is not removal
- Isolate the system from the network
    - Physical isolation, if possible, logical isolation at a minimum
- Disable System Restore

### Malware Removal Tools and Methods

- Updated antivirus/anti-malware software
- Use of a third-party application or removal tool
- Scan from another system
- Recovery options
    - WinRE, restore from backup
        - Backups should be carefully evaluated, as they may also contain the malware
- OS reinstallation
    - Erase, repartition, reinstall

### Malware Infection Prevention

- On-access scanning
- Schedule regular scans
- Re-enable System Restore and Services
- Educate end user
    - Do not assign blame
    - Educate not alienate
