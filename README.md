# Linux Command Guide

This repository contains Linux commands I am learning while studying Linux fundamentals and cybersecurity operations.

---

## 1. File & Directory Management

| Command | Description |
|--------|-------------|
| ls | List files in a directory |
| ls -la | Show hidden files with detailed information |
| cd /path | Change directory |
| pwd | Show current directory |
| mkdir foldername | Create a new directory |
| rmdir foldername | Remove empty directory |

---

## 2. File Operations

| Command | Description |
|--------|-------------|
| cp file1 file2 | Copy file |
| mv file1 file2 | Move or rename file |
| rm file | Delete file |
| rm -r folder | Delete directory recursively |
| touch filename | Create an empty file |

---

## 3. File Permissions

| Command | Description |
|--------|-------------|
| chmod 755 file | Change file permissions |
| chmod +x script.sh | Make file executable |
| chown user file | Change file owner |

Example:

chmod 755 script.sh

---

## 4. System Monitoring

| Command | Description |
|--------|-------------|
| top | Show running processes |
| htop | Interactive process viewer |
| df -h | Check disk space |
| free -m | Check RAM usage |
| uptime | Show system uptime |

---

## 5. Networking Commands

| Command | Description |
|--------|-------------|
| ip a | Show network interfaces |
| ping google.com | Test network connectivity |
| netstat -tuln | Show open ports |
| ss -tuln | Display listening ports |
| traceroute google.com | Trace network path |

---

## 6. User Management

| Command | Description |

| adduser username | Create new user |
| passwd username | Change user password |
| userdel username | Delete user |
| whoami | Show current user |

---

## 7. Log Investigation (Useful for SOC)

| Command | Description |
|--------|-------------|
| cat /var/log/syslog | View system logs |
| tail -f /var/log/syslog | Monitor logs in real time |
| grep "error" logfile | Search for errors in logs |

Example:

grep "failed" /var/log/auth.log

---

## Learning Goal

This repository is part of my learning journey into:

- Linux System Administration  
- Cybersecurity Operations  
- SOC Analysis


  ## Practical Command Examples

### Example 1: Checking Disk Usage

df -h

Output example:

Filesystem      Size  Used Avail Use% Mounted on
/dev/sda1        50G   20G   28G  42% /


### Example 2: Checking Running Processes

top

This command shows CPU usage, memory usage, and active processes.



### Example 3: Testing Network Connectivity

ping google.com

This checks whether the system can reach external networks.

## Linux Practice Lab

Some exercises I performed while learning Linux fundamentals.

### Task 1: Create and Navigate Directories

mkdir practice_folder
cd practice_folder
touch testfile.txt

### Task 2: Change File Permissions

chmod 755 testfile.txt

### Task 3: Search Logs for Failed Login Attempts

grep "failed" /var/log/auth.log

