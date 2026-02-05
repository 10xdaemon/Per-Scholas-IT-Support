# Week 2.3: 2026-02-05

# Comparing local networking hardware

## 5.1 NETWORK TYPES

### Local Area Network (LAN)
- Local Area Network (LAN): Single geographic location
- Wide Area Network (WAN): Large geographic location
- Wireless Local Area Network (WLAN): IEEE 802.11
- Metropolitan Area Network (MAN)
- Personal Area Network (PAN)
- Storage Area Network (SAN)

### SOHO and Enterprise Networks
- Small Office/Home Office (SOHO): LAN with single network appliance for connectivity

![soho networks](/assets/soho_nets.png)

- Enterprise: LAN with separate devices for network connectivity

![enterprise networks](/assets/enterprise_nets.png)

### Datacenters
- Site housing server resources
- Dedicated network, power, climate-controlled, with secure access controls to protect the environment 

## 5.2 NETWORKING HARDWARE

### Network Interface Cards

- Ethernet, fiber, and wireless
- MAC address = hardware address `Media Access Control`
    - 48-Bit, hexadecimal digits
        1. 24-bit OUI
        1. 24-BIT NIC specific

- Wireshark Demo

![wireshark demo](/assets/shark_demo.png)

### Patch Panel

![patchpanel](/assets/patchpanel.png)

- Connection point from wall jacks (Keystone Jacks) to switch
- Punch down tool used for rear connections

### Switches 

- Connection between end point nodes
- CAM table
- Collision domain(switch) vs. broadcast domain(router)

![switch diagram](/assets/switch_diagram.png)

### Unmanaged and Managed Switchs

- Unmanaged- plug and play
- Managed- management Interface for configuration

**Modular unit allows customized configuration**

![managed demo](/assets/managed_demo.png)

### Power over Ethernet

- IEEE standards
    1. 802.3af PoE or Type 1
    1. 802.3at PoE+ or Type 2
    1. 802.3bt PoE++ or Type 3 and Type 4
- PoE-enabled switch
- PoE injector (port specific)

## 5.3 NETWORK CABLE TYPES

### Unshielded Twisted Pair

 - Copper conductor
 - 100m (328')
 - Twisted to reduce attenuation(increases bandwidth)

### Shielded Twisted Pair

*In areas with high EMI(electromagnetic interferance)*
- Copper conductor
- Each pair has foil shielding
- May contain braided screen
- EMI protection

### CAT Standards

![cat standards](/assets/cat_table.png)

### Copper Cabling Connectors

- Registered jack
- RJ-45 (network)
- RJ-11 (POTS - plain old telephone service)

### Copper Cabling Installation Tools

- Cable/wire stripper: Used to trim back outer jacket
- Snips/cutter: Used to trim wire and cable to correct length
- Punchdown tool: Connect individual wires to an IDC or keystone jack
- Crimper: Attach RJ-11 or RJ-45 plug

### Copper Cabling Test Tools

- Cable tester: LED indicator testing connection on individual pairs of wire
- Toner probe: Used to trace and locate cables in network closet or cable bundles
- Loopback plug: Used to test transmit and receive wire pathways

### Network Taps

- Passive: Monitors traffic without interruption of dataflow by creating a copy of the data
- Active: Monitors traffic directly and then regenerates the traffic signal to continue it along its pathway to its destination

### Copper Cabling Installation Considerations

- Plenum rated
- Direct burial

### Optical Cabling

- Higher bandwidth
- Longer distance signaling
- Single mode vs. multimode fiber 
- Connectors
    1. ST (straight tip)
    1. SC (subscriber connector)
    1. LC (lucid connector)

### Coaxial Cabling

- Radio Grade (RG)
- Connector: F-type

![coax diagram](/assets/coax.png)

## 5.4 WIRELESS NETWORKING TYPES

### Access Points (AP)

- IEEE 802.11 standards
- BSSID- MAC of AP

### Frequency Bands

- 2.4 GHz (~far)
- 5 GHz (~close)
- 6 GHz

### IEEE 802.11a

- 5 GHz frequency
- 54 Mbps
- DFS

### IEEE 802.11b/g

- 2.4 GHz frequency band
- Modulation- DSSS and OFDM
- 11/54 Mbps

![2.4GHz chart](/assets/2.4_charts.png)



- 2.4/5 GHz dual band
- Channel bonding
- MIMO (multiple input/ multiple output ie.multi-user)
- 600 Mbps
- Wi-Fi 4

### Wi-Fi 5 and Wi-Fi 6

- 802.11ac- 5GHz only
    1. MU-MIMO
    1. Dual and triple band- backward compatibility with 2.4GHz systems
    1. 2.1+ Gbps 
- 802.11ax- 2.4/5/6GHz(6e)
    1. OFDMA modulation
    1. MU-MIMO
    1. 1.1 Gbps 2.4GHz; 4.8 Gbps 5GHz

### Wi-Fi 7 (802.11be)

- 2.4/5/6 GHz
- 46 Gbps

### Wireless LAN Installation Considerations

- SSID
- Frequency band
- Channels

**Router Setup Demo**

![router setup demo](/assets/router_demo.png)

### Wi-Fi Analyzers

- Signal strength
- Interference

![analyzer demo](/assets/analyzer_demo.png)

### Long-Range Fixed Wireless

- Licensed(cell towers) vs. unlicensed(cable dish)
- High-powered antenna

### Bluetooth, RFID, and NFC


- Bluetooth pairing
- RFID- inventory tracking and badge access
- NFC- contactless payment and badge access use