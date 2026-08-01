# Practical 9: Linux Log Analysis

## Overview

Linux systems generate log files that record system activities, user authentication, service events, and security-related information. These logs are essential for troubleshooting, monitoring system health, and investigating security incidents.

In this practical, you will explore the Linux authentication log (`/var/log/auth.log`) and learn how to analyze login attempts, SSH connections, and sudo activities using common Linux commands. This hands-on exercise introduces the fundamentals of log analysis used by Linux administrators and SOC (Security Operations Center) analysts.

<p align="center">
  <img src=""
       alt="Linux Log Analysis"
       width="900"/>
</p>

---

## Learning Objectives

After completing this practical, you will be able to:

- Understand the purpose of Linux log files.
- Navigate to the `/var/log` directory.
- Read authentication logs using Linux commands.
- Analyze successful and failed login attempts.
- Monitor SSH authentication events.
- Track sudo (privileged) activities.
- Use log analysis techniques for basic security investigations.

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

### Areas Covered

| Area | Description |
|-------------------------|------------------------------------------------------------|
| Linux Logging | Understanding the purpose of system log files |
| `/var/log` Directory | Exploring the default Linux log storage location |
| Authentication Logs | Reading `/var/log/auth.log` |
| Log Reading Commands | Using `cat`, `less`, `head`, and `tail` |
| Log Filtering | Searching log entries with `grep` |
| SSH Monitoring | Identifying successful and failed SSH logins |
| Sudo Monitoring | Tracking privileged command execution |
| Real-Time Monitoring | Watching new log entries using `tail -f` |
| Security Investigation | Performing basic authentication log analysis |

---

## Lab Environment

| Component | Details |
|-----------|---------|
| Operating System | Ubuntu Linux |
| Virtualization Platform | VMware Workstation |
| User Privileges | Standard User with Sudo Access |
| Log File | `/var/log/auth.log` |
| Terminal | Ubuntu Terminal |

---

## Tools Used

| Tool | Purpose |
|------|---------|
| Ubuntu Terminal | Execute Linux commands |
| VMware Workstation | Virtual machine environment |
| cat | Display complete log file |
| less | Read large log files page by page |
| head | Display the beginning of a log file |
| tail | Display the latest log entries |
| grep | Search specific log entries |
| sudo | Execute administrative commands |

---

## Key Takeaways

- Linux stores important system and authentication logs inside the `/var/log` directory.
- The `auth.log` file records authentication-related events such as logins, SSH access, and sudo activities.
- Commands like `cat`, `less`, `head`, `tail`, and `grep` help efficiently analyze log files.
- Failed login attempts can indicate brute-force attacks or unauthorized access attempts.
- Successful authentication events help verify legitimate user access.
- Sudo logs provide accountability for administrative actions.
- Real-time log monitoring is useful during system administration and incident response.
- Log analysis is a fundamental skill for Linux administrators, SOC analysts, and cybersecurity professionals.

---

## Repository Structure

```
Practical-9-Linux-Log-Analysis/
│
├── README.md
├── Images/
│   ├── overview.png
│   ├── auth-log.png
│   ├── grep-search.png
│   └── tail-follow.png
│
└── Commands/
    └── linux-log-analysis-commands.txt
```

---

## Author

**Himadri Singh**

---
## License

This practical is created for educational and learning purposes.
