# Week 3: 2026-02-13

# Module 10 Supporting Printing Devices

## 10.1 PRINTERS AND MULTIFUNCTION DEVICES

### Printer Unboxing and Setup Location

- Select a printer: Consider speed, resolution, paper handling, options
- Setup location: Consider power, network, environmental concerns, accessibility
- Unboxing a printer
    - Lifting heavier units may require two people
    - Packing materials
    - Acclimation to humidity and temperature [*sensitive to temperature change*]

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
- Paper tray selection i.e., A4 `8'x 11'(letter)`, `8'x 14'(legal)`
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

## 10.2 PRINT DEVICE MAINTENANCE

### Laser Printer Imaging Process

1. `Step 1 Processing`
    - Document is encoded and sent to printer to be converted to bitmap
2. `Step 2 Charging`
    - Charge roller applies negative charge to imaging drum
3. `Step 3 Exposing`
    - Laser shines on imaging drum, removing the negative charge
4. `Step 4 Developing`
    - Toner sticks to neutralized areas on imaging drum
5. `Step 5 Transferring`
    - Toner is transferred to paper
6. `Step 6 Fusing`
    - Heat is applied to fuse toner to paper
7. `Step 7 Cleaning`
    - Imaging drum is cleaned of residual toner

![laser process](/assets/laser_process.png)

### Laser Printer Maintenance

- Load paper when empty
- Replace toner cartridge
    - Ensure packing is removed before installation
- Clean printer
    - Never use compressed air
    - Use damp cloth to wipe exterior
- Maintenance Kit
    - Fuser/imaging unit
    - Rollers
- Calibration

### Inkjet Printer Imaging Process

- Thermal printers: Heat ink to form a bubble that bursts, spraying ink
- Piezoelectric printers: Use jet nozzle to spray ink
- Carriage system: Holds print head and sometimes ink cartridges

![inkjet image processing](/assets/inkjet-img.png)

### Inkjet Printer Maintenance

- Replace rollers regularly
- Ensure paper is installed correctly
- Replace inkjet cartridges
- Printers with ink tanks are refilled with liquid ink
- Calibrate print head alignment
- Clean print head
- Fix paper jams

### Thermal Printer Maintaenance

- Wax-coated paper heats to transfer image
- Commonly for receipts, shipping labels, and barcode labels
- Tearing creates dust so clean regularly

![thermal schema](/assets/thermal_schema.png)

### Impact Printer Maintenance

*Functions similar to a typewriter*

- A dot matrix is a series of dots used to form characters
- Multipart paper is carbon/carbonless paper with white, yellow, and pink layers
- Create multiple copies in one pass
- Tractor-fed paper has holes on side to aid feeding

### 3D Printer

- Spool :Has the filament used by the printer
- For some prints, print in batches for stability reasons and accurate models
- Filament types: Resin, etc...
- Uses CAD/Blender

## 10.3 TROUBLESHOOT PRINT DEVICES

### Printer Connectivity Issues

- Check if printer is powered on and online
- Verify consumables (ink, paper) are loaded
- Print a test page
- Inspect cables or wireless settings
- Check for needed firmware and driver updates
- For cloud printers, verify registration with cloud service 

### Print Feed Issues

- For paper jams: Follow on-screen instructions to clear paper path
- Verify paper settings and feed roller condition
- Grinding noises: Ensure cartridges and print head are seated correctly

### Print Quality Issues


- Faded or faint: Verify print resolution and/or replace toner cartridge
- Black stripes: Check charge roller or high-voltage power supply 
- Vertical or horizontal lines: Clean rollers
- Smudged toner: Replace fuser
- A color is missing: Replace cartridge and clean contacts
- Print test pages to verify the results

*The distance from the nozzle to the page is called the plating gap*
- too close hit the paper hard
- too far away, shotgun spray

### Finishing Issues

- Check for incorrect page orientation
- Hole punch errors: Verify max number of pages allowed
- Staple errors 
    1. Check for a stapler jam
    1. Check for staples empty

### Print Job Issues

- Print monitor provides printing status updates
- Clear old or obsolete jobs from print queue and spooler
- Tray not recognized error: Verify tray is fully inserted
- Frozen print queue/spooler: Stop and restart print spooler and clear cache 
- Garbled print job **(printing out gibberish i.e., `aldkgasldkgjasdg`)**
    - Verify correct PDL is selected
    - Print test page: If test page is good, it may be an application-specific issue
