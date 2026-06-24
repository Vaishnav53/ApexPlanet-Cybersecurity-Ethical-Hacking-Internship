# Lab Environment Setup

## Objective

To establish a controlled cybersecurity testing environment using Kali Linux and Metasploitable2 virtual machines for security research, vulnerability assessment, and penetration testing exercises.

---

## Tools Used

* Oracle VirtualBox
* Kali Linux
* Metasploitable2
* Nmap
* Linux Networking Utilities

---

## Virtual Machine Configuration

### Attacker Machine

| Parameter        | Value             |
| ---------------- | ----------------- |
| Operating System | Kali Linux        |
| Role             | Attacker Machine  |
| Network Mode     | Host-Only Adapter |

### Target Machine

| Parameter        | Value             |
| ---------------- | ----------------- |
| Operating System | Metasploitable2   |
| Role             | Vulnerable Target |
| Network Mode     | Host-Only Adapter |

---

## Network Verification

The network connectivity between Kali Linux and Metasploitable2 was verified using ICMP echo requests (Ping).

### Evidence

* Ping Connectivity Test
* Routing Table Verification

---

## Service Discovery

An Nmap service version scan was performed against the Metasploitable2 machine to identify exposed services and determine running versions.

### Evidence

* Nmap Service Version Scan

---

## Results

The lab environment was successfully configured and verified.

The attacker machine (Kali Linux) was able to communicate with the target machine (Metasploitable2), and network services were successfully identified using Nmap.
