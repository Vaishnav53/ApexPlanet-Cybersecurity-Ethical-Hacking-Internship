# Linux Fundamentals

## Introduction

Linux is an open-source operating system widely used in cybersecurity, penetration testing, server administration, cloud computing, and digital forensics. Most security tools, including Kali Linux, are built on Linux distributions.

---

# 1. File System Navigation

## pwd

### Purpose

Displays the current working directory.

### Syntax

```bash
pwd
```

### Example

```bash
pwd
```

### Output

```text
/home/vaishnav
```

### Cybersecurity Relevance

Helps security professionals identify their current location while navigating system files during assessments and investigations.

---

## ls

### Purpose

Lists files and directories.

### Syntax

```bash
ls
ls -l
ls -la
```

### Example

```bash
ls -la
```

### Cybersecurity Relevance

Used to enumerate files, hidden files, permissions, and directory contents during system analysis.

---

## cd

### Purpose

Changes the current directory.

### Syntax

```bash
cd <directory>
```

### Example

```bash
cd /etc
```

### Cybersecurity Relevance

Allows navigation through system directories during audits and penetration testing activities.

---

# 2. File & Directory Management

## mkdir

Creates a new directory.

```bash
mkdir project
```

---

## touch

Creates an empty file.

```bash
touch notes.txt
```

---

## cp

Copies files and directories.

```bash
cp source.txt backup.txt
```

---

## mv

Moves or renames files.

```bash
mv old.txt new.txt
```

---

## rm

Deletes files or directories.

```bash
rm file.txt
rm -r folder
```

---

## cat

Displays file contents.

```bash
cat notes.txt
```

---

# 3. File Permissions

Linux uses a permission model based on:

* Owner
* Group
* Others

## Viewing Permissions

```bash
ls -l
```

Example:

```text
-rwxr-xr-x
```

---

## chmod

Changes file permissions.

### Example

```bash
chmod 755 script.sh
```

### Meaning of 755

| Value  | Permission           |
| ------ | -------------------- |
| Owner  | Read, Write, Execute |
| Group  | Read, Execute        |
| Others | Read, Execute        |

---

## Common Permission Values

| Value | Meaning             |
| ----- | ------------------- |
| 777   | Full Access         |
| 755   | Standard Executable |
| 644   | Standard File       |
| 600   | Owner Only          |

---

## chown

Changes file ownership.

```bash
sudo chown user:user file.txt
```

---

# 4. Package Management

Package management allows software installation and updates.

## Update Package Lists

```bash
sudo apt update
```

---

## Upgrade Installed Packages

```bash
sudo apt upgrade
```

---

## Install Package

```bash
sudo apt install nmap
```

---

## Install Local Package

```bash
sudo dpkg -i package.deb
```

---

# 5. Networking Commands

## ip a

Displays network interface information.

```bash
ip a
```

---

## ping

Tests connectivity between systems.

```bash
ping 192.168.1.3
```

---

## netstat

Displays network connections and listening ports.

```bash
netstat -tulpn
```

---

## ss

Modern alternative to netstat.

```bash
ss -tulpn
```

---

## traceroute

Shows packet path to destination.

```bash
traceroute google.com
```

---

# 6. User Management

## whoami

Displays current user.

```bash
whoami
```

---

## id

Displays user and group information.

```bash
id
```

---

## passwd

Changes user password.

```bash
passwd
```

---

# 7. Process Management

## ps

Displays running processes.

```bash
ps aux
```

---

## top

Real-time process monitoring.

```bash
top
```

---

## htop

Interactive process viewer.

```bash
htop
```

---

## kill

Terminates a process.

```bash
kill <PID>
```

---

# Importance of Linux in Cybersecurity

Linux is the primary operating system used by cybersecurity professionals due to its flexibility, transparency, command-line capabilities, security tools, and extensive networking features. Most penetration testing distributions, including Kali Linux, Parrot OS, and BlackArch, are Linux-based.

---

# Conclusion

Linux fundamentals form the foundation of cybersecurity operations. Understanding navigation, permissions, networking, package management, and process control is essential for system administration, penetration testing, vulnerability assessment, and incident response.
