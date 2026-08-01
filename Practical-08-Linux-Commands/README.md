#  Practical 8: Linux Commands

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-08-Linux-Commands/Linux%20Commands.png" alt="Linux Commands Practical" width="900"/>
</p>

<p align="center">

![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04%20LTS-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Bash-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-Educational-blue?style=for-the-badge)

</p>

---

#  Overview

Linux is the backbone of modern IT infrastructure. From enterprise servers and cloud platforms to cybersecurity operations and DevOps environments, Linux powers a significant portion of today's technology ecosystem. Unlike desktop operating systems, Linux professionals primarily interact with systems through the Command Line Interface (CLI), making command-line proficiency an essential skill for IT careers.

In this practical, you will explore the fundamental Linux commands used to navigate the file system, manage files and directories, search file contents, and configure file permissions. All demonstrations are performed on **Ubuntu 22.04 LTS** running inside **VMware Workstation**, providing a safe virtual lab environment for learning and experimentation.

This practical is designed for beginners who want to build a strong foundation in Linux Administration, Cybersecurity, Cloud Computing, DevOps, and IT Support.

---

#  Learning Objectives

After completing this practical, you will be able to:

- Understand the Linux Command Line Interface (CLI).
- Navigate directories using Linux navigation commands.
- Display files and folders using different variations of the `ls` command.
- Create and organize directories using `mkdir`.
- Create files using `touch`.
- Copy, move, rename, and delete files using Linux file management commands.
- Search file contents efficiently using `grep`.
- Understand Linux file permissions.
- Modify permissions securely using `chmod`.
- Perform common Linux system administration tasks.
- Gain practical experience working inside a Linux virtual machine.

---

#  Demonstration

<p align="center">

<a href="https://www.youtube.com/watch?v=pg-vjo2DsDo">
<img src="https://img.icons8.com/color/96/video.png" alt="Watch Practical"/>
<br>
<strong>▶ Watch the Complete Practical on YouTube</strong>

</a>

</p>

> **Video Duration:** ~9 Minutes  
> **Difficulty Level:** Beginner  
> **Operating System:** Ubuntu 22.04 LTS  
> **Category:** Linux Fundamentals

---

#  Prerequisites

Before performing this practical, ensure you have the following:

- Basic understanding of computer operating systems.
- VMware Workstation installed.
- Ubuntu 22.04 LTS Virtual Machine configured.
- Basic knowledge of keyboard and terminal usage.
- Administrator access to the Ubuntu virtual machine.
- Willingness to practice commands using the Linux Terminal.

---

#  Lab Environment

| Component | Details |
|-----------|---------|
| **Host Operating System** | Windows 11 |
| **Virtualization Software** | VMware Workstation |
| **Guest Operating System** | Ubuntu 22.04 LTS |
| **Shell** | Bash |
| **Terminal Emulator** | GNOME Terminal |
| **Architecture** | x86_64 |
| **User Account** | Standard Linux User |
| **Internet Connection** | Optional |

---

#  Tools Used

| Tool | Purpose |
|------|---------|
| Ubuntu 22.04 LTS | Linux Operating System |
| VMware Workstation | Virtualization Platform |
| Bash Shell | Linux Command Interpreter |
| GNOME Terminal | Terminal Emulator |
| Linux CLI | Command Line Interface |

---

#  Commands Practiced

The following Linux commands are demonstrated during this practical.

| Command | Purpose |
|----------|---------|
| `pwd` | Display current working directory |
| `ls` | List files and directories |
| `ls -l` | Display detailed file information |
| `ls -a` | Display hidden files |
| `cd` | Change directory |
| `mkdir` | Create a new directory |
| `touch` | Create an empty file |
| `cp` | Copy files |
| `mv` | Move or rename files |
| `rm` | Delete files |
| `grep` | Search text inside files |
| `chmod` | Change file permissions |

---

#  Areas Covered

| Area | Description |
|------|-------------|
| Linux Terminal | Introduction to the Linux Command Line Interface (CLI). |
| Directory Navigation | Navigate the Linux file system using `pwd` and `cd`. |
| File Listing | Display files and directories using `ls`, `ls -l`, and `ls -a`. |
| Directory Management | Create directories using the `mkdir` command. |
| File Management | Create files using `touch`. |
| Copy Files | Duplicate files safely using `cp`. |
| Move & Rename Files | Move files between directories or rename them using `mv`. |
| Delete Files | Remove files using the `rm` command. |
| Search File Content | Search text and keywords inside files using `grep`. |
| File Permissions | Understand and modify Linux permissions using `chmod`. |
| System Administration | Perform common Linux administration tasks through the terminal. |

