# Practical 9: Linux Log Analysis

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-09-Linux-Log-Analysis/Linux%20Log%20Analysis.png"
       alt="Linux Log Analysis"
       width="900"/>
</p>

<p align="center">

![Linux](https://img.shields.io/badge/Linux-Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Shell](https://img.shields.io/badge/Shell-Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![VMware](https://img.shields.io/badge/VMware-Workstation-607078?style=for-the-badge&logo=vmware&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Log%20Analysis-blue?style=for-the-badge)

</p>

---

# Overview

Linux records almost every important system activity inside log files. These logs provide valuable information about authentication events, user activities, system services, SSH connections, and administrative actions. They play a crucial role in system administration, troubleshooting, compliance auditing, and cybersecurity investigations.

In this practical, we perform a hands-on analysis of the Linux authentication log (`/var/log/auth.log`). Using standard Linux commands, we examine login events, monitor privileged activities, search authentication records, and understand how security analysts investigate incidents using log data.

This practical is designed for beginners in Linux, System Administration, IT Support, and Cybersecurity.

---

# Learning Objectives

After completing this practical, you will be able to:

- Understand what Linux log files are.
- Explain why system logs are important.
- Navigate to the `/var/log` directory.
- Identify common Linux log files.
- Read authentication logs using Linux commands.
- Search specific events using `grep`.
- Analyze failed login attempts.
- Verify successful authentication events.
- Monitor sudo activities.
- Perform basic authentication log investigations.
- Understand how log analysis supports Security Operations Centers (SOC).

---

# 🎬 Demonstration

<p align="center">
  <a href="https://www.youtube.com/watch?v=ENOPQDy9idI">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo"/>
    <br>
    <strong>Watch Complete Practical Demonstration</strong>
  </a>
</p>

---

# Practical Workflow

```
Understand Linux Logs
          │
          ▼
Navigate to /var/log
          │
          ▼
Explore auth.log
          │
          ▼
Read Log File
(cat, less, head, tail)
          │
          ▼
Search Authentication Events
(grep)
          │
          ▼
Monitor Sudo Activities
          │
          ▼
Real-Time Log Monitoring
          │
          ▼
Security Investigation
```

---

# Areas Covered

| Area | Description |
|-------------------------|--------------------------------------------------------------|
| Linux Logging | Understanding Linux logging architecture |
| /var/log | Exploring the system log directory |
| Authentication Logs | Reading authentication-related events |
| Log Reading | Viewing log files using Linux commands |
| Searching Logs | Filtering logs using grep |
| SSH Monitoring | Identifying login attempts |
| Sudo Monitoring | Tracking privileged command execution |
| Live Monitoring | Monitoring logs using tail -f |
| Security Investigation | Basic incident investigation workflow |

---

# Lab Environment

| Component | Details |
|------------|--------------------------------|
| Operating System | Ubuntu Linux |
| Virtualization Platform | VMware Workstation |
| User Account | Standard User with Sudo Privileges |
| Terminal | Ubuntu Terminal |
| Log File | `/var/log/auth.log` |

---

# Commands Demonstrated

| Command | Purpose |
|----------|--------------------------------|
| `pwd` | Display current directory |
| `whoami` | Show logged-in user |
| `cd /var/log` | Navigate to log directory |
| `ls` | List available log files |
| `cat auth.log` | Display entire log file |
| `less auth.log` | Read large log files |
| `head auth.log` | View first lines |
| `tail auth.log` | View latest log entries |
| `grep "Failed password"` | Search failed logins |
| `grep "Accepted password"` | Search successful logins |
| `grep sudo` | Search sudo activities |
| `tail -f auth.log` | Live log monitoring |

---

# Common Linux Log Files

| Log File | Purpose |
|----------------------|--------------------------------|
| `/var/log/auth.log` | Authentication events |
| `/var/log/syslog` | General system logs |
| `/var/log/kern.log` | Kernel messages |
| `/var/log/dpkg.log` | Package installation logs |
| `/var/log/boot.log` | Boot process logs |

---

# Screenshots

## Authentication Log

<p align="center">
<img src="Images/auth-log.png" width="900">
</p>

---

## Monitoring tail Activities

<p align="center">
<img src="Images/sudo-log.png" width="900">
</p>

---

## Monitoring Sudo Activities

<p align="center">
<img src="Images/sudo-log.png" width="900">
</p>

---

# Real-World Scenario

Imagine you are working as a SOC Analyst.

An organization reports multiple failed SSH login attempts on a production Linux server.

Instead of guessing what happened, you:

- Open the authentication log.
- Search for failed login attempts.
- Verify successful logins.
- Review sudo activities.
- Determine whether the activity is suspicious.
- Escalate the incident if unauthorized access is detected.

This is one of the most common investigation workflows performed by Security Operations Center (SOC) analysts.

---

# Best Practices

- Regularly review authentication logs.
- Investigate repeated failed login attempts.
- Monitor privileged user activities.
- Restrict unnecessary sudo access.
- Archive old logs for compliance.
- Protect log files from unauthorized modification.
- Monitor logs continuously in production environments.

---

# Key Takeaways

- Linux stores important logs inside the `/var/log` directory.
- Authentication events are commonly recorded in `auth.log`.
- Commands like `cat`, `less`, `head`, `tail`, and `grep` simplify log analysis.
- Failed login attempts may indicate brute-force attacks.
- Successful authentication confirms valid access.
- Sudo logs provide accountability for privileged actions.
- Real-time monitoring helps detect suspicious activities quickly.
- Log analysis is a foundational skill for Linux administrators and cybersecurity professionals.

---

# Repository Structure

```

Practical-9-Linux-Log-Analysis/
│
├── README.md
│
├── Images/
│   ├── banner.png
│   ├── linux-log-analysis-overview.png
│   ├── authentication-log.png
│   ├── tail-auth-log.png
│   ├── grep-sudo-log.png
│   ├── terminal-overview.png
│   └── commands-summary.png
│
├── Commands/
│   └── linux-log-analysis-commands.txt
│
├── Slides/
│   └── Practical-9-Linux-Log-Analysis.pdf
│
└── LICENSE

```

---

# Skills Gained

- Linux Fundamentals
- Linux Administration
- Authentication Log Analysis
- Command Line Navigation
- Bash Commands
- Security Monitoring
- Incident Investigation
- SOC Fundamentals
- Blue Team Basics

---

# Author

**Himadri Singh**

Cybersecurity Enthusiast | Linux Learner | SOC Analyst Aspirant

---

# License

This project is created for educational and learning purposes.

Feel free to use it for study, practice, and academic learning.
