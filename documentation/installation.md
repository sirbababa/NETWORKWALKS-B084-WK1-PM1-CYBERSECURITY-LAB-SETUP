Kali Linux Lab Installation and Configuration

1. Introduction

This document describes the installation and initial configuration of Kali Linux as a virtual machine using Oracle VirtualBox.

2. Host Environment

* Operating System: Windows 10
* Virtualization Software: Oracle VirtualBox 7.2.16

3. Virtual Machine

* Virtual Machine Name: Kali Linux
* Guest Operating System: Kali GNU/Linux Rolling
* Version: 2026.2

4. Network Configuration

The virtual machine is connected to a VirtualBox NAT Network named CyberLab-NATNetwork.

The required network settings are:

* Network: 10.0.0.0/24
* Gateway: 10.0.0.1
* Kali Linux IP: 10.0.0.2/24

5. Initial Configuration Tasks

The following configuration tasks are part of the lab:

1. Create the Kali Linux virtual machine.
2. Attach its network adapter to CyberLab-NATNetwork.
3. Configure the required static IP address.
4. Configure DNS and internet connectivity.
5. Enable bidirectional clipboard and drag-and-drop.
6. Configure the shared folder between Windows and Kali Linux.

6. Verification

The following Linux commands can be used to verify the configuration:

Check IP address

ip addr show eth0

Check network interfaces

nmcli device status

Test gateway connectivity

ping -c 4 10.0.0.1

Test internet connectivity

ping -c 4 1.1.1.1

Test DNS resolution

ping -c 4 google.com

7. Configuration Status

The required static IP address and internet connectivity will be marked as completed only after successful verification.
