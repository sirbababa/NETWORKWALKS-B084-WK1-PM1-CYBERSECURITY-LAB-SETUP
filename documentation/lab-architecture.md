Cybersecurity Lab Architecture

1. Introduction

The cybersecurity lab is designed using Oracle VirtualBox to create a virtual environment for practical cybersecurity and networking exercises.

2. Lab Components

Component	Description
Host Machine	Windows 10
Virtualization Software	Oracle VirtualBox 7.2.16
Virtual Machine	Kali Linux
Network Type	NAT Network
Network Name	CyberLab-NATNetwork
Network Subnet	10.0.0.0/24
Gateway	10.0.0.1
Required Kali IP	10.0.0.2/24

3. Network Design

The virtual machine connects to the CyberLab-NATNetwork network through its virtual network adapter.

The intended network configuration is:

* Network address: 10.0.0.0/24
* Gateway address: 10.0.0.1
* Kali Linux address: 10.0.0.2
* DHCP address range: 10.0.0.3–10.0.0.253

4. Architecture Diagram

             Windows 10 Host
                    |
             Oracle VirtualBox
                    |
             CyberLab-NATNetwork
               10.0.0.0/24
                    |
                Kali Linux
              10.0.0.2/24
                    |
               Internet Access

5. Purpose

This architecture provides a virtual environment for learning Linux, networking, cybersecurity tools, and security testing.

Note: The required Kali IP address and connectivity must be verified before being reported as successfully configured.