---

#  Step-by-Step Practical Workflow

Follow these steps to complete the practical:

### Step 1 – Open Ubuntu Virtual Machine
- Launch **VMware Workstation**.
- Start the **Ubuntu 22.04 LTS Virtual Machine**.
- Open the **GNOME Terminal**.

---

### Step 2 – Check Current Directory

```bash
pwd
```

Displays the current working directory.

---

### Step 3 – List Files and Directories

```bash
ls
ls -l
ls -a
```

- Display files and folders.
- View detailed file information.
- Display hidden files.

---

### Step 4 – Navigate Directories

```bash
cd Desktop
pwd

cd ..
pwd

cd
pwd
```

Move between different directories within the Linux file system.

---

### Step 5 – Create a Directory

```bash
mkdir Linux_Practice
cd Linux_Practice
```

Create a new working directory for this practical.

---

### Step 6 – Create Files

```bash
touch notes.txt
```

Create an empty text file.

---

### Step 7 – Copy Files

```bash
cp notes.txt backup.txt
```

Create a backup copy of the file.

---

### Step 8 – Rename and Move Files

```bash
mv backup.txt backup_notes.txt

mkdir Backup

mv backup_notes.txt Backup/
```

Rename files and move them to another directory.

---

### Step 9 – Delete Files

```bash
touch test.txt

rm test.txt
```

Delete unnecessary files.

---

### Step 10 – Search Text Inside Files

Create a file using Nano Editor.

```bash
nano notes.txt
```

Add the following text:

```text
Linux is powerful.
Linux is widely used.
Cybersecurity teams use Linux.
```

Save the file.

Search for text.

```bash
grep Linux notes.txt

grep Cybersecurity notes.txt
```

---

### Step 11 – Change File Permissions

```bash
ls -l

chmod 777 notes.txt

ls -l

chmod 644 notes.txt

ls -l
```

Observe how Linux permissions change.

---

#  Real-World System Administrator Scenario

Imagine you are working as a **Linux System Administrator** for an organization. One morning, the development team reports that a web application hosted on a Linux server has stopped working.

To investigate the issue, you perform the following tasks:

1. Connect to the Linux server using SSH.
2. Navigate to the application directory using `cd`.
3. Verify your current location using `pwd`.
4. List files and permissions using `ls -l`.
5. Search application logs using `grep` to identify errors.
6. Verify configuration file permissions.
7. Correct permission issues using `chmod`.
8. Validate that the application is functioning correctly.

This workflow demonstrates how Linux administrators use these commands every day to troubleshoot production servers, investigate issues, and maintain secure systems.

---

#  Repository Structure

```text
Practical-08-Linux-Commands/
│
├── README.md
├── Linux Commands.png
├── Practical 8.pdf
└── Resources/
    └── Linux Commands.txt
```

---

#  Key Takeaways

- Linux command-line skills are essential for modern IT careers.
- Navigation commands allow efficient movement through the Linux file system.
- File management commands simplify administration tasks.
- The `grep` command enables quick searching inside files and log data.
- Linux file permissions protect sensitive system files.
- Understanding `chmod` is essential for securing Linux systems.
- These commands form the foundation of Linux Administration, Cybersecurity, Cloud Computing, DevOps, and IT Support.

---

#  Best Practices

- Practice commands inside a virtual machine before using them on production systems.
- Verify your current directory using `pwd` before performing operations.
- Use `ls -l` to review file permissions before making changes.
- Avoid using `chmod 777` on production servers unless absolutely necessary.
- Create backup copies of important files before modifying them.
- Read command documentation using:

```bash
man <command>
```

Example:

```bash
man grep
```

---

#  Further Learning

After completing this practical, consider exploring the following Linux topics:

- Linux File System Hierarchy
- File Ownership (`chown`)
- File Groups (`chgrp`)
- User and Group Management
- Linux Processes
- Shell Scripting (Bash)
- Linux Networking Commands
- SSH Remote Administration
- Linux Log Analysis
- Cron Jobs
- Package Management (`apt`)
- System Monitoring

---

# 👨‍💻 Author

**Himadri Singh**

- GitHub: https://github.com/himadri2324
- YouTube: https://www.youtube.com/@littlesunflower

---

# 📄 License

This project is created solely for **educational and learning purposes**.

You are welcome to use this practical for personal learning, teaching, and skill development. If you share or reference this work, please provide appropriate credit to the original repository.

---

<p align="center">
⭐ If you found this practical helpful, consider giving this repository a star and sharing it with others learning Linux and Cybersecurity.
</p>

---
