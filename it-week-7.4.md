# Week 7: 2026-03-12

# MODULE 20: Supporting Mobile Software

## 20.1 Mobile OS Security

### Screen Locks

- Swipe to access
    - No authentication
- PIN
    - 4–6-digit numerical access code
    - Password/Passphrase is preferred
- Fingerprint
- Facial recognition
- Pattern lock
    - Connect the dots on screen in a pattern
- Failed login attempts
    - Locks device for a period after failed login attempts

### Mobile Security Software

- Patching/OS updates
    - Regular updates of OS and applications
- Antivirus/anti-malware
- Firewall

### Enterprise Mobility Management

- EMM allows remote management and control of device
- BYOD
    - Personal device connected to corporate network and systems
    - Could require access to the device for monitoring by company
- COBO
    - Business owned and for business use only
- COPE
    - Business owned, but personal activities like social media are allowed under AUP
- CYOD
    - COPE but user can select the device type they prefer (Android or iPhone) 

### Mobile Device Management

- MDM applies security policy to the mobile device
- MDM can:
    - Manage device settings
    - Enforce security policies
    - Control app installations and permissions
    - Regulate network access
    - Monitor compliance
    - Facilitate remote management

### Two-Factor Authentication

- Two different authentication credentials
- Something you are and something you have, etc.
- Push notification or authenticator application
    - Microsoft and Google both have their own authenticator apps
    - Many third-party services are available like RSA's SecureID

### Mobile Data Security

- Device encryption
    - Apple- default on and cannot be switched off
    - Android- default for file level encryption
- Remote backup applications
    - Cloud services
        - iCloud
        - Google Drive
        - Microsoft OneDrive
        - DropBox
    - Backup to local computer

### Locator Apps and Remote Wipe

- GPS/IPS/Wi-fi/Cellular location services
- "Find My Phone/Device" apps for both Apple and Android
- Remotely
    - Lock
    - Play sound
    - Wipe device

## 20.2 Troubleshoot Mobile OS and App Software

### Mobile Device Troubleshooting Tools

- Settings app
    - Down from Top
    - Up from Bottom
- Reboot
- Factory reset
- Battery life
    - Battery health report
    - Smart Charge technology

### Troubleshoot Device and OS Issues

- OS fails to update
- Device randomly reboots
- Device slow to respond
- Auto-rotate screen not working

### Troubleshhot App Issues

- Fail to launch, close, or crashes
    - Android- Settings > Apps > Force Stop or Disable
    - Apple- swipe up from bottom of screen, swipe app card up to close
- Clear cache
- Fail to install
    - Verify storage and permissions
        - Corporate devices may have restrictions
    - Confirm connectivity or restriction to download only over wi-fi

### Troubleshoot Connectivity Issues

- Signal strength and interference
- Configuration issues
- Troubleshooting NFC
- Troubleshooting AirDrop
    - Everyone, Contacts Only, Off
    - Verify range to device
        - Bluetooth
    - Android has a feature like AirDrop called Nearby Share

## 20.3 Troubleshoot Mobile OS and App Security

### Root Access Security Concerns

- Root
    - Primarily refers to Android OS root level access to bypass controls
- Jailbreak
    - Primarily refers to iOS device administrative access to bypass controls
- Developer mode
    - This is not rooting or jailbreaking
    - Specifically used for diagnostic data access and advanced configuration settings

### Mobile App Source Security Concerns

- App spoofing
- Enterprise apps
- APK sideloading
- Bootleg app stores
- Users should only download apps from trusted sources and verify the app digital signature, if possible

### Mobile Security Symptoms

- Excessive ads, fake security warnings
- Unexpected app behavior
- Leaked personal files/data
- Location services
    - Geotagging photos and videos

# MODULE 21: Using Data Security

## 21.1 Data Backup and Recovery

### Backup Operations

- Protects against data loss
- Backup scheme
    - Series of backup types and timelines
    - IE hourly snapshots of VM's and weekly backups of data files
- File History
    - Versioning
- Backup and Restore Center

### Backup Methods

- Frequency- how often
- Retention- how long to hold on to backup file
- Backup chains
    - Full- all data
    - Incremental- only changes since last backup of any type
    - Differential- changes since last FULL backup
- Synthetic full backup
    - Series of backups that append changes from incremental backup to the end of the original full backup
        - IE: Full backup on the first of month at 7am and then incremental backups every 3 hours for remainder of month

![backup_table](/assets/backup_table.png)

### Backup Media Requirements

- Media reuse
    - Magnetic tape, internal/external hard drives, NAS/SAN, cloud
- Grandfather-Father-Son (GFS)
- On site vs off site storage
- 3-2-1 rule
    - Popular scheme consists of
    - 3 full copies of data(includes production system), 2 different media types,  offline and offsite stored backup
        - IE: Production system, External hard drive backup stored on site, and a backup of data to the cloud

### Backup Testing and Recovery Best Practices

- Always test backups will provide restoration of data in the event of a loss
- Verify data after backup
- Test periodically to ensure procedural compliance
- Recovery options
    - In-place
    - Alternative system/site location

## 21.2 Data Handling Best Practices

### Regulated Data Classification

- PII
    - US Privacy Act and GDPR regulatory compliance
- PGI
    - Social security, passport, driver's license
- PHI
    - Protected health information
    - HIPAA compliance in US
- Credit card and bank card transactions
    - PCI-DSS
- Best practices and requirements

### Prohibited Content and Licensing Issues

- Information not applicable to work
    - Obscene or illegally copied/pirated
- End-user license agreements (EULA)
- License compliance
    - Personal vs corporate use
    - Single user vs multiple user license
- Open-source license
    - Does not necessarily indicate free cost to use
- Digital rights management
- Non-disclosure agreement (NDA)

### Incident Response

- Standard procedures and policy to follow when something occurs like a data breach or system outage
- Incident response plan
- CIRT/CERT/CSERT
    - Team of responders identifies specifically to handle various situations

### Data Integrity and Preservation

- Forensics
    - Collection of evidence from a computer system or network to a standard that will be accepted in a court of law
    - Certified technicians and facilities for processing
- Document, document, document
    - Pictures, videos, notes
- Order of volatility
- Chain of custody
    - Positive, documented, control over evidence to prevent tampering and documents collection, storage, processing, and even transport of said evidence

### Data Destruction Methods

- Sanitization
- Re-formatting may not be sufficient
- Erasing/wiping
- Low level format
    - Secure erase
    - Instant secure erase

### Disposal and Recycling Outsourcing Concepts

- Drilling
- Shredding
- Incineration
- Degaussing
    - Only works on magnetic media like HDD and magnetic tape, not SSD or optical media
- Certificate of destruction/recycling

## 21.3 Artifical Intelligence

### Application Integration

- AI can analyze data and provide recommendations
- Use of third-party providers like website add-on chatbot
- NLP, ML, Computer Vision

### Policy

- Organizational policy should be designed to dictate the legal and ethical use or banning of AI solution use
- Acceptable use policy
- May restrict what corporate data can and cannot be shared with authorized AI integrations

### Limitations

- Bias- garbage in, garbage out
- Hallucinations- wrong info generated without regard for facts
- Accuracy- trust, but verify

### Private vs. Public

- Private- for the sole use within the organization for business purposes
- Public- available for anyone to utilize
    - CHATGPT, Gemini, and Bard are examples
