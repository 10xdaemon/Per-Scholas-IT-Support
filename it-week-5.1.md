# Week 5: 2026-02-23

# MODULE 13: MANAGING WINDOWS

## 13.1 USE MANAGEMENT CONSOLES

### Device Manager

- Updating devices
- Driver information
- Troubleshooting malfunctioning devices
- Built-in troubleshooter to assist in diagnosis and correction of issues
- Removing devices
- Uninstalling devices
- Disabling devices
- Some hardware devices can be disabled in the BIOS/UEFI menus
- 
**work on missing**
########################################

### Disk Management Console

### Disk Maintenance Tools

- Disk DeFragmenter
    - HDD: Reorganizes data into contiguous clusters to improve access timelines
    - SSD: Performs a trim operation to reduce cell degradation `
- Disk Clean-up
    - Removes temporary files and files marked for deletion
    - Can remove old Windows installation files and updates no longer needed by the OS

![disk optimization demo](/assets/diskopt_demo.png)

### Task Scheduler

- Automates operations run at specific intervals or based on a trigger
- Logging: Allows troubleshooting when task failure
- Schedules tasks 
    - Updates, backups, and synchronizing data

### Local Users and Groups Console

- Advanced interface for managing user accounts on the local system
- Create and modify security groups for easier permissions management

### Certificate Manager

`logs all certs in one place and to view expiration date`
- Manage digital certificates for identify of users, computers, or services
- Facilitates verification of certificate information
- `Certmgr.msc` (current user) or certlm.msc (computer certificates)

### Group Policy Editor

- Manage local policies for users and computers
- Configure Windows settings without direct registry changes
- Apply settings efficiently system-wide 

### Registry Editor
*central database where all the keys for files are stored*
- Five root keys
![registry demo](/assets/registry_demo.png)
- Edit settings and configurations of user accounts, hardware, applications, and operating system
![registry key edit](/assets/registry_key_edit.png)

### Custom Microsoft Management Consoles `MMC`  

- Container for various snap-ins
- Place all necessary snap-ins needed for job in one location

## 13.2 COMMAND-LINE TOOLS

### Command Prompt

- "Run As Administrator" option for elevated permissions
- Syntax
    -  order of command, switches, and arguments
- CTRL+C
    - stop command execution
- Help
    - command /? Or help command 

### Navigation Commands

- Dir
    - /o: (n, s, e, d)
    - /t: (c, a, w)
    - /a: (r, h, s, a)
- Cd
    - .. {go back a directory}
    - \  {go forward}
- Change drive
    - Type drive letter then : (D: or E:)

### File Management Commands

- move
- copy
- robocopy: `robust copy`
    - Recommended for long filenames and NTFS attribute handling
- md or mkdir - make directory
- rd or rmdir - remove directory

### Disk Management Commands

- Diskpart
    - command line Disk Management tool
        1. select disk x
        1. detail disk
        1. select partition x
            - assign, delete, extend
        1. exit
- format 
    - Erases and reformats the drive 
- chkdsk
    - Scans file system and sectors for faults and attempts to repair

### System Management Commnands

- shutdown
    1. /s shutdown
    1. /h hibernate
    1. /l log off
    1. /r restart
    1. /t assign a delay to the shutdown command execution
        - Example: shutdown /r /t 45 will restart the system after 45 seconds
- sfc
    - System file checker to fix corrupt or damaged system files
- winver 
    - Displays Windows version information
- whoami
    - Displays current user who is logged in
