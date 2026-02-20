# Week 4: 2026-02-19

# Managing Support Procedures

## 11.1 DOCUMENTATION

**Core 1 is completed i.e. chapters 1-10**

### Standard Operating Procedure

- SOP {standard operating procedure}: How you should do your job
- Defined as step-by-step instructions for any task
- Use guidelines when there are many variables or complex decision-making processes involved

### Service Level Agreements

- Defines the metrics of service delivery
- Internal agreements between departments
- External agreements with third-party providers like an ISP or CSP
- Rule of Nines {In relation to uptime}
    - `5 nines`(99.999%) `5.26 mins` of downtime per year
    - `8 nines`(99.999999%) `315.58 milliseconds` downtime per year

### Incident and Ticketing Systems

- Used to manage requests, incidents, and problems
- Can be used to assign issues to technicians and track updates of the resolution process

![ticket_demo](/assets/ticketdemo.png)

 ### Categories and Severity

- Categories unique to each organization
    - Requests: Provision assets like new accounts or systems
    - Incidents: Errors or unexpected conditions 
    - Problems: Incidents that require reconfiguring the system or network
- Prioritize issues by severity
    - Critical
    - Major
    - Minor

### Ticket Management

- Ticket: Communicates updates to technicians and clients/customers
- Escalation 
    - An issue is beyond the scope of the technician/agent
    - Internal escalation to another technician or department
    - External escalation to third-party provider or manufacturer support 
    - Tier 0- self service
    - Tier 1- initial agent for diagnosis
    - Tier 2- senior technicians
    - Tier 3- engineering team or senior management

### Support Documentation and Knowledge Base Articles

- Documents relevant information for the issue or incident resolution
- Provides information for future issues
- Provides technicians with initial diagnosis checks 
- Provides troubleshooting steps that worked in the past

### Lessons Learned

- After-action reports
- In-depth analysis of an issue or incident that drives changes to policy or procedures
- Can evolve into new SOPs
*Always have a record of what you're doing as to have a cover for yourself*

### Clear Written Communication
`be aware of who you're writing it for`
- Include issue description
- Include progress notes
- Include problem resolution
- Keep notes clear and concise

### Knowledge Base

- A self-serve central repository for information related to service issues
- Can include checklists for troubleshooting
- OEM or application developers may provide information

### Policy Documentation

- Acceptable Use Policy (AUP)
    - A list of acceptable behaviors and practices while utilizing corporate networks and systems
- Splash screen reminders to reinforce compliance

## 11.2 PROFESSIONAL COMMUNICATION

### Professional Support Process

- Document service hours and procedures to open a ticket
- Set and meet expectations and timelines
- Consider repair and replacement options
- Follow up to ensure solution works

### Professional Support Delivery

- Arrive on time
- Avoid distractions: Personal phone calls, text messages, or social media
- Handle confidential and private material appropriately: Do not access material or data on a system without permission

### Professional Appearance

- Professional appearance and attire
- Use proper language: Avoid jargon
- Use cultural sensitivity: Customs and habits of cultures vary

### Professional Communications

- Active listening
    - Maintain eye contact
    - Avoid interrupting
    - Repeat back your understanding

### Clarifying and Question Techniques

- Open-ended questions draw out further information: Start with these questions
- Closed-ended questions result in simple answers like yes or no: Use these to confirm the suspected issue

### Difficult Situations

- Maintain a positive attitude
- Avoid
    1. Arguing with the customer
    1. Denying or dismissing the problem
    1. Being judgmental

### Dealing with Difficult Customers

- Identify when a customer is getting angry
- Do not take complaints personally
- Actively listen to complaints
- Hang up if a customer becomes abusive or threatening
- Seek assistance from a supervisor or other technicians

### Do Not Post Experiences on Social Media

- Venting in public opens the door for scrutiny
- Follow company policy when discussing issues and cases


## 11.3 TYPES OF OPERATING SYSTEMS

### Windows and macOS

- Windows
    - Windows 10 and 11
    - Server 2019, 2022, and 2025 are optimized for enterprise environment management
- macOS offers a desktop OS exclusive to Apple hardware

### UNIX, Linux, and Chrome OS

- Unix features a shell and kernel architecture
    1. The shell provides user interactions
    1. The kernel manages system resources
- Linux is derived from UNIX for open-source licensing
    1. Includes a shell, desktop environment, and app packages
    1. Standard release vs. rolling release
- Chrome OS was developed by Google and based on Linux
    - For web applications

### iOS and Android

- iOS is built to run only on Apple iPhone hardware
- iPad, iWatch, tvOS
- Android OS
    1. open-source 
    1. OS built to run on multiple hardware platforms

### Windows File System Types

- New Technology File System `NTFS` 
    - Developed by Microsoft
    - Parts
        1. Journaling
        1. Snapshots
        1. Security
        1. Indexing
        1. Dynamic disk support
- ReFS
    - Microsoft developed for large storage and data integrity solutions
    - A high-performing, scalable, and resilient file system
- FAT32/exFAT
    - File allocation table (FAT) and extended FAT (exFAT)

### Linux and macOS File System Types

- Linux
    1. ext4 
    1. XFS extended file system
- macOS: APFS proprietary Apple File System

### OS Compatibility Issues

- OS developed for a particular set of device hardware 
    - Example: Windows 11 requires the support of a TPM v2.0
- Software applications 
    - Developed for a specific OS and file system
- Network compatibility
- Provide user training and support with changes

### Vender Life-cycle Limitations

- End-of-life/end-of-service-life
    OEM or developer no longer supports product

![compatability demo](/assets/compatdemo.png)

