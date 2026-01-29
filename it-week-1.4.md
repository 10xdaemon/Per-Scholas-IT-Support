# Week 1.4: 2026-01-29
## 3.1 POWER SUPPLIES AND COOLING
### Power Supply Units
- converts AC to DC
- outlet voltage compatibility (`selector switch` or `auto`)
- 3.3V, 5V, 12V
- 110V - 120V AC in the US
- 220V - 240V rest of the world
- Biggest leakage these days are graphics cards (300+ W)

### Power Supply Connectors
- Transfer power to system components
- P1/24-pin: Powers the motherboard
- Molex: Hard drives (PATA) `legacy`
- SATA
- 4/6/8/16-pin connectors

### 20-pin to 24-pin Motherboard Adapter
- 20-pin legacy
- 24 or 20+4 pin

### Modular Power Supplies
- Detachable cables
    1. Customizable connectors/cable needs
    2. Reduce clutter in chassis: space efficient and energy

### Redundant Power Supplies
- Failover protection
- Commonly seen in servers and datacenter configurations
- Hot swappable vs. cold swappable
- Fault tolerance

### Heat Sinks and Thermal Paste
- Passive cooling
- Transfer heat better due to surface area
- Bridges microscopic gaps between metal CPU and heat sink block

### Liquid Cooling Systems
- Water loop tubing
- Pump
- Water block
- Radiator
- Fan
- Cooling liquid

## 3.2 STORAGE DEVICES
### Mass Storage Devices
- Data is stored in a partition/volume
- Motherboard drive bays
- Removable and externally attached
- Evaluate choice based on:
    1. Reliability
    2. Performance
    3. Use

### Solid-State Drives
- No moving components
- Non-magnetic
- High performance: ==Read('viewing')/write(modifying data) speeds==
- Higher cost
- Connection methods
    1. SATA
    2. PCIe- M.2, NVMHCI, or NVMe
    3. SAS: Serial Attached `SCSI`(legacy server hardrive connectors)

### `RAID`: Redundant Array of Independent Disks
- *All hardrives should have the same amount of storage*
- Data distribution across multiple physical drives
- Redundancy and capacity
- RAID levels

### RAID 0 and RAID 1
- `RAID 0`- striping without parity (split between hard drives)
- 2 physical drive minimum
- Better performance than regular hard drive use
- No redundancy
*total space: Amount of hardrives / 2*

- `RAID 1`- mirroring
- 2 physical drive minimum
- Redundancy
*total space: Amount of hardrives / 2*

**NOTE: think about things on the enterprise level**

### RAID 5 and RAID 10
- RAID 5- striping with single parity
- 3 physical drive minimum
- Slower write operation - fast read operation
*total space: storage total - 1(storage)*

- RAID 10- strip of mirrors
- 4 physical drive minimum: Must be an even number of drives
*total space: Amount of hardrives / 2*

### Removable Storage Drives
- Drive enclosures
- External- USB, Thunderbolt, eSATA
- Network attached storage

**NOTE: A server is a primary function is to give a resource**

## 3.3 SYSTEM MEMORY
### System RAM and Virtual Memory
`RAM stores active dynamic data`
- Address space:
    - Data pathway
    - Address pathway

### RAM types
- DRAM: `dynamic`
- SDRAM: `synchronous dynamic`
- DDR SDRAM: `dual data rate`
- CAS latency: `clock-speed latency`

### Memory Modules
- DIMM: `dual inline memory module`
- SODIMM: `small outline %`
- Installation
- Incompatibility: DDR4 module will not fit DDR3 slot

### ECC RAM
- Error correction code
- Compatibility considerations
    1. Motherboard and CPU
    2. DIMM compatibility
    3. ECC and non-ECC mixing

## 3.4 CPUs
### CPU Architecture
*CPU PIPELINE*
1. Fetch
2. Decode
3. Execute
4. Write-back(to save data)

### x86 CPU Architecture
- `32-bit` instruction set
- Manufacturers
    1. Intel
    2. AMD
- ALU- Arithmetic Logic Unit
- Cache memory- L1, L2, L3

### ARM CPU Architecture
- consider mobile platforms

### CPU features `x64 only`
- Multithreading
- Symmetric multiprocessing
- Multicore CPUs
- Virtualization

### CPU Socket Types
- PGA vs LGA
    - AMD- PGA; pins on chip
        1. AM4
        2. TR4
        3. SP3
- Intel- LGA; pins on socket
    1. LGA 1200
    2. LGA 1700

### CPU Types and Motherboard Compatibility
- Motherboard socket must match CPU
    1. Core configuration
    2. Performance
- Desktops
- Workstations
- Servers
