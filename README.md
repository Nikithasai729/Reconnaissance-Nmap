# Reconnaissance & Nmap Scanning Lab

## Overview

This project demonstrates basic reconnaissance and network scanning techniques using Nmap in a virtual penetration testing lab environment. A vulnerable machine from VulnHub (Kioptrix Level 1) was deployed using VirtualBox, and Kali Linux was used to discover hosts, identify open ports, detect services, and analyze the attack surface.

---

## Objective

The objective of this project is to:

* Set up a vulnerable virtual machine environment
* Perform host discovery using Nmap
* Identify open ports and running services
* Detect operating system information
* Understand basic reconnaissance techniques

---

## Tools Used

* Kali Linux
* Nmap
* Oracle VirtualBox
* VulnHub – Kioptrix Level 1

---

## Lab Setup

### Attacker Machine

* Kali Linux VirtualBox Image

### Target Machine

* Kioptrix Level 1 Vulnerable VM

### Virtualization Platform

* Oracle VM VirtualBox

### Network Configuration

* Bridged Adapter / NAT Networking

---

## Procedure

### 1. Download and Configure Vulnerable Machine

* Downloaded Kioptrix Level 1 from VulnHub
* Extracted the VM files
* Added the VM into VirtualBox

### 2. Configure Kali Linux

* Downloaded Kali Linux VirtualBox image
* Imported Kali Linux into VirtualBox
* Started the virtual machine

### 3. Identify Network Information

Executed:

```bash id="e2djlwm"
ip a
```

This displayed the IP address assigned to Kali Linux.

### 4. Perform Host Discovery Scan

Executed:

```bash id="49n9v5"
sudo nmap -sn 10.0.2.0/24
```

This identified active hosts in the subnet.

### 5. Perform Aggressive Nmap Scan

Executed:

```bash id="jju5y6"
sudo nmap -A -T4 10.0.2.2
```

```bash id="8v2duj"
sudo nmap -A -T4 10.0.2.3
```

This performed:

* Service Detection
* Version Detection
* OS Detection
* Script Scanning
* Traceroute

---

## Results

* Successfully identified active hosts on the network
* Performed reconnaissance on target systems
* Detected operating system information
* Identified available services and ports
* Learned practical Nmap scanning techniques

---

## Screenshots

Add screenshots in the `screenshots` folder:

1. Kali Linux running
2. Output of `ip a`
3. Host discovery scan
4. Aggressive Nmap scan results

---

## Learning Outcomes

* Virtual lab environment setup
* Basic penetration testing workflow
* Network reconnaissance techniques
* Host discovery using Nmap
* Service enumeration
* OS detection

---

## Conclusion

This project provided hands-on experience in reconnaissance and network scanning using Nmap. By setting up a virtual cybersecurity lab using Kali Linux and Kioptrix, host discovery and attack surface analysis were successfully performed in a controlled environment.

---

## Author

Your Name
