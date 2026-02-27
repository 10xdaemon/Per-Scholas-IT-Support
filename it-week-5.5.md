# Week 5 : 2026-02-27

# MODULE 16 INSTALLING OPERATING SYSTEMS

## 16.1 WINDOWS EDITIONS

### Windows Versions

- 32-bit vs 64-bit: Windows 11 only in 64-bit edition
- Home, Pro, Pro for Workstations, Enterprise, Education
- N versions compliant with EU regulations

### Windows Home Edition

- Designed for SOHO use
- Internet connection required for Microsoft account login and activation
- Licensing
    - OEM
    - Retail
- Limitations
    - 64 cores
    - Single CPU
    - 128 GB RAM (64-bit)

### Work and Education Features

- Pro, Enterprise, and Education editions
- Domain support
- Group Policy Editor
- BitLocker
    - Disk encryption for hard drives and USB (not in Home edition)
- RDP
    - Client and server (Home only has RDP Client)

### Windows Pro and Enterprise Editions

- Pro
    - OEM, retail, volume licensing
    - Pro for Workstations is same as Pro but support for larger memory and advanced hardware
- Enterprise and Education
    - Volume licensing only
    - DirectAccess VPN, AppLocker, MS Desktop Optimization Pack
- 128 core max (Pro and Education)
- 256 core max (Pro for Workstations and Enterprise)
- 2TB RAM (Pro and Education)
- 6TB RAM (Pro for Workstations and Enterprise)

### Windows Upgrade Paths and Feature Updates

- From Windows 10 to 11
    - TPM 2.0, UEFI with Secure Boot, supported processor
    - Upgrade with same edition or from Home to Pro 
    - Need license to update from Home to Enterprise 
    - Downgrade from Pro to Home
- Win 10
    - Semi-annual feature updates
    - Microsoft support ends Oct 2025
- Win 11
    - Annual feature update cycle

## 16.2 OS INSTALLATIONS AND UPGRADES

### Installation and Upgrade Considerations

- Clean install `last resort`
    - Repartition and reformat drive then install
- In-place upgrade
    - Updates existing OS install with new OS
    - User data remains on system
- Considerations
    - Hardware compatibility
    - Application and driver support
    - Backup files and user preferences
    - Third-party drivers
- Feature updates

### Unattended Installations

- Image deployment with answer file `installation file`
- Network-pushed installation
    - Zero-touch install 
        - Remote install using cloud-based service to deploy the image onto hardware

![Answer File](/assets/answer_file.png)

### Boot Devices

- Configured in BIOS/UEFI config
- Optical media
- USB, external drive, flash drive, hot-swappable drive
- Network boot
    - PXE boot (pronounced "pixie")
    - DHCP server required
- Internet-based boot
- Internal drive
- Multiboot
    - Multiple OSs installed on their own partition
    - OS selection menu shows up during boot

### Disk Configuration

- MBR-style partition
    - Master boot record takes first 512-byte to store the partition table
- GPT-Style partition
    - GUID partition table
    - Larger number of partitions (128 in Windows) and larger partition size (over 2TB)
- Drive Format
    - NTFS for Windows
    - APFS for macOS
    - ext3/4 for Linux

### Repair Installation

- Recovery partition
    - OEM created on drive
- Reset Windows
    - Refresh reinstalls system files and resets most settings to default
    - Reset erases all user data and resets the system for fresh installation
