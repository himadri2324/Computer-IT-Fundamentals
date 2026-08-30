# Practical 7: Linux Hands-On – Connect via SSH

<p align="center">
  <img src="Images/practical-7-ssh-overview.png"
       alt="Practical 7 - Linux Hands-On Connect via SSH"
       width="1000"/>
</p>

## Overview

Secure Shell (SSH) is one of the most widely used protocols for securely accessing and managing Linux systems remotely.

In this practical, an **Ubuntu 22.04 LTS virtual machine** is configured as an SSH server using **OpenSSH Server**. The SSH service is installed and verified, the server IP address is identified, and a secure remote connection is established from a client machine.

The practical also demonstrates basic Linux command execution through a remote SSH session and explains how SSH is commonly used in Linux administration, cloud infrastructure, DevOps, IT operations, and cybersecurity environments.

---

## Learning Objectives

After completing this practical, you will be able to:

- Understand the purpose of SSH (Secure Shell).
- Understand the role of an SSH client and SSH server.
- Install the OpenSSH Server package on Ubuntu 22.04 LTS.
- Verify the SSH service using `systemctl`.
- Identify the IP address of the Ubuntu server.
- Establish a secure SSH connection from a client machine.
- Execute basic Linux commands through a remote SSH session.
- Properly terminate an SSH session.
- Understand common enterprise use cases of SSH.
- Understand basic security considerations for SSH.

---

# What is SSH?

**SSH (Secure Shell)** is a network protocol used to securely connect to and manage remote computers over a network.

SSH provides an encrypted communication channel between the client and server. This helps protect authentication credentials, commands, and other information transmitted during a remote session.

SSH is commonly used by:

- Linux Administrators
- System Administrators
- Cloud Engineers
- DevOps Engineers
- IT Support Teams
- SOC Analysts
- Cybersecurity Engineers

The default SSH port is:

```text
TCP Port 22
````

---

# SSH Client and SSH Server

An SSH connection consists of two main components:

```text
+-----------------------+          +-------------------------+
|      SSH Client       |          |       SSH Server        |
|-----------------------|          |-------------------------|
| Windows PowerShell    |          | Ubuntu 22.04 LTS        |
| Windows Terminal      |  SSH     | OpenSSH Server          |
| Linux Terminal        | -------> | sshd service            |
+-----------------------+          +-------------------------+
                                             |
                                             |
                                      TCP Port 22
```

The **SSH client** initiates the connection.

The **SSH server** listens for incoming SSH connections and provides the remote shell after successful authentication.

---

# Lab Environment

| Component               | Configuration                       |
| ----------------------- | ----------------------------------- |
| Host Operating System   | Windows 10 / Windows 11             |
| Virtualization Platform | VMware Workstation                  |
| Guest Operating System  | Ubuntu 22.04 LTS                    |
| Remote Access Protocol  | SSH                                 |
| SSH Server              | OpenSSH Server                      |
| Default SSH Port        | TCP 22                              |
| SSH Client              | Windows PowerShell / Command Prompt |
| Network                 | VMware Virtual Network              |
| Internet Connection     | Required for package installation   |

> **Note:** Internet access is required to download the OpenSSH Server package from the Ubuntu repositories. The SSH connection itself can be established over a local or private network.

---

# Tools Used

* VMware Workstation
* Ubuntu 22.04 LTS
* OpenSSH Server
* Linux Terminal
* Windows PowerShell
* Windows Command Prompt
* SSH Client

---

# Practical Workflow

The practical follows the workflow below:

```text
Ubuntu Virtual Machine
        |
        v
Update Package Repository
        |
        v
Install OpenSSH Server
        |
        v
Verify SSH Service
        |
        v
Identify Server IP Address
        |
        v
Open SSH Client
        |
        v
Connect to Ubuntu Server
        |
        v
Authenticate User
        |
        v
Execute Remote Commands
        |
        v
