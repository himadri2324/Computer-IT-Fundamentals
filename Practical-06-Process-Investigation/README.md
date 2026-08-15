# Practical 6: Process Investigation

## Overview

Process Investigation is a fundamental Windows administration and cybersecurity skill used to understand what is running on a system and identify processes that may require further investigation.

In this practical, I demonstrated how to safely investigate Windows processes using **Windows Task Manager** and **Microsoft Process Explorer**. The practical focuses on understanding running processes, analyzing system resource usage, examining process properties, verifying digital signatures, using VirusTotal integration, and learning the basic indicators considered during process investigations.

This practical was performed on a **host Windows machine** in an observation-only manner without making any system changes.

<p align="center">
  <img src="images/process-investigation-overview.png"
       alt="Process Investigation Overview"
       width="900"/>
</p>

---

# Learning Objectives

After completing this practical, you will be able to:

- Understand what a Windows process is
- Explain why process investigation is important
- Navigate Windows Task Manager
- Monitor CPU, Memory, Disk, and Network usage
- Understand Process IDs (PID)
- Examine executable locations
- Use Search Online for initial process research
- Use Microsoft Process Explorer
- Understand parent-child process relationships
- Verify digital signatures
- Use VirusTotal integration
- Recognize basic indicators of suspicious processes

---

# 🎬 Demonstration

<p align="center">
  <a href="https://www.youtube.com/watch?v=aR6UipUg2_s">
    <img src="https://img.icons8.com/color/96/video.png"
         alt="Watch Demo"/>
    <br>
    <strong>Watch Full Practical on YouTube</strong>
  </a>
</p>

---

# Part 1: Introduction

## Objective

Understand Windows processes and why process investigation is an important troubleshooting and cybersecurity skill.

## Topics Covered

- Introduction to Process Investigation
- What is a Windows process
- Why process investigation matters
- Windows Task Manager overview
- Applications, Background Processes, and Windows Processes
- Demonstration using Notepad

## Practical Demonstration

Task Manager was used to observe running applications and processes. Notepad was opened and its associated process was observed in Task Manager.

<p align="center">
  <img src="images/task-manager-notepad.png"
       alt="Task Manager with Notepad Process"
       width="900"/>
</p>

### What Was Observed

- Running applications appear as processes in Task Manager
- Notepad appears as a running process while the application is open
- Closing an application can result in its associated process ending
- Windows displays applications and background processes separately in Task Manager

## Skills Developed

- Understanding Windows processes
- Basic Task Manager navigation
- Identifying running applications
- Observing process creation and termination

### Video Demonstration

https://www.youtube.com/watch?v=2-_y56S3Ewo

---

# Part 2: Investigating Running Processes Using Task Manager

## Objective

Learn how to investigate running processes using Windows Task Manager and examine system resource usage.

## Topics Covered

- CPU usage
- Memory usage
- Disk usage
- Network usage
- Process ID (PID)
- Open File Location
- Search Online

## Practical Demonstration

Windows Task Manager was used to review running processes and observe CPU, Memory, Disk, and Network resource usage.

<p align="center">
  <img src="images/task-manager-processes.png"
       alt="Windows Task Manager Processes"
       width="900"/>
</p>

### What Was Observed

- Task Manager displays currently running applications and background processes
- CPU, Memory, Disk, and Network usage can be monitored
- Processes can be reviewed based on their resource consumption
- Each running process is assigned a Process ID (PID)
- Executable location can provide useful investigation context
- Search Online can provide an initial reference for unfamiliar processes
- Resource usage alone cannot determine whether a process is malicious

## Skills Developed

- Performance monitoring
- Resource analysis
- Process identification
- Basic process investigation

### Video Demonstration

https://www.youtube.com/watch?v=QOXnGqLFaEU

---

# Part 3: Process Explorer

## Objective

Perform deeper process analysis using **Microsoft Process Explorer**.

## Topics Covered

- Process Explorer
- Process tree
- Parent-child relationships
- Process properties
- Image information
- Performance information
- Verify Image Signatures
- VirusTotal integration

## Practical Demonstration

Microsoft Process Explorer was used to examine running processes and obtain additional process information.

