# Practical 7: Linux Hands-On – Connect via SSH

## Overview

This practical introduces Secure Shell (SSH), one of the most essential protocols for remotely accessing and managing Linux systems. In this hands-on lab, you will configure an Ubuntu 22.04 LTS virtual machine as an SSH server, verify that the SSH service is running, identify the server's IP address, and establish a secure remote connection from a client machine.

SSH is widely used by Linux Administrators, Cloud Engineers, DevOps Engineers, IT Support Professionals, SOC Analysts, and Cybersecurity Engineers for secure remote system administration and troubleshooting.

<p align="center">
  <img src=""
       alt="SSH Hands-On"
       width="900"/>
</p>

---

## Learning Objectives

After completing this practical, you will be able to:

- Understand the purpose of SSH (Secure Shell).
- Install the OpenSSH Server package on Ubuntu 22.04 LTS.
- Verify the SSH service status.
- Identify the server's IP address.
- Connect securely to the Ubuntu server using SSH.
- Execute basic Linux commands through a remote SSH session.
- Understand real-world use cases of SSH in enterprise environments.

---

## 🎬 Demonstration

<p align="center">
  <a href="YOUR_FULL_VIDEO_LINK">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo" />
    <br>
    <strong>Click to watch the demonstration video</strong>
  </a>
</p>

---

# Overall Practical

## Areas Covered

| Area | Description |
|----------------------------|--------------------------------------------------------------|
| SSH Fundamentals | Understand Secure Shell (SSH) and its purpose |
| OpenSSH Installation | Install the OpenSSH Server package on Ubuntu |
| Service Management | Verify that the SSH service is active and running |
| Network Configuration | Find the Ubuntu server's IP address |
| Remote Access | Connect securely to the Ubuntu server using SSH |
| Remote Command Execution | Execute Linux commands after successful login |
| Enterprise Use Case | Understand how SSH is used in production environments |

---

## Lab Environment

| Component | Configuration |
|----------------------|--------------------------------------|
| Host Operating System | Windows 10/11 |
| Virtualization Platform | VMware Workstation |
| Guest Operating System | Ubuntu 22.04 LTS |
| Remote Access Protocol | SSH (Secure Shell) |
| Default SSH Port | TCP Port 22 |
| Internet Connection | Required for package installation |

---

## Tools Used

- VMware Workstation
- Ubuntu 22.04 LTS
- OpenSSH Server
- Linux Terminal
- Windows PowerShell / Command Prompt (SSH Client)

---

## Key Takeaways

- SSH provides secure remote access to Linux systems.
- OpenSSH Server enables Ubuntu to accept SSH connections.
- The SSH service must be running before remote clients can connect.
- The server's IP address is required for establishing an SSH session.
- SSH encrypts communication between the client and the server.
- Remote administration through SSH is a standard practice in Linux, cloud, and cybersecurity environments.

---

## Repository Structure

```text
Practical-7-Linux-Hands-On/
│
├── README.md
├── Images/
│   ├── ssh-overview.png
│   ├── ssh-architecture.png
│   └── practical-demo.png
│
├── Commands/
│   └── ssh-commands.md
│
└── Resources/
    └── additional-notes.md
```

---

## Commands Used

```bash
# Update package list
sudo apt update

# Install OpenSSH Server
sudo apt install openssh-server

# Verify SSH service status
systemctl status ssh

# Display server IP address
hostname -I

# Connect to the server (from client)
ssh username@server-ip

# Exit SSH session
exit
```

---

## Author

**Himadri Singh**

---

## License

This practical is created for educational and learning purposes.
