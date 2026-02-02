# Week 1.5: 2026-01-30
## Troubleshooting PC Hardware

## 4.1 BIOS AND UEFI
- Basic input output system
- Unified extensible firmware interface
- Boot process interrupt

### Boot and Device Options
- Boot parameters:
    1. Fixed disk
    2. Optical drive
    3. USB
    4. Network/PXE (Pre-boot execution environment `pixi boot`)

### USB Permissions
- Enable and disable:
    1. USB controllers
    2. Adapters
    3. Ports (Individual/All)
    *CMOS and RTC are the same thing*

### Fan Considerations
- Optimized performance
- Balance power and speed
- Temperature monitoring (`80C Ideal Temp`)
    1. Manual
    2. Third-party application

### Boot Passwords and Secure Boot
- Supervisor/Admin/BIOS password: Restrict access to make changes in BIOS/UEFI menu (flash resets to factory settings)
- User system password: Locks system
- Secure boot: Digital signature

### Trusted Platform Modules `TPM`
- Securely store
    1. Digital certificates such as those for secure boot
    2. Cryptographic keys
    3. Hashed passwords
- Hardware Security Module (HSM)
    1. USB drive to store keys

## 4.2 POWER AND DISK ISSUES
### Troubleshoot Power Issues
- Follow power flow
    1. Outlet to power cable
    2. Power cable to power supply
    3. Power supply to motherboard
- Verify each component individually
    1. Power supply tester

### Troubleshoot POST Issues `power on self test`
1. Verify any changes
2. Check cables and connections
3. Faulty interfaces
4. Verify PSU
5. Faulty CPU or firmware issues
6. Beep codes (*no beep codes*- power issue)

### Troubleshoot Boot Issues
- Power
- Data connections
- UEFI/BIOS settings
- M.2/NVMe drive faults

### Troubleshoot Boot Sector Issues
- MBR(master boot record)/GPT errors
- Display connections
- Boot error
    1. Verify beep codes
- Malware issues
- Repair options
*BIOS->MBR || UEFI->GPT*

### Troubleshoot OS Errors and Crash Screens
- Blue screen of death - BSOD
    1. Device drive issues
    2. Corrupt system files
    3. Defective hardware
    4. Overheating or PSU issues

### Troubleshoot Drive Availability
- Unusual noise
- LED status/activity lights
- Boot device not found
- Missing drive in OS
- Read/write failure
- Audible alarms
- BSOD

###  Troubleshoot Drive Reliability and Performance
- S.M.A.R.T. drive tests
- Input/Output Operations Per Second (IOPS)
- Bad sectors

###  Troubleshoot RAID Failure
- Device failure
- Array failure
- Controller alerts

## 4.3 SYSTEM AND DISPLAY ISSUES
### Troubleshoot Component Issues
- Diagnostic steps
    1. Eliminate software issues
    2. Identify patterns
    3. Check power supply
    4. Suspect hardware
    5. Observe physical symptoms

### Overheating
- Temperature sensors
- CPU and case fans
- Heat sink
- Blanking plates
- Environmental issues: Dust and ambient heat

### Physical Damage
-  ESD, power spikes
-  Overheating
-  Careless insertion of connectors
-  Dirt
-  Liquid spills
-  Scorch marks
-  Swollen capacitors

### Troubleshoot Performance Issues
- Overheating
- Misconfigurations
- Verify the problem
- Rule out software and networking issues

### Troubleshoot Inaccurate System Date/Time
- Real-Time Clock (RTC) or CMOS battery (legacy)
    1. Provides power to maintain settings and configuration
- CR2032 battery

### Troubleshoot Missing Video Issues
- Physical cable issues
- Burnt-out bulbs
- Projector shutdown:
    1. Overheating
    2. Blown bulb
- Dim/fuzzy images
- Flashing screen
- Dead pixels (rainbow dots)
- Burn-in
- Incorrect color (cabling issue)

