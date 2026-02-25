# Week 4: 2026-02-20

# 12. CONFIGURING WINDOWS

## 12.1 Windows User Settings

- Windows 10 Desktop
    - Start button is bottom left on taskbar
- Windows 11 Desktop
    - Start button is center on taskbar
- Taskbar search in both OS versions

### Account Settings

- Profile: The settings and configuration for a specific user
- Microsoft account vs. local account
- UAC settings: Prevent unauthorized use of administrative privileges

### Privacy Settings

- Data collection default opt-in option for Microsoft
- Optional for data sharing
    1. Contacts
    1. Calendar
    1. Email
    1. Files

### Desktop Settings

- Time
    - Date/time format and time zone
- Language
    - Spelling and localization, keyboard input, and speech recognition
- Personalization settings
    - Themes, wallpaper, screensaver, color scheme, and font
- Vision
    - Cursor indicators, high-contrast and color-filter modes, and magnifier
- Hearing
    - Volume, mixing, visual notifications, and closed-captioning
- Interaction
    - Keyboard and mouse options, speech and eye-controlled input

### File Explorer

- File management via GUI
- System objects
    - User account
    - OneDrive
    - This PC
    - Network
    - Recycle Bin
- Drives and folders
- System files: Windows, Program Files/Program Files (x86), and users

![file exp](/assets/fileexp.png)

### File Explorer Options
- General tab
    - Layout 
    - Single vs. double-click interactions
- View tab
    - Hide extensions 
    - Hide files and folders 
    - Hide protected OS files
    - Default folder 
    - Search options and behaviors

## 21.2 WINDOWS SYSTEM SETTINGS

### System Settings

- Input/output devices
- Power
- Remote desktop
- Notifications
- Clipboard
- About

### Update and Security Settings

- Update: Updates OS and associated Microsoft products (ex: Office) and hardware drivers
- Patch: Minor fix for issue in program or OS code
- Security: Includes Windows Defender antivirus, threat protection, and firewall
- Activation: Activates product with Microsoft for anti-piracy

### Device Settings

- System settings: Display and sound
- Bluetooth & devices: Input and output devices with Bluetooth or USB connectivity
- Mobile devices: Smartphone device management
- Devices and printers (Control Panel): Manually add devices

### Display and Sound Settings

- Scale: Changes size proportions for large screens
- Color: Changes monitor calibration for color matching
- Multiple displays: Set up multiple screens and/or projector configuration
- Resolution and refresh rate
    - Resolution: Pixel by pixel
    - Refresh rate
        1. Speed of entire display refresh 
        1. Expressed in Hz
- Sound
    - Output and input device selection
    - Level adjustment

### Power Options

- Standby/suspend: Removes power to most devices but maintains power to memory (RAM)
- Hibernate/suspend 
    - Removes power from all components 
    - Saves memory data to disk
- Power options: Change power button functionality
    1. Power saver 
    1. Balanced 
    1. High performance


### Apps, Programs, and Features

- Features 
    - Windows components of the OS that may be enabled/disabled
- Store apps 
    - Run in restricted sandbox to prevent system-wide changes
    - Do not require admin privileges
- Windows Subsystem for Linux (WSL)
    - Installation of Linux distribution without using a virtual machine

### Apps Settings

- Menu to view and uninstall applications and Windows features
- Configure default apps
- Auto-startup apps
- Programs and Features: Legacy interface
- Mail 
    - Manage mail accounts for Microsoft Outlook
- Gaming for game mode on/off
    - Suspends Windows updates and improves 3-D performance and frame rate for graphics

### Network Settings

- Network and Internet Settings: Network status, IP properties, and other tools
- Network Connections: Change IP properties of network adapters
- Use Network and Sharing Center: See status information
- Advanced sharing: Configure network discovery options and file/printer sharing
- Windows Defender Firewall
- Internet options: System-wide web browser settings

### Administrative Tools
`you can use the run command to access it **win + r**`
- Computer Management (compmgmt.msc)
- Defragment and Optimize Drives (dfrgui.exe)
- Disk Cleanup (cleanmgr.exe)
- Event Viewer (eventvwr.msc)
- Local Security Policy (secpol.msc)
- Resource Monitor (resmon.exe)
- Performance Monitoring (perfmon.msc)
- Registry Editor (regedit.exe)
- Services console (services.msc)
- Task Scheduler (taskschd.msc)

### Management Shortcuts

- Windows + X
- Right-click start button
- Instant search
- Run dialog box

## 12.3 INSTALL AND CONFIGURE APPLICATIONS

### System Requirements for Appications

- CPU: Clock speed, number of cores, architecture
- Memory: Speed and minimum requirements
- Storage: Minimum storage
- Graphics
- External hardware token: Smart card or USB for authentication

### OS Requirements for Applications

- OS compatibility
- 64-bit vs. 32-bit 

### Disturbitions Methods

- Physical media
    - CD/DVD
    - USB drive
- Download from the Internet
- Mount ISO file directly in Windows
- UAC confirmation of changes

### Other Considerations

- Business impacts: Licensing, support, training needs `needed for enterprise`
- Operation impacts: Deployment, updating, maintenance
- Device and network impacts `sending out service announcement is procedure`
    - Use of limited local system resources
    - Use of network resources and bandwidth

## 12.4 CLOUD-BASED APPLICATIONS

### Email Systems

- Outlook Web in Microsoft 365
- Gmail in Google Workspace

### Storage

- OneDrive, Google Drive, Apple iCloud
- Data storage and synchronization across multiple platforms

### Collaboration Tools

- Documents
    - Office 365 or GoogleDocs and Slides
    - Multiple users with simultaneous access and editing capability
    - Changes synchronize in near real-time with tracking
- Videoconferencing
    - Video, audio, and text-based chat features
    - Zoom, Slack, Teams

### User Licensing

- Licensing terms
    - Personal vs. commercial use
    - Multi-user access
- Enterprise management
    - Admin portal for issuing licenses to individual accounts

### Identity Synchronization

- Cloud identity account: Used across platforms and applications
- Single account: Used to access multiple applications
- Used for federated access or single sign-on configurations

![entra infrasturcutre](/assets/entrainfra.png)

