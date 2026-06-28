# Nmap Scanning

## Introduction

Nmap (Network Mapper) is one of the most popular open-source network scanning tools used by security professionals, penetration testers, and system administrators.

It is used to discover hosts, identify open ports, detect running services, determine operating systems, and identify vulnerabilities.

---

# Features

- Host Discovery
- Port Scanning
- Service Detection
- OS Detection
- Version Detection
- NSE Scripting
- Firewall Detection

---

# Types of Scans

## TCP Connect Scan

Performs a complete TCP handshake.

Command

nmap -sT IP

---

## SYN Scan

Half-open scan.

Command

nmap -sS IP

---

## UDP Scan

Scans UDP ports.

Command

nmap -sU IP

---

## Service Version Detection

Command

nmap -sV IP

---

## Operating System Detection

Command

nmap -O IP

---

## Aggressive Scan

Command

nmap -A IP

---

## Ping Scan

Command

nmap -sn IP

---

# Common Uses

- Network Inventory
- Security Auditing
- Vulnerability Assessment
- Firewall Testing
- Service Discovery

---

# Advantages

- Fast
- Accurate
- Free
- Cross-platform

---

# Interview Questions

- What is Nmap?
- Difference between SYN and TCP Scan?
- What does -A do?
- What is OS Detection?
- What is NSE?
