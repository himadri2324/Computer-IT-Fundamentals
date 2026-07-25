# Practical 6: Process Investigation

## Overview

Process Investigation is a fundamental Windows administration and cybersecurity skill used to understand what is running on a system and identify processes that may require further investigation.

In this practical, I demonstrated how to safely investigate Windows processes using **Task Manager** and **Microsoft Process Explorer**. The practical focuses on understanding running processes, analyzing system resource usage, examining process properties, verifying digital signatures, using VirusTotal integration, and learning the basic indicators that security professionals consider during process investigations.

This practical was performed on a host Windows machine in an observation-only manner without making any system changes.

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
- Monitor CPU, Memory, Disk and Network usage
- Understand Process IDs (PID)
- Verify executable locations
- Use Search Online for initial process research
- Use Microsoft Process Explorer
- Understand parent-child process relationships
- Verify digital signatures
- Use VirusTotal integration
- Recognize basic indicators of suspicious processes

---

# 🎬 Demonstration

<p align="center">
  <a href="YOUR_FULL_VIDEO_LINK">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo"/>
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
- Applications vs Background Processes vs Windows Processes
- Demonstration using Notepad

## What Was Observed

- Running applications appear as processes in Task Manager
- Chrome uses multiple processes due to its multi-process architecture
- A process exists only while its associated program is running
- Windows separates user applications, background processes and system processes

## Skills Developed

- Understanding Windows processes
- Basic Task Manager navigation
- Identifying running applications
- Observing process creation and termination

### Video Demonstration

YOUR_PART_1_VIDEO_LINK

---

# Part 2: Investigating Running Processes Using Task Manager

## Objective

Learn how to investigate running processes using Windows Task Manager.

## Topics Covered

- CPU usage
- Memory usage
- Disk usage
- Network usage
- Process ID (PID)
- Open File Location
- Search Online

## What Was Observed

- Resource usage can be sorted to identify active processes
- Every process has a unique PID
- Executable location helps during investigations
- Search Online provides an initial reference for unknown processes
- Resource usage alone cannot determine whether a process is malicious

## Skills Developed

- Performance monitoring
- Resource analysis
- Process identification
- Basic process investigation

### Video Demonstration

YOUR_PART_2_VIDEO_LINK

---

# Part 3: Process Explorer

## Objective

Perform deeper process analysis using Microsoft Process Explorer.

## Topics Covered

- Installing Process Explorer
- Process tree
- Parent-child relationships
- Process properties
- Image tab
- Performance tab
- Verify Image Signatures
- VirusTotal Integration

## What Was Observed

- Parent-child relationships provide additional investigation context
- Process properties contain detailed executable information
- Digital signatures help verify software publishers
- VirusTotal checks file reputation using its cryptographic hash

## Skills Developed

- Advanced Windows process analysis
- Process hierarchy investigation
- Signature verification
- Reputation-based analysis

### Video Demonstration

YOUR_PART_3_VIDEO_LINK

---

# Part 4: Malware Detection Basics

## Objective

Understand the basic indicators analysts use during process investigations.

## Topics Covered

- Executable location
- Digital signature
- VirusTotal reputation
- Resource usage
- Suspicious process indicators
- Investigation methodology

## What Was Observed

- Legitimate software should be evaluated using multiple indicators
- Chrome was demonstrated as an example of a legitimate process
- Analysts avoid conclusions based on a single indicator
- Process investigation combines technical evidence before making decisions

## Skills Developed

- Basic malware investigation concepts
- Evidence-based analysis
- Process validation
- Analytical thinking

### Video Demonstration

YOUR_PART_4_VIDEO_LINK

---

# Overall Practical Summary

This practical introduced the fundamentals of Windows process investigation using Task Manager and Microsoft Process Explorer. It demonstrated how to inspect running processes, analyze system resource usage, verify executable information, understand process relationships, validate digital signatures, and use VirusTotal integration. The practical concluded by explaining how security professionals evaluate multiple indicators before determining whether a process requires further investigation.

### Areas Covered

| Area | Description |
|------|-------------|
| Windows Processes | Understanding running processes |
| Task Manager | Process monitoring and resource analysis |
| PID | Process identification |
| File Location | Executable verification |
| Process Explorer | Advanced process analysis |
| Parent-Child Processes | Process relationship analysis |
| Digital Signatures | Publisher verification |
| VirusTotal | File reputation lookup |
| Malware Detection | Basic investigation methodology |

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
- Microsoft Sysinternals Suite
- VirusTotal Integration

---

# Key Takeaways

- Every running application is represented by one or more Windows processes.
- Task Manager provides an overview of running applications and system resource usage.
- Process Explorer offers deeper visibility than Task Manager.
- Digital signatures help verify software publishers.
- VirusTotal provides file reputation information.
- High resource usage alone does not indicate malware.
- No single indicator confirms malicious activity.
- Professional investigations rely on multiple pieces of evidence before reaching a conclusion.

---

# Repository Structure

```
Practical-6-Process-Investigation/
│
├── README.md
├── images/
│   ├── process-investigation-overview.png
│   ├── task-manager.png
│   ├── process-explorer.png
│   └── investigation-workflow.png
│
├── videos/
│   ├── Part-1.md
│   ├── Part-2.md
│   ├── Part-3.md
│   └── Part-4.md
│
└── resources/
    └── references.md
```

---

# Author

**Himadri Singh**

---

# License

This practical is created for educational and learning purposes.
