# Network Reconnaissance & Service Fingerprinting Analysis 

## Project Overview
This project demonstrates the use of Nmap and Zenmap to perform comprehensive network reconnaissance. The goal was to map the attack surface of various targets (Localhost, Network Assets, and External Servers) to identify open ports, active services, and potential security misconfigurations.

## Tools & Technologies
* **Nmap:** Command-line network mapper.
* **Zenmap:** GUI version of Nmap for visual analysis.
* **Linux/Windows:** Cross-platform scanning environments.

##  Scanning Methodology
I utilized several Nmap flags to gather deep technical data:
* `nmap -sV`: Service Version Detection to identify software versions (e.g., Apache 2.4.7, OpenSSH 6.6.1p1).
* `nmap -A`: Aggressive scanning for OS Fingerprinting, Traceroute, and Script Scanning.
* `nmap -T4`: Optimized timing for faster scanning in lab environments.

##  Key Findings
1. **Service Mapping:** Identified critical services including SSH (Port 22), HTTP (Port 80), and RPC (Port 135).
2. **Vulnerability Assessment:** Detected outdated service versions (like Apache 2.4.7) which are associated with known CVEs, highlighting the need for patch management.
3. **OS Fingerprinting:** Successfully identified target operating systems (Linux 4.X/5.X) using TCP/IP stack analysis.
4. **Network Topology:** Performed hop-by-hop traceroute analysis to visualize the path to the target server.

## Project Screenshots
Below are the visual results of the scanning process:

### 1. Localhost Baseline Scan
![nmap3](https://github.com/user-attachments/assets/08737313-727d-41e2-af26-3fcceee81c01)


### 2. External Target Identification
![nmap](https://github.com/user-attachments/assets/705ffde6-6cf9-4997-933e-0fffa1a687d4)


### 3. Service Version Detection (-sV)
![nmap1](https://github.com/user-attachments/assets/15041819-1a13-4026-8da4-fac58c1a4e44)


### 4. Deep Dive & OS Fingerprinting (-A)
![nmap2](https://github.com/user-attachments/assets/4001901b-270a-4ea1-aa24-84c5442e3329)


### 5. Advanced Fingerprinting Metadata
![nmap4](https://github.com/user-attachments/assets/96a705c9-1e42-4187-8030-6769dce3d2aa)


### 6. Subnet Asset Discovery
![nmap6](https://github.com/user-attachments/assets/f5d9cb7d-a627-4d5b-b552-d35824635988)


## Conclusion
As an aspiring **SOC Analyst**, this project emphasizes the importance of visibility. By identifying unauthorized open ports and outdated services, security teams can proactively reduce the attack surface and prevent exploitation before it occurs.
