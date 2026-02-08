# Linux Fundamentals Part 2 (TryHackMe)

## Overview
This lab continued my Linux learning by teaching me how to use command arguments, create and manage files and folders, switch users, understand numeric permissions, and explore important Linux system directories.

---

## What I learned

### 1. Command Arguments (Flags / Switches)
- Many commands accept arguments using `-` or `--`
- Arguments change the behavior of a command
- Example:
  - `ls` → shows files
  - `ls -a` → shows hidden files
- `--help` shows available options
- `man <command>` opens the manual page with full documentation

---

### 2. File and Folder Management
- Create files with: `touch`
- Create folders with: `mkdir`
- Remove files with: `rm`
- Remove folders with: `rm -R`
- Copy files with: `cp`
- Move or rename files with: `mv`
- Check file type with: `file`

---

### 3. Switching Users
- Use `su <username>` to switch accounts
- `su -l <username>` loads the full user environment
- Switching users requires that user’s password
- Useful for checking permissions and testing access

---

### 4. Understanding File Permissions
- Permissions control who can read, write, or execute a file
- Three groups: **Owner**, **Group**, **Others**
- Permission letters:
  - `r` = read
  - `w` = write
  - `x` = execute

#### Numeric Values
- `r = 4`
- `w = 2`
- `x = 1`

Examples:
- `rwxr-xr-x` → **755**
- `rw-r--r--` → **644**

These numbers are used with `chmod`.

---

### 5. Important Linux Directories
- **/etc** → system configuration files (sudoers, passwd, shadow)
- **/var** → logs and frequently changing data
- **/root** → home directory of root user
- **/tmp** → temporary files, cleared on reboot, writable by all users

---

## Commands practiced
- ls
- ls -a
- ls --help
- man ls
- touch
- mkdir
- rm
- rm -R
- cp
- mv
- file
- su
- su -l
- chmod (numeric permissions)

---

## What I practiced
- Using flags and understanding command arguments
- Viewing documentation using `--help` and `man`
- Creating, copying, moving, and deleting files and folders
- Switching between users and understanding their environments
- Reading file permissions and converting them to numeric format
- Exploring system folders like /etc, /var, /root, /tmp

---

## Why this matters
- Flags make commands more powerful and flexible
- File management is essential for every Linux job
- User switching is important for privilege escalation and troubleshooting
- Numeric permissions are important for system security
- Knowing system directories helps in cybersecurity, pentesting, and system administration
- These skills support log analysis, scripting, and running security tools
