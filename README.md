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
<img src="https://static.wixstatic.com/media/1f97f7_c3819a585fb44cc896e93c99d512ba1a~mv2.jpg/v1/fill/w_740,h_496,al_c,q_90/1f97f7_c3819a585fb44cc896e93c99d512ba1a~mv2.webp" height="80%" width="80%" alt="Disk Sanitization Steps"/>

### VMware Workstation Installation

VMware Workstation 16 Pro is utilized as the hypervisor for hosting all virtual machines within this lab environment. I’ll use VMware Workstation 16 Pro as my hypervisor for this lab. This license costs about $120 with a student discount, but it is a worthwhile investment. VirtualBox is also a free and feature-rich alternative Hypervisor from Oracle. If you cannot afford the VMware license, VirtualBox is equally good.

### Network Configuration with pfSense

Pfsense will be configured as a firewall to segment our private homelab network and will be only accessible from our Kali Linux machine.
Click “Create a New Virtual Machine” on VMware Workstation Homescreen.

Make sure “Typical (recommended)” is selected and click Next.
https://static.wixstatic.com/media/1f97f7_d02e7abecb6844d582f05652b2c37154~mv2.png/v1/fill/w_360,h_442,al_c,q_95/1f97f7_d02e7abecb6844d582f05652b2c37154~mv2.webp

Click “Browse” and navigate to the folder where your pfsense file is located.

Click Next.
https://static.wixstatic.com/media/1f97f7_63b52e827b084f7db51adcc4b25e0a60~mv2.png/v1/fill/w_360,h_366,al_c,q_95/1f97f7_63b52e827b084f7db51adcc4b25e0a60~mv2.webp

Rename your Virtual Machine. Preferably “pfsense”

Click Next.

https://static.wixstatic.com/media/1f97f7_898063d9fc5b4de89132f664279f17d9~mv2.png/v1/fill/w_360,h_365,al_c,q_95/1f97f7_898063d9fc5b4de89132f664279f17d9~mv2.webp

20GB disk size is sufficient for this VM.

Ensure that the “Split virtual disk into multiple files” option is selected.

Click Next.

https://static.wixstatic.com/media/1f97f7_348d9ea51d1544cabc1dac259d222c24~mv2.png/v1/fill/w_360,h_329,al_c,q_95/1f97f7_348d9ea51d1544cabc1dac259d222c24~mv2.webp

Click “Customize Hardware”.

https://static.wixstatic.com/media/1f97f7_34ab981aadce4c76a8cbab08248f9b5c~mv2.png/v1/fill/w_360,h_352,al_c,q_95/1f97f7_34ab981aadce4c76a8cbab08248f9b5c~mv2.webp

https://static.wixstatic.com/media/1f97f7_34ab981aadce4c76a8cbab08248f9b5c~mv2.png/v1/fill/w_360,h_352,al_c,q_95/1f97f7_34ab981aadce4c76a8cbab08248f9b5c~mv2.webp

Increase the memory to 2GB.

https://static.wixstatic.com/media/1f97f7_a77b664e42b54fec97df442b7ae48ab7~mv2.png/v1/fill/w_360,h_339,al_c,q_95/1f97f7_a77b664e42b54fec97df442b7ae48ab7~mv2.webp

Add 5 network adapters and correspond them with a VMnet interface as shown below. Then click Finish.

https://static.wixstatic.com/media/1f97f7_a6dc26a3a64346a2b8b689681b792376~mv2.png/v1/fill/w_360,h_344,al_c,q_95/1f97f7_a6dc26a3a64346a2b8b689681b792376~mv2.webp
https://static.wixstatic.com/media/1f97f7_5e4c0107dadd4d79857fd8c0275f052e~mv2.png/v1/fill/w_360,h_316,al_c,lg_1,q_95/1f97f7_5e4c0107dadd4d79857fd8c0275f052e~mv2.webp

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
