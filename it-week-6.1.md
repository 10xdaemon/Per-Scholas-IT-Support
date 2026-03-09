# Week 6: 2026-03-02

# MODULE 17: Supporting Other OS

## 17.1 Linux Features

### Shells, Terminals, and Consoles

- Bootloader
- Shell and Terminal
    - Shell provides command line interface for user
    - Bash, zsh, ksh are popular shells
    - Terminal application connects to shell interpreter
        - stdin, stdout, stderr
- Desktop environment
    - GUI for user interaction
- Console switching
    - CTRL+ALT+Fx

### Command Interface

- Command
    - Command to be executed
- Options
    - Modification of the command
- Arguments
    - Values that operate the command
- Pipes
    - Redirection of one commands output as the input to second command
- String multiple commands
    - Use semicolon (;) to string commands together
- Case sensitivity
- Help options
- Text Editor
    - vi
    - vim 
    - nano

### Navigation Commands

- No drive letters in Linux
    - Everything is a directory or sub directory of the root of the file system
- pwd 
    - Present working directory
    - Your location currently within the file system
- cd 
    - Change directory
- ls 
    - List contents of directory
- cat 
    - Display the contents of a file

### Search Commands

- find to search for file by name, owner, size, etc.
- grep to search for strings within a file
    - -i option will ignore case sensitivity
- Metacharacters and escaping
    - * wildcard character
    - Backslash \
    - Single and double quotes ' ' or " "

### Filesystem Management

- mount
    - Logical connection of file system to the OS
- /etc/fstab
    - File system information file dictating file system mount points
- fsck (File system check)
    - Check and repair utility

### File Management Commands

- cp 
    - copy
- mv 
    - move
- rm
    - remove
- df 
    - disk space free statistics
- du 
    - disk space used statistics

### User Account Management

- su
    - switch user
- sudo
    - Run specified commands with elevated permissions
    - Account must be listed in /etc/sudoers file
- /etc/passwd
- /etc/shadow
- useradd, usermod, userdel
- groupadd, groupmod, groupdel


### File Permissions Commands

- Read, Write, Execute (rwx)
- Symbolic mode using rwx designations or - for denied permission
- Octal mode
    - Read (4), Write (2), Execute (1)
- chmod 
    - Change or modify permissions
- chown 
    - Change ownership of file/directory

![permsissions demo](/assets/permissions_demo.png)

## 17.2 PACKAGE AND NETWORK MANAGEMENT

### Package Management Commands

- apt Debian based distros
    - apt update
    - apt upgrade
    - apt install
- DNF(yum) Red Hat distros
    - dnf check-update
    - dnf update
    - dnf upgrade
    - dnf install or dnf remove
- Updates are retrieved from repositories (repos)

### Process Monitoring Commands

- ps
    - Display process table
- top 
    - Display all running processes in real time statuses
- systemd
    - Init system and service manager in Linux
- systemctl
    - Used with systemd to start, stop, enable, and disable services

![system processes](/assets/process_table.png)

### Network Management Commands

- ip
    - ip addr
- /etc/hosts
    - Host name to IP mapping locally; queried before DNS
- /etc/resolv.conf
    - DNS server information
- ping
    - Tests connectivity
- dig 
    - DNS query through CLI
- curl 
    - Transfer data from one system to another
- traceroute 
    - Network diagnostic tool

### Backup and Scheduling Commands

- cron job 
    - Task scheduler for Linux
- crontab 
    - List of scheduled jobs
- Syntax for scheduling jobs
    - mm hh dd MM 
    - weekday
    - command

## 17.3 macOS FEATURES

### Interface Features

- Menu bar 
    - Top of screen
- Dock
    - Bottom of screen with one click access to apps and files
- Spotlight Search searches content on system
    - COMMAND+SPACE
- Terminal
    - CLI for macOS
- Mission Control
    - Multiple desktop displays
    - F3 key to activate

### System Folders and Finder

- Everything stems from root of directory
    - /Applications all applications installed
    - /Library system-wide resources and settings
    - /System core system files and resources for operation
    - /Users user account data
    - /Users/Library hidden folder for each user's home directory
- Finder
    - File Explorer for macOS

### System Settings

- Settings, network options, and configurations
- Apple keyboard differences
    - COMMAND- CTRL on Windows
    - OPTION- ALT key
    - CONTROL
- Displays
    - Scaling and display settings
- Accessibility
    - Vision and sound

### Security and User Management

- System Settings > Users & Groups
- Apple ID
    - Appstore purchases
    - iCloud sync and data storage
- Privacy and Security
    - Analytics
    - Telemetry data
    - Permissions 
- Internet Accounts
    - Keychain
- File Vault
    - Disk encryption 

### iCloud and Continuity

- Cloud storage including Mail, Contacts, Calendar, Photos, Notes and Reminders
- FaceTime
    - Audio and video call service
- iMessage
    - Apple’s proprietary messaging service
- iCloud Drive 
    - Store and access files
- Continuity
    - Switch between devices seamlessly
- AirDrop 
    - File sharing service direct between two Apple devices

### App Installation and Management

- App Store
    - Applications and OS updates and new releases
    - Apple ID required
- System Settings > Security and Privacy to adjust settings
- .dmg
    - Disk image like Windows .iso files
- .pkg
    - Package files
- Uninstall
    - Drag app to Trash
- Ensure regular updates are enabled for Antivirus
- Corporate Restrictions
    - Managed in Business Manager portal

### OS and App Updates

- App Store 
    - Enable auto download of updates
- macOS updates 
    - System Settings > General > Software Update
- Rapid Security Response (RSR)
    - Security updates direct from Apple
    - Enable automatic install is best practice

### Network and Device Settings

- Status menu > Advanced
    - Configure IP, DNS, and Wi-Fi options
- Printers & Scanners 
    - Add and manage devices
- Disk Utility used to verify and repair disk or file system

### Time Machine Backup

- Utility that uses a separate physical drive or partition to backup a system
- Partition or drive must be formatted using APFS
- Auto deletes oldest backup when full

### Troubleshoot Crashes and Boot Issues

- Use Force Quit from Apple menu for unresponsive apps
- Recovery Menu
    - Hold COMMAND+R while powering up Mac until Apple icon appears
- If internet access is available, Recovery can download a fresh installation of the OS
