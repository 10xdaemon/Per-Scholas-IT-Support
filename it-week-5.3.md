# Week 5: 2026-02-25

# LESSON 14 SUPPORTING WINDOWS

## 14.1 TROUBLESHOOT WINDOWS NETWORKING

### Troubleshoot IP Configuration

- Limited IP connectivity
    - Verify IP config
    - DHCP Settings and server availability (APIPA)
- No Internet access
    - IP configuration: IP/Subnet Mask/Gateway
    - DNS server configuration
- ipconfig command
    - /all, /release, /renew, /displaydns, and /flushdns
- hostname command

![ip config demo](/assets/ip_demo.png)

### Troubleshoot Local Network Connectivity

- Connectivity test
    - Ping command
    - Loopback IP, local workstation IP, then gateway IP, then remote system FQDN or IP
- Local loopback or local workstation IP unreachable
    - Troubleshoot network adapter configuration
- Gateway IP unreachable
    - DHCP server options configured correctly
    - Router IP configuration done correctly
- Remote system FQDN or IP unreachable
    - Verify resource exists
    - Verify DNS settings

### Troubleshoot Remote Network Connectivity

- tracert command `shows how many hops it takes to get to an ip`
    - RTT per hop
- pathping command
    - Can show latency and packet loss per hop

### Troubleshoot Name Resolution

- Connection via FQDN vs. connection with IP address directly
- nslookup command
    -type=<resourcerecordtype> where <resourcerecordtype> = A, AAAA, MX, NS, PTR, CNAME etc.

### Troubleshoot Network Ports

- netstat command (show you what connections you computer is using)
- -a include UDP connections
- -b show process that opened port
- -n numerical format
- -e report ethernet statistics
- -s report protocol statistics

![netstat view](/assets/netstat_demo.png)

## 14.2 REMOTE ACCESS TECHNOLOGIES

### Remote Desktop Tools

- Remote Desktop Protocol (RDP)
    - Remote Desktop Connection application (mstsc.exe)
    - TCP port 3389
    - Encrypted authentication and session
    - IP or FQDN of remote system needed
    - Credentials to log in
- Virtual Network Computing (VNC)
    - TCP port 5900
### `VNC` is open-source whereas `RDP` is **specifically** for windows 

### Microsoft Remote Assistance

- Initiated by invite only
- Includes chat feature and remote-control capability
- Ephemeral port use (49152-65535)
- Quick Assist 
    - Facilitates Remote Assistance without reconfiguring firewall using TCP port 443 (HTTPS)
- `similar to a Stream`

### WinRM

- Uses SOAP[Simple Object Access Protocol]-based communication
- Allows access and exchange of management information across network
- Interoperability between different hardware and software platforms using HTTP/HTTPS
- Can be easily used in PowerShell scripts

### Secure Shell

- TCP port 22
- Encrypted
- Password or key-based authentication methods

### Desktop Management and Remote Monitoring Tools

- Remote monitoring and management (RMM)
    - Primarily an MSP tool for remote support
- Desktop management and MDM
    - Management of device belonging to a single organization
- Endpoint Detection and Response (EDR) capability
    - Security tool for scans and reporting of issues with pre-programmed responses

### Simple Protocol for Independent Computing Environments (SPICE)

- Remote display to monitor and interact with a VM
- Authentication support for Kerberos and others
- TLS encryption of communication

### Other Remote Access Tools

- Screen sharing
    - TeamViewer or LogMeIn
- Video conferencing tools
    - Microsoft Teams or Zoom
    - Screen share capabilities
- File transfer software
    - AirDrop for Apple
    - Nearby Sharing for Microsoft
    - Nearby Share for Android
- VPN
    - Encrypted tunnel to connect to internal systems through the VPN gateway/server

## 14.3 PERFORMANCE AND TROUBLESHOOTING TOOLS

### System Information

- msinfo32.exe
- System resources
- Firmware version
- OS version
- Hardware
- Environment variables
- Network status

