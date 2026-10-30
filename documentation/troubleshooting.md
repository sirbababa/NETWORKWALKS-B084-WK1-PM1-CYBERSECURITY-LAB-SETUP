
Lab Troubleshooting Notes

1. Introduction

This document records potential issues encountered during the configuration of the Kali Linux cybersecurity lab and the steps taken to investigate them.

2. Network Configuration Issue

Problem

After configuring the Kali Linux network adapter to use a static IP address, the network interface showed a disconnected state and did not obtain an IP address.

Environment

* Virtualization software: Oracle VirtualBox 7.2.16
* Virtual machine: Kali Linux
* Network: CyberLab-NATNetwork
* Required IP: 10.0.0.2/24

Investigation

The following commands were used to inspect the network:

ip addr show eth0
nmcli device status

The VirtualBox NAT Network and DHCP server settings were also inspected using:

VBoxManage.exe natnetwork list
VBoxManage.exe list dhcpservers

Status

The network issue is still under investigation. A successful connection and connectivity tests are required before considering it resolved.

3. Useful Troubleshooting Commands

Check network interfaces:

ip link show

Check IP configuration:

ip addr

Check routing table:

ip route

Check NetworkManager:

nmcli device status

4. Conclusion

Troubleshooting is an important part of setting up a reliable cybersecurity lab. Network configuration and connectivity must be tested before practical security exercises begin.
