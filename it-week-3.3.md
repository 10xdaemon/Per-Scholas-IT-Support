# Week 3: 2026-02-11

# Summarizing Virtualization and Cloud Concepts

## 8.1 CLIENT-SIDE VIRTUALIZATION

### Hypervisors

- Type II or 2
    - Installed as an application on top of host OS
        1. Oracle VirtualBox
        2. Parallels Workstation


- Type I or 1 aka `bare-metal`
    - Installed directly on hardware
        1. Hyper-V
        2. VMWare ESXi

### Uses for Virtualization

- Client side: Sandboxing{*test environment*}, legacy OS hosting, cross-platform, training and labs
- Server side: Hosting of additional network nodes
- Desktop: VM desktop for employees to use rather than a traditional desktop system
    - FIM client
- Application
- Container

![container vs vm](/assets/containervm.png)

### Virtualization Resource Requirements

- CPU and virtualization extensions
    - CPU support of virtualization technology
    - Enabled in firmware (BIOS or UEFI)
- Memory
    - Allocation must meet minimum to support OS and/or applications
- Mass storage
    - Shared physical, separate logical
- Networking
    - Access between VMs, VM to host, VM to host network

![Bios settings for virtualization](/assets/biosvirtual.png)

### Virtualization Security Requirements

- Guest OS security (Any VM you setup)
    - Protect host OS from issues with VMs
- Host security
    - Host system is a single point of failure; should host go offline, all virtualized nodes hosted on it are also down
- Hypervisor security
    - Monitor for vulnerabilities within the hypervisor platform

## 8.2 CLOUD CONCEPTS

### Cloud Characteristics

- High availability (uptime)
    - Minimal downtime
- Scalability
    - Expand and contract virtual environment based on demand
- Elasticity
    - Expand and contract without affecting service or performance
- Shared resources

### Common Cloud Deployment Models
 
 - Public: Multitenancy *more than one person*
 - Private: Hosted private-cloud services hosted within a public provider, but dedicated to a single customer
 - Community
 - Hybrid

### Common Cloud Service Models

- Infrastructure (IaaS): Servers, storage, networking, load balancers
- Software (SaaS): Application fully run in cloud environment
- Platform (PaaS): Servers and storage like IaaS, but also has tools for development and deployment of applications like databases
- Desktop (DaaS)

![ec2 dashboard](/assets/ec2dashboard.png)

### Cloud File Storage

- File synchronization
    - Tracking of changes across multiple platforms
    - May include commenting features
- Content delivery networks
    - Replication across multiple datacenters