Exit SSH Session
```

---

# Step 1: Update the Package Repository

Before installing OpenSSH Server, update the Ubuntu package repository information.

Run:

```bash
sudo apt update
```

This command refreshes the local package index and retrieves information about available packages and updates from the configured Ubuntu repositories.

---

# Step 2: Install OpenSSH Server

Install the OpenSSH Server package using:

```bash
sudo apt install openssh-server -y
```

The `-y` option automatically confirms the installation prompt.

OpenSSH Server provides the server-side functionality required for Ubuntu to accept incoming SSH connections.

After installation, the SSH service is managed by the systemd service:

```text
ssh.service
```

---

# Step 3: Verify the SSH Service

After installing OpenSSH Server, verify that the SSH service is running.

Run:

```bash
systemctl status ssh
```

A successful configuration should display:

```text
Active: active (running)
```

The command also provides information about the SSH daemon and the port on which the server is listening.

### SSH Service Status

![SSH Service Status](Images/ssh-service-status.png)

The screenshot above shows that:

* The OpenSSH Secure Shell server is loaded.
* The SSH service is enabled.
* The SSH service is **active (running)**.
* The `sshd` daemon is running.
* The server is listening on **TCP port 22**.
* The service is listening for IPv4 and IPv6 connections.

The service output includes entries similar to:

```text
Server listening on 0.0.0.0 port 22.
Server listening on :: port 22.
```

This confirms that the SSH server is listening for incoming connections on port 22.

---

# Step 4: Identify the Server IP Address

The client needs the IP address of the Ubuntu server to establish the SSH connection.

Run:

```bash
hostname -I
```

Example output:

```text
192.168.1.100
```

The actual IP address will depend on the VMware network configuration and the network environment being used.

Make a note of the IP address because it will be required in the SSH connection command.

---

# Step 5: Connect to the Ubuntu Server

From the client machine, open:

* Windows PowerShell
* Windows Command Prompt
* Windows Terminal

Use the following syntax:

```bash
ssh username@server-ip
```

For example:

```bash
ssh stem@192.168.1.100
```

Replace:

```text
username
```

with the Ubuntu account username and:

```text
server-ip
```

with the IP address obtained in the previous step.

---

## First-Time SSH Connection

When connecting to the SSH server for the first time, the client may display a host authenticity message similar to:

```text
The authenticity of host '192.168.1.100' can't be established.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

After verifying that the server address is correct, enter:

```text
yes
```

The SSH client will then request the password of the specified Ubuntu user.

After successful authentication, the client will receive a remote shell on the Ubuntu server.

---

# Step 6: Verify the Remote SSH Session

Once the SSH connection is established, commands entered into the terminal are executed on the remote Ubuntu server.

### Check the Current User

```bash
whoami
```

This displays the username associated with the current SSH session.

### Check the Server Hostname

```bash
hostname
```

This displays the hostname of the remote Ubuntu system.

### Check the Current Directory

```bash
pwd
```

This displays the current working directory.

### List Files and Directories

```bash
ls
```

This displays files and directories in the current location.

### Display System Information

```bash
uname -a
```

This displays Linux kernel and system information.

These commands demonstrate that the SSH connection provides interactive remote command-line access to the Ubuntu server.

---

# Step 7: Exit the SSH Session

After completing the remote administration tasks, terminate the SSH session using:

```bash
exit
```

The SSH connection will close and the client will return to its local command prompt.

---

# Commands Used

```bash
# Update Ubuntu package information
sudo apt update

# Install OpenSSH Server
sudo apt install openssh-server -y

# Verify SSH service status
systemctl status ssh

# Display the Ubuntu server IP address
hostname -I

# Connect to the Ubuntu server
ssh username@server-ip

# Display the currently logged-in user
whoami

# Display the server hostname
hostname

# Display the current working directory
pwd

# List files and directories
ls

# Display Linux system information
uname -a

# Exit the SSH session
exit
```

---

# Understanding the SSH Service

The OpenSSH server uses the **`sshd` daemon** to handle incoming SSH connections.

The basic communication flow is:

```text
+------------------+
|    SSH Client    |
| Windows / Linux  |
+--------+---------+
         |
         | SSH Connection
         | TCP Port 22
         v
+------------------+
|   Ubuntu Server  |
+--------+---------+
         |
         v
+------------------+
|      sshd        |
| SSH Server Daemon|
+--------+---------+
         |
         v
+------------------+
| User Authentication |
+--------+---------+
         |
         v
+------------------+
|   Remote Shell   |
+------------------+
```

The SSH server is controlled by the `ssh.service` systemd unit.

The service can be checked using:

```bash
systemctl status ssh
```

A running SSH server should report:

```text
Active: active (running)
```

---

# Understanding TCP Port 22

The default port used by SSH is:

```text
TCP 22
```

The SSH service status in this practical confirms that the server is listening on port 22.

Example:

```text
Server listening on 0.0.0.0 port 22.
Server listening on :: port 22.
```

