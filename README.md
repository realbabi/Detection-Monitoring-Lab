# Detection-Monitoring-Lab
# Home Lab Setup

This guide outlines the setup for a comprehensive home lab environment, including network segmentation, security monitoring, attack simulation, and log management. The lab is hosted on a single PC using VMware Workstation.

## Overview

- **Hypervisor**: Using VMware Workstation to host all virtual machines.
- **Network Configuration**: Leveraging pfSense for firewall and network segmentation.
- **Intrusion Detection System**: Setting up Security Onion as an all-in-one solution for IDS, security monitoring, and log management.
- **Attack Simulation**: Configuring Kali Linux as an attack machine.
- **Domain Controller**: Utilizing a Windows Server as a domain controller.
- **Client Simulation**: Configuring Windows desktops for domain interaction.
- **Log Management**: Implementing Splunk for log aggregation and analysis.
- **Additional VMs**: Including Ubuntu, CentOS, Metasploitable, DVWA, and Vulnhub machines for various testing purposes.

## Home Lab Network Design & Topology
https://static.wixstatic.com/media/1f97f7_d7b77d2971dc4741aac5d1135b366f50~mv2.png/v1/fill/w_360,h_282,al_c,q_95/1f97f7_d7b77d2971dc4741aac5d1135b366f50~mv2.webp
### VMware Workstation Installation

VMware Workstation 16 Pro is utilized as the hypervisor for hosting all virtual machines within this lab environment.

### Network Configuration with pfSense

pfSense is configured to serve as the lab's firewall, providing network segmentation and security.

### Security Onion Configuration

Security Onion is deployed to provide comprehensive network security monitoring, intrusion detection, and log management capabilities.

### Kali Linux Setup

Kali Linux is set up as the attack machine to simulate various cybersecurity attacks within the lab environment.

### Windows Server and Desktop Configuration

A Windows Server is configured as the domain controller, along with Windows desktops to simulate a corporate network environment.

### Splunk Integration

Splunk is implemented for aggregating, analyzing, and visualizing logs from various sources within the lab.

### Adding Linux Machines

Several Linux machines, including Ubuntu, CentOS, Metasploitable, DVWA, and Vulnhub, are added to the network for exploitation, detection, or monitoring purposes.

## Detailed Setup Instructions

The following sections provide step-by-step instructions for configuring each component of the home lab.

[Detailed instructions for each component would follow here, but remember to keep them concise and to the point, avoiding the full reproduction of external content.]

## Conclusion

This home lab setup provides a robust environment for exploring various aspects of cybersecurity, from network security monitoring and log management to attack simulation and domain management. By following this guide, users can build a comprehensive lab environment suitable for a wide range of security exercises and experiments.