### Event Viewer

- Eventvwr.msc
- Windows Log viewing
    - Application
    - Security
    - Setup
    - System
    - Forwarded Events
- Severity Levels
    - Information, Warning, Error, Critical

### Task Manager Process Monitoring

- CTRL+SHIFT+ESC
- CTRL+ALT+DEL then select Task Manager
- Right-click Start button or the taskbar
- Processes
- Details
- Set Priority

### Task Manager Performance Monitoring

- App history
    - Windows Store apps
- Disk monitoring
- Network monitoring

### CPU and GPU Monitoring

- CPU
    - Cores and logical processors (HyperThreading)
    - Virtualization status
- GPU
    - Dedicated graphics adapter monitoring
    - Graphics memory monitor

### Memory Monitoring

- In use
- Committed
- Cached
- Paged pool/non-paged pool
- High utilization can be normal to maximize performance

### Resource Monitor and Performance Monitor

- Resource Monitor (resmon.exe)
    - Advanced monitoring of resources beyond Task Manager's capabilities
- Performance Monitor (perfmon.exe)
    - Real-time statistic charts and logs for long-term analysis
    - Counter logs
    - Trace logs

![resourse dashboard](/assets/resource_dashboard.png)

### Performance Counters

- Specific monitoring metrics to be used in Performance Monitor utility
- Examples
    - % processor time
    - Average disk queue length
    - Memory pages/sec
    - Paging file % usage

## 14.4 TROUBLESHOOT WINDOWS OS PROBLEMS

### Boot Process

- BIOS
    - POST
    - Boot loader- BOOTMGR.EXE
    - WINLOAD.EXE
        - Kernel
        - HAL.DLL
        - Drivers

- UEFI
    - POST
    - GPT read
    - BCD and BOOTMGFW.EFI
        - Kernel
        - HAL.DLL
        - Drivers

### Boot Recovery Tools

- Advanced Boot Options
    - Interrupt boot process
    - Hold shift while selecting restart from power menu in Windows
- Troubleshoot
- WinRE
- Start-up repair
- Advanced options

### System Restore

- Configure system protection
    - Restore point
    - Disk space usage
- Using system restore

### Update and Driver Roll Back

- Programs and Features applet > view installed updates > select update and then uninstall
- Device Manager > Properties > Driver > Roll Back Driver

### System Repair, Reinstall, and Reimage

- Recovery image
    - Backup of the system used to restore system config and files
- Reinstall Windows
    - Reset this PC option in WinRE
    - Keep data files or remove everything

### Troubleshoot Boot Issues

- Failure to boot
    - Verify no floppy disk is installed or USB is plugged in still and set to boot
- No OS Found
    - Use chkdsk and bootrec commands from the command prompt
    - diskpart could also be used to verify system partition is set to active
- GUI Fails to Load
    - Verify monitor turned on and connected to correct video port
    - Verify input selection
    - Boot to Safe Mode

### Troubleshoot Profile Issues

- Display highly detailed status messages
- Verify drivers and services set to load immediately after startup
- Rebuild the local profile, if necessary

### Troubleshoot Performance Issues

- Degraded Performance
    - Task Manager, PerfMon, and ResMon can be used to verify utilization
    - Reboot the system
    - Update OS, applications, and drivers as they may improve performance by fixing known issues
    - Scan for malware and verify antivirus/antimalware updates
    - Power management issues

### Troubleshoot System Fault Issues

- Blue Screen of Death (BSOD)
    - Research indicated problem from details on screen or using QR code
- System instability
- Frequent unplanned shutdowns
    - Overheating or corruption of system files
- USB Issues
    - Controller resource issues

### Troubleshoot Application and Service Fault Issues

- Application crashes
    - Update
    - If no change, uninstall and reinstall
- Services not starting
    - Verify service is set to automatically start, if necessary
- Time drift
    - Replace RTC battery (CR 2032)
    - Synchronize clock with known good source (NTP server)
