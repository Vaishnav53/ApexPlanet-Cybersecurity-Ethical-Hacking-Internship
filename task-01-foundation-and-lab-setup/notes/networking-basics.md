# Networking Basics

## Introduction

Networking is the foundation of communication between devices, systems, and applications. Understanding networking concepts is essential for cybersecurity professionals because most attacks, defenses, monitoring, and investigations occur over networks.

---

# 1. OSI Model

The Open Systems Interconnection (OSI) Model consists of seven layers that describe how data travels across a network.

| Layer | Name         | Function                              |
| ----- | ------------ | ------------------------------------- |
| 7     | Application  | User interaction and network services |
| 6     | Presentation | Data formatting and encryption        |
| 5     | Session      | Session establishment and management  |
| 4     | Transport    | Reliable data delivery                |
| 3     | Network      | Routing and IP addressing             |
| 2     | Data Link    | MAC addressing and switching          |
| 1     | Physical     | Hardware and signal transmission      |

---

## Memory Trick

```text
Application
Presentation
Session
Transport
Network
Data Link
Physical
```

Mnemonic:

```text
All People Seem To Need Data Processing
```

---

# 2. TCP/IP Model

The TCP/IP model is the practical networking model used on the Internet.

| TCP/IP Layer   | Corresponding OSI Layers           |
| -------------- | ---------------------------------- |
| Application    | Application, Presentation, Session |
| Transport      | Transport                          |
| Internet       | Network                            |
| Network Access | Data Link, Physical                |

---

# 3. DNS (Domain Name System)

DNS translates domain names into IP addresses.

### Example

```text
www.google.com
↓
142.250.x.x
```

### Common DNS Record Types

| Record | Purpose              |
| ------ | -------------------- |
| A      | IPv4 Address         |
| AAAA   | IPv6 Address         |
| MX     | Mail Server          |
| CNAME  | Alias                |
| TXT    | Verification Records |

---

# 4. HTTP

HTTP (Hypertext Transfer Protocol) is used for web communication.

### Characteristics

* Port 80
* Unencrypted
* Plain text communication

### Example Request

```http
GET / HTTP/1.1
Host: example.com
```

---

# 5. HTTPS

HTTPS is the secure version of HTTP.

### Characteristics

* Port 443
* Uses SSL/TLS
* Encrypts communication

### Benefits

* Confidentiality
* Integrity
* Authentication

---

# 6. IP Addressing

An IP address uniquely identifies a device on a network.

### IPv4 Example

```text
192.168.1.100
```

### Structure

```text
Network Portion + Host Portion
```

---

# Private IP Ranges

| Range                         | Class |
| ----------------------------- | ----- |
| 10.0.0.0 - 10.255.255.255     | A     |
| 172.16.0.0 - 172.31.255.255   | B     |
| 192.168.0.0 - 192.168.255.255 | C     |

---

# 7. Subnetting

Subnetting divides a large network into smaller networks.

### Example

```text
192.168.1.0/24
```

### Meaning

```text
24 bits = Network
8 bits = Host
```

### Benefits

* Better performance
* Improved security
* Easier management

---

# 8. NAT (Network Address Translation)

NAT allows multiple devices to share a single public IP address.

### Types

* Static NAT
* Dynamic NAT
* PAT (Port Address Translation)

### Benefits

* Conserves IP addresses
* Hides internal networks
* Provides basic security

---

# 9. Common Ports & Protocols

| Protocol | Port | Purpose              |
| -------- | ---- | -------------------- |
| FTP      | 21   | File Transfer        |
| SSH      | 22   | Secure Remote Access |
| Telnet   | 23   | Remote Access        |
| SMTP     | 25   | Email Sending        |
| DNS      | 53   | Name Resolution      |
| HTTP     | 80   | Web Traffic          |
| POP3     | 110  | Email Retrieval      |
| IMAP     | 143  | Email Access         |
| HTTPS    | 443  | Secure Web Traffic   |
| SMB      | 445  | File Sharing         |
| RDP      | 3389 | Remote Desktop       |

---

# Cybersecurity Relevance

Understanding networking is essential for:

* Reconnaissance
* Network Scanning
* Vulnerability Assessment
* Packet Analysis
* Firewall Configuration
* Intrusion Detection
* Incident Response

---

# Conclusion

Networking forms the backbone of cybersecurity. A strong understanding of protocols, addressing, DNS, HTTP/HTTPS, and network communication is essential for security professionals.
