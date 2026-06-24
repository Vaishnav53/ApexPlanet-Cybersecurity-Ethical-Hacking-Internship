# Linux Command Cheat Sheet

## File System Navigation

| Command      | Description                           |
| ------------ | ------------------------------------- |
| pwd          | Display current directory             |
| ls           | List files and directories            |
| ls -la       | List all files including hidden files |
| cd directory | Change directory                      |
| cd ..        | Move one directory up                 |
| cd ~         | Move to home directory                |

---

## File & Directory Management

| Command               | Description         |
| --------------------- | ------------------- |
| mkdir folder          | Create directory    |
| touch file.txt        | Create file         |
| cp source destination | Copy file           |
| mv old new            | Move or rename file |
| rm file.txt           | Delete file         |
| rm -r folder          | Delete directory    |
| cat file.txt          | View file contents  |

---

## File Permissions

| Command              | Description        |
| -------------------- | ------------------ |
| ls -l                | View permissions   |
| chmod 755 file       | Change permissions |
| chmod +x script.sh   | Make executable    |
| chown user:user file | Change ownership   |

### Common Permission Values

| Value | Permission                      |
| ----- | ------------------------------- |
| 777   | Read, Write, Execute for all    |
| 755   | Owner Full, Others Read/Execute |
| 644   | Owner Read/Write, Others Read   |
| 600   | Owner Only                      |

---

## User Management

| Command      | Description              |
| ------------ | ------------------------ |
| whoami       | Current user             |
| id           | User information         |
| passwd       | Change password          |
| sudo command | Execute as administrator |

---

## Package Management

| Command                  | Description                |
| ------------------------ | -------------------------- |
| sudo apt update          | Update package list        |
| sudo apt upgrade         | Upgrade installed packages |
| sudo apt install package | Install package            |
| sudo apt remove package  | Remove package             |
| dpkg -i file.deb         | Install local package      |

---

## Networking Commands

| Command         | Description       |
| --------------- | ----------------- |
| ip a            | Show interfaces   |
| ping host       | Connectivity test |
| netstat -tulpn  | Open ports        |
| ss -tulpn       | Socket statistics |
| traceroute host | Route path        |
| nslookup domain | DNS lookup        |

---

## Process Management

| Command  | Description            |
| -------- | ---------------------- |
| ps aux   | Running processes      |
| top      | Real-time monitoring   |
| htop     | Interactive monitoring |
| kill PID | Stop process           |

---

## Nmap Quick Commands

```bash
nmap <IP>
nmap -sV <IP>
nmap -O <IP>
nmap -A <IP>
```

---

## Netcat Quick Commands

```bash
nc -lvnp 4444
nc <IP> 4444
```

---

## Wireshark Filters

```text
http
dns
ftp
tcp
udp
ip.addr == 192.168.56.101
```

---

## Cybersecurity Tip

Always verify commands before execution and avoid running unknown scripts with root privileges.
