# Nmap Cheat Sheet

## Host Discovery

nmap -sn 192.168.1.0/24

---

## Scan Single Host

nmap 192.168.1.10

---

## Scan Multiple Hosts

nmap 192.168.1.10 192.168.1.20

---

## Scan Entire Subnet

nmap 192.168.1.0/24

---

## SYN Scan

nmap -sS IP

---

## TCP Connect Scan

nmap -sT IP

---

## UDP Scan

nmap -sU IP

---

## Version Detection

nmap -sV IP

---

## OS Detection

nmap -O IP

---

## Aggressive Scan

nmap -A IP

---

## Scan Specific Ports

nmap -p 22,80,443 IP

---

## Scan All Ports

nmap -p- IP

---

## Save Output

nmap -oN report.txt IP

---

## XML Output

nmap -oX report.xml IP

---

## Grepable Output

nmap -oG report.gnmap IP

---

## Verbose Mode

nmap -v IP

---

## Timing

nmap -T4 IP

---

## NSE Default Scripts

nmap -sC IP

---

## Vulnerability Scan

nmap --script vuln IP
