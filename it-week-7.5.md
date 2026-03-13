# Week 7: 2026-03-13

# MODULE 22: Implementing Operational Procedures

## 22.1 Change and Inventory Management

### Change Requests

- Policies and procedures that reduce risk of outages caused by changes
- Should include: Purpose, scope, type, timeline, effect

### Risks Analysis

- Identify possible issues with implementation
- What controls or monitors can be implemented to reduce the risk
- Identify cause and effect
- Qualitative and quantitative analysis

### Change Board Approvals

- Change advisory board (CAB)
    - Officially approves changes after request is thoroughly reviewed
- Some changes may not need full approval of board, especially during incident response or emergency procedures

### Implementation and Acceptance

- Implement change
- Rollback and/or backup plan
- End-user acceptance

### Asset Management

- Inventory
    - Name, make, model
    - Asset ID: Tag or barcodes are popular
    - Manufacturer
    - Specifications
    - Dates: Warranty, purchase, etc.
    - Cost
- Configuration management database (CMDB)
- Lifecycle
    - Procurement through disposal/destruction

![asset tag](/assets/asset_tag.png)

### Warranty and Licensing

- Invoice documentation
- Warranty timelines and paperwork
- Document limits and license allocations/use

## 22.2 Common Saftey and Environmental Procedures

### Compliance with Regulations

- Health and safety
- Building codes
    - Fire and electrical system protection
- Environmental regulations
    - Waste disposal like chemicals and lithium batteries

### Electrical Saftey

- Current- amps
- Voltage- volts
- Resistance- ohms
- Tools
    - Voltage testers
    - Fuses
    - Grounding
- Power handling
- Electrical fire safety- CO2 or powder extinguishers vice water
- Equipment placement considerations

### Other Safery Hazard Mitigations

- Trip hazards
- Lifting techniques
    - Legs not back
    - Use multiple people when needed
- Safety goggles and mask

### Environmental Impacts

- Dust cleanup
    - Mask, vacuum, compressed air
- Temperature
- Humidity
- Ventilation

### Electrostatic Discharge Mitigation

- ESD can damage components
- ESD strap, mat, workbench
- Antistatic bag or dissipative packaging for component storage

![discharge demo](/assets/discharge_mitigation.png)

### Building Power Issues and Mitigations

- Surge, under-voltage, failure
- Surge suppressors
- Battery backups or uninterruptable power supply (UPS)
    - Not meant for long term secondary power
- Generator
    - Gas, Diesel, Propane, Natural gas

### Materials Handling and Responsible Disposal

- Material safety data sheet (MSDS)
    - Hazards and cleanup/safety requirements
- Proper disposal
    - Battery
    - Toner
    - Chemicals
    - Devices and assets

## 22.3 Scripting Basics

### Shell Scripts

- Specific to an OS
- Script
    - Series of commands that are executed in order
- Integrated development environment (IDE)
- Linux shell .sh
    - Bash (Bourne Again Shell)
    - Ksh (Korn Shell)

### Basic Script Constructs

- Comments
    - Not read by compiler or interpreter
- Variables
- Branches
- Loops
- Operators

![script commands](/assets/script_commands.png)


### Windows Scripts

- PowerShell .ps1
- VBScript .vbs
- Batch file .bat

![windows ise](/assets/windows_ise.png)

### JavaScript and Python

- JavaScript .js
    - Web content and apps
- Python .py
    - General purpose primarily used in automation and software apps
    - Python IDLE

### Use Cases for Scripting

- API use
- Restarting machines
- Remapping network drives
- Installation of applications
- Updating system OS and apps
- Automated backups
- Information gathering
    - Inventory

### Scripting Best Practices and Considerations

- Malware risk
- Inadvertent system/settings changes
- Browser or system crash due to resource mishandling