<p align="center">
  <img src="images/process-explorer.png"
       alt="Microsoft Process Explorer"
       width="900"/>
</p>

### What Was Observed

- Process Explorer provides a detailed view of running processes
- Parent-child relationships provide additional investigation context
- Process properties contain additional executable information
- Process Explorer can display publisher information
- Digital signature verification can help verify software publisher information
- VirusTotal integration provides additional file reputation information

## Skills Developed

- Advanced Windows process analysis
- Process hierarchy investigation
- Process property inspection
- Digital signature verification
- Reputation-based analysis

### Video Demonstration

https://www.youtube.com/watch?v=QgaATRIT6q8

---

# Part 4: Malware Detection Basics

## Objective

Understand the basic indicators considered when investigating potentially suspicious processes.

## Topics Covered

- Executable location
- Digital signature
- VirusTotal reputation
- Resource usage
- Process names
- Parent-child process behavior
- Suspicious process indicators
- Evidence-based investigation

## Investigation Scenario

A user reports that their Windows computer has suddenly become slow and the cooling fan is running continuously.

The investigation approach discussed in this practical is:

1. Identify processes using system resources
2. Examine the process name and behavior
3. Check the executable location
4. Inspect process properties
5. Verify the digital signature
6. Review VirusTotal reputation
7. Consider multiple indicators before reaching a conclusion

### What Was Observed

- Legitimate software should be evaluated using multiple indicators
- Chrome was discussed as an example of a legitimate process
- An unusual process should be investigated rather than immediately classified as malware
- High resource usage alone does not confirm malicious activity
- A suspicious indicator does not automatically mean that a process is malware
- Professional investigations rely on multiple sources of evidence before reaching a conclusion

## Skills Developed

- Basic malware investigation concepts
- Evidence-based analysis
- Process validation
- Analytical thinking
- Suspicious process identification

### Video Demonstration

https://www.youtube.com/watch?v=fDgn-be6rJg

---

# Overall Practical Summary

This practical introduced the fundamentals of Windows process investigation using **Task Manager** and **Microsoft Process Explorer**.

The practical demonstrated how to inspect running processes, analyze system resource usage, examine process information, understand process relationships, verify digital signatures, use VirusTotal integration, and recognize basic indicators that may require further investigation.

The practical also emphasized that **no single indicator confirms malware** and that professional investigations should consider multiple sources of evidence and context before reaching a conclusion.

---

# Areas Covered

| Area | Description |
|------|-------------|
| Windows Processes | Understanding running processes |
| Task Manager | Process monitoring and resource analysis |
| CPU / Memory / Disk / Network | Monitoring process resource usage |
| PID | Process identification |
| File Location | Examining executable location |
| Process Explorer | Advanced process analysis |
| Parent-Child Processes | Understanding process relationships |
| Digital Signatures | Verifying software publisher information |
| VirusTotal | File reputation lookup |
| Malware Detection | Basic process investigation methodology |

---

# Lab Environment

| Component | Details |
|-----------|---------|
| Operating System | Microsoft Windows |
| Environment | Host Machine |
| Practical Type | Observation and Analysis |
| Internet Connection | Required for VirusTotal lookup |

---

# Tools Used

- Windows Task Manager
- Microsoft Process Explorer
- Microsoft Sysinternals
- VirusTotal Integration

---

# Key Takeaways

- Windows uses processes to execute running applications and system components.
- Task Manager provides an overview of running processes and resource usage.
- Process Explorer provides deeper visibility into Windows processes.
- Process IDs (PIDs) help identify individual running processes.
- Executable locations provide useful context during process investigation.
- Parent-child relationships help analysts understand process execution.
- Digital signatures help verify software publisher information.
- VirusTotal provides additional file reputation information.
- High resource usage does not automatically indicate malware.
- No single indicator confirms malicious activity.
- Professional investigations rely on multiple pieces of evidence and context.

---

# Repository Structure

```text
Practical-6-Process-Investigation/
│
├── README.md
│
└── images/
    ├── process-investigation-overview.png
    ├── task-manager-notepad.png
    ├── task-manager-processes.png
    └── process-explorer.png
```

---

# Author

**Himadri Singh**

---

# License

This practical is created for educational and learning purposes.