The first entry represents listening on IPv4 addresses, while the second represents listening on IPv6 addresses.

> **Security Note:** Changing the default SSH port can reduce exposure to basic automated scans, but it is not a replacement for proper authentication, access control, firewall rules, patching, and monitoring.

---

# SSH Security Considerations

SSH provides encrypted remote access, but the SSH service should still be securely configured.

## 1. Use Strong Authentication

Use strong passwords and, where possible, use SSH key-based authentication.

## 2. Prefer SSH Keys

SSH public-key authentication can provide stronger authentication and is commonly used for administrative and server access.

## 3. Restrict User Access

Only users who require SSH access should be permitted to connect to the server.

## 4. Protect Privileged Accounts

Direct remote access using highly privileged accounts should be restricted wherever possible.

## 5. Use Firewall Controls

Restrict access to TCP port 22 to trusted networks or administrative systems where practical.

## 6. Keep OpenSSH Updated

Regularly apply security updates to Ubuntu and the OpenSSH package.

## 7. Monitor Authentication Activity

SSH authentication logs can be reviewed to identify:

* Successful login attempts
* Failed login attempts
* Repeated authentication failures
* Suspicious connection attempts
* Unauthorized access attempts

---

# Real-World Enterprise Use Cases

SSH is widely used across IT infrastructure and cybersecurity environments.

## Linux System Administration

System administrators use SSH to remotely:

* Manage Linux servers
* Install software packages
* Modify configuration files
* Restart services
* Troubleshoot system issues

## Cloud Infrastructure

SSH is commonly used to administer Linux virtual machines hosted in cloud environments.

## DevOps

SSH can support:

* Remote server administration
* Application deployment
* Git operations
* Infrastructure management
* Troubleshooting

## Cybersecurity

Security teams can use SSH for:

* Secure administrative access
* Incident response
* Remote investigation
* System hardening
* Security monitoring

## IT Support

IT support teams can use secure remote sessions to troubleshoot Linux systems without requiring physical access to the server.

---

# Practical Validation

The practical is considered successfully completed when the following conditions are verified:

| Validation           | Expected Result                        |
| -------------------- | -------------------------------------- |
| OpenSSH installation | OpenSSH Server installed successfully  |
| SSH service          | `active (running)`                     |
| SSH daemon           | `sshd` running                         |
| SSH port             | TCP port 22 listening                  |
| Server IP            | IP address successfully identified     |
| SSH connection       | Remote connection established          |
| Authentication       | Ubuntu user authenticated successfully |
| Remote commands      | Linux commands execute successfully    |
| Session termination  | SSH session exits successfully         |

---

# Key Takeaways

* SSH provides secure remote access to Linux systems.
* OpenSSH Server enables Ubuntu to accept incoming SSH connections.
* The SSH service is managed through `ssh.service`.
* The `sshd` daemon handles incoming SSH connections.
* The default SSH port is TCP 22.
* The server IP address is required to establish the SSH connection.
* SSH encrypts communication between the client and server.
* SSH allows administrators to manage Linux systems remotely.
* SSH is widely used in Linux administration, cloud computing, DevOps, IT operations, and cybersecurity.
* Secure authentication, access control, firewall restrictions, patching, and monitoring are important for protecting SSH services.

---

# 🎬 Demonstration

The practical demonstration covers the complete process of configuring and testing SSH access:

1. Start the Ubuntu 22.04 LTS virtual machine.
2. Update the Ubuntu package repository.
3. Install OpenSSH Server.
4. Verify the SSH service status.
5. Identify the Ubuntu server IP address.
6. Open an SSH client from the Windows host.
7. Connect to the Ubuntu server.
8. Authenticate using the Ubuntu user account.
9. Execute basic Linux commands remotely.
10. Exit the SSH session.

<p align="center">
  <a href="YOUR_FULL_VIDEO_LINK">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demonstration Video"/>
    <br>
    <strong>Click to Watch the Demonstration Video</strong>
  </a>
</p>

---

# Repository Structure

```text
Practical-7-Linux-Hands-On/
│
├── README.md
│
├── Images/
│   └── ssh-service-status.png
│
├── Commands/
│   └── ssh-commands.md
│
└── Resources/
    └── additional-notes.md
```

---

# Author

**Himadri Singh**

---

# License

This practical is created for educational and learning purposes.

The demonstration is intended to provide hands-on understanding of Linux administration, SSH, and secure remote access concepts.
