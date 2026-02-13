# Week 3: 2026-02-13

# Module 10 Supportting Printing Devices

## 10.1 PRINTERS AND MULTIFUNCTION DEVICES

### Printer Unboxing and Setup Location

- Select a printer: Consider speed, resolution, paper handling, options
- Setup location: Consider power, network, environmental concerns, accessibility
- Unboxing a printer
    - Lifting heavier units may require two people
    - Packing materials
    - Acclimation to humidity and temperature [sensitive to temperature change]

### Firmware Management in MDFs and Printers
`Multi-Function Device`

- Even new printers may require firmware updates
- Reset and reflash firmware to avoid malfunctions
*{Some printers may require reflashing. When reflashing, ensure that stable power is provided. If the reflash sequence is interrupted, it could lead to a non-functioning device.}*
- Backup configurations and settings before resetting or reflashing

### Print Device Connectivity

- USB is directly connected to a computer 
- Ethernet is connected to network with its own IP address
- Wireless is connected to Wi-Fi network or to computer via Bluetooth `uses wi-fi direct`

![print gui](/assets/printgui.png)

### Printer Drivers and Page Description Languages

- Driver Selection
    - Plug and play {`streamlines the process`}
    - Manual installation for page descriptive language (PDL)
        - XPS, PCL, and PostScript
- PDL supports
-   Scalable fonts
-   Vector [**uses a math eqn to determine each letter/pixel**] graphics
-   Color printing: CMYK- Cyan, Magenta, Yellow, Black

### Printer Properties

- Print queue
- Paper tray selection i.e., A4 `8'x11'(letter)`, `8'x14'(legal)`
- Fonts
- Driver

### Printing Preferences
**finishing touches**

- Print quality 
    - DPI (dots per inch)
    - economy/draft mode
- Paper type and size
- Finishing
    - Duplex: {printing on both sides i.e. `duplexer`}
    - Multiple pages per sheet
    - Landscape vs. portrait

### Printer Sharing

- Public printers have no access controls
- Print server are connected to server/computer then shared to network
- Shared printer connections

### Printer Security

- User authentication
- Pin entry or badge swipe can release print jobs
- Audit logs track details of each print job

### Scanner configuration

- Optical Character Recognition (OCR) identifies characters to recreate document
- Flatbeds use moving head across document
- Automatic Document Feeder (ADF) uses fixed scan head `paper jam zone`
- Network scanning services 
    - Email
    - Server Message Block (SMB)
    - Cloud
![mtf schema](/assets/mtfschema.png)

