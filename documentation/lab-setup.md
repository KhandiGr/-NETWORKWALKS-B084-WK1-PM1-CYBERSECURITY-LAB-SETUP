# 🔐 Cybersecurity Lab Environment Setup

## Lab Overview

This document outlines the setup, configuration, and verification of the cybersecurity lab environment for the B084 WK1 PM1 Cybersecurity Lab.

The lab uses VirtualBox and Kali Linux to create an isolated environment for cybersecurity activities, including network reconnaissance, port scanning, vulnerability assessment, and security testing.

The environment provides a controlled space to practice cybersecurity techniques while reducing the risk of affecting external systems.

## Lab Objectives

- Install and configure Oracle VirtualBox.
- Set up and import the Kali Linux virtual machine.
- Configure a dedicated NAT Network.
- Configure Kali Linux network connectivity.
- Assign and verify the Kali Linux IP address.
- Configure the gateway and DNS server.
- Test network connectivity and DNS resolution.
- Create a clean snapshot of the lab environment.
- Document the setup and verification process.

## Lab Configuration

| Component | Configuration |
|---|---|
| Host Operating System | Windows 10 |
| Virtualization Software | Oracle VirtualBox 7.2 |
| Virtual Machine | Kali Linux |
| Kali Linux RAM | 2048 MB |
| Network Mode | NAT Network |
| NAT Network Name | NatNetwork |
| Network Address | 10.0.0.0/24 |
| Kali Linux IP Address | 10.0.0.2/24 |
| Default Gateway | 10.0.0.1 |
| DNS Server | 10.0.0.1 |

## Lab Setup Procedure

### Step 1: Install 7-Zip

7-Zip was used to extract the Kali Linux virtual machine files where required.

### Step 2: Install VirtualBox

Oracle VirtualBox was installed to provide the virtualization environment for the cybersecurity lab.

### Step 3: Configure the NAT Network

A dedicated NAT Network named `NatNetwork` was configured in VirtualBox.

The network was configured with the following settings:

- Network: `10.0.0.0/24`
- DHCP: Enabled
- IPv6: Disabled

The NAT Network allows virtual machines to communicate with one another and access external networks through the host system.

### Step 4: Import and Configure Kali Linux

The Kali Linux virtual machine was imported into VirtualBox.

The virtual machine was configured with:

- 2048 MB RAM
- Network Adapter 1 connected to `NatNetwork`
- Intel PRO/1000 MT Desktop network adapter
- Shared folder configuration

### Step 5: Configure Kali Linux Networking

The Kali Linux network configuration was prepared using the following values:

| Setting | Value |
|---|---|
| IP Address | 10.0.0.2 |
| Gateway | 10.0.0.1 |
| DNS Server | 10.0.0.1 |

The gateway and DNS server were configured using `10.0.0.1`.

### Step 6: Create a Virtual Machine Snapshot

A snapshot was created to preserve the configured lab environment.

Snapshot name:

`Clean Kali - Network Setup`

The snapshot provides a baseline that can be restored if the virtual machine configuration is changed during future lab activities.

## What I Learned

This lab provided practical experience with:

- Installing and configuring VirtualBox.
- Importing and configuring a Kali Linux virtual machine.
- Understanding NAT Network configuration.
- Configuring IP addressing and network interfaces.
- Identifying the role of a default gateway.
- Configuring and testing DNS resolution.
- Verifying network connectivity.
- Creating and restoring virtual machine snapshots.
- Documenting cybersecurity lab configuration and verification.

## Security and Ethical Considerations

The cybersecurity lab is intended for authorized learning, testing, and experimentation.

Cybersecurity tools should only be used against systems and networks for which permission has been granted.

The isolated lab environment provides a controlled space for practicing cybersecurity techniques and understanding network security concepts.

## Lab Evidence

- [WK1 Lab Report (PDF)](Lab%20WK1.pdf)
- [WK1 Screenshots](../screenshots/)

## Tools Used

- 7-Zip
- Oracle VirtualBox
- Kali Linux

## Conclusion

The cybersecurity lab environment was prepared using VirtualBox and Kali Linux.

The lab setup provided an environment for practicing network configuration, connectivity verification, DNS resolution, and cybersecurity activities.

The configuration and verification activities are documented in this repository, with supporting screenshots and lab report files.
