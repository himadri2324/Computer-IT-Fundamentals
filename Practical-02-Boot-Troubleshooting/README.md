# Practical 2: Boot Troubleshooting

## Overview

This practical focuses on understanding the Windows boot process and learning how startup-related issues can be diagnosed using built-in Windows troubleshooting and recovery tools.

During this practical, I explored startup applications, reviewed system startup events using Event Viewer, accessed the Windows Recovery Environment (WinRE), booted into Safe Mode, and examined Startup Repair options available in Windows.

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-02-Boot-Troubleshooting/Boot%20Troubleshooting%20Infographics.png"
       alt="Boot Troubleshooting Infographics"
       width="900"/>
</p>

---

## Learning Objectives

After completing this practical, I was able to:

* Understand the basic Windows startup process.
* Identify common startup and boot-related issues.
* Review startup applications that may affect boot performance.
* Analyze startup-related events using Event Viewer.
* Access and navigate Windows Recovery Environment (WinRE).
* Explore Safe Mode and its troubleshooting purpose.
* Understand how Startup Repair is used to resolve startup problems.
* Apply a structured troubleshooting approach used in IT support environments.

---

## 🎬 Demonstration
<p align="center">
  <a href="https://www.youtube.com/watch?v=hV8pe57Sy8M" target="_blank">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo" />
    <br>
    <strong>Click to watch the demonstration video</strong>
  </a>
</p>

---

# Part 1: Understanding the Windows Boot Process

## Objective

To understand how Windows starts, identify common startup issues, and explore tools that help investigate startup-related problems.

## Topics Covered

| Topic                | Description                                     |
| -------------------- | ----------------------------------------------- |
| Windows Boot Process | Overview of how Windows starts                  |
| Startup Applications | Programs configured to launch at startup        |
| Event Viewer         | Reviewing startup-related logs                  |
| Common Boot Issues   | Typical startup problems encountered in Windows |

### Startup Applications Analysis

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-02-Boot-Troubleshooting/Startup%20Apps%20Analysis.png"
       alt="Startup Apps Analysis"
       width="900"/>
</p>

### Event Viewer Analysis

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-02-Boot-Troubleshooting/Event%20Viewer%20Analysis.png"
       alt="Event Viewer Analysis"
       width="900"/>
</p>

## What I Did

* Opened Task Manager and reviewed Startup Apps.
* Examined applications configured to run during startup.
* Opened Event Viewer and navigated to Windows Logs → System.
* Reviewed informational, warning, and error events related to system startup.
* Observed how Event Viewer can be used to investigate startup-related issues.

## Skills Gained

* Startup Application Analysis
* Event Log Investigation
* Basic Troubleshooting Methodology

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=1KqUqRt0vxU

---

# Part 2: Windows Recovery Environment (WinRE)

## Objective

To access Windows Recovery Environment and explore the recovery options available for startup troubleshooting.

## Topics Covered

| Tool / Option    | Purpose                    |
| ---------------- | -------------------------- |
| Troubleshoot     | Access recovery tools      |
| Startup Settings | Configure startup behavior |
| Command Prompt   | Advanced troubleshooting   |
| System Restore   | Restore system state       |
| Startup Repair   | Repair startup issues      |

### WinRE Main Menu

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-02-Boot-Troubleshooting/WinRE%20Main%20Menu.png"
       alt="Windows Recovery Environment Main Menu"
       width="900"/>
</p>

### Advanced Recovery Options

<p align="center">
  <img src="https://github.com/himadri2324/Computer-IT-Fundamentals/blob/main/Practical-02-Boot-Troubleshooting/WinRE%20Advanced%20Options.png"
       alt="Windows Recovery Environment Advanced Options"
       width="900"/>
</p>

## What I Did

* Accessed Windows Recovery Environment.
* Explored the "Choose an Option" screen.
* Navigated through Advanced Options.
* Reviewed available recovery and troubleshooting tools.
* Examined Startup Settings and Startup Repair options.

## Skills Gained

* Recovery Environment Navigation
* Windows Recovery Fundamentals
* Startup Troubleshooting Awareness

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=r2iXtMtaI9o

---

# Part 3: Safe Mode Troubleshooting

## Objective

To understand the purpose of Safe Mode and how it assists in troubleshooting startup-related problems.

## Topics Covered

* Safe Mode
* Startup Diagnostics
* Driver Troubleshooting
* Software Conflict Isolation

## What I Did

* Accessed Startup Settings through WinRE.
* Reviewed Safe Mode startup options.
* Explored how Safe Mode loads Windows with minimal drivers and services.
* Discussed situations where Safe Mode can be used during troubleshooting.

## Skills Gained

* Safe Mode Navigation
* Driver Troubleshooting Concepts
* Software Conflict Investigation

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=NhbmJymmFmk

---

# Part 4: Startup Repair & Recovery Tools

## Objective

To understand the purpose of Startup Repair and review how Windows recovery tools can assist in resolving startup problems.

## Topics Covered

* Startup Repair
* Recovery Options
* Startup Diagnostics
* Windows Recovery Tools

## What I Did

* Explored Startup Repair from the Advanced Options menu.
* Reviewed how Startup Repair checks for startup-related issues.
* Examined the role of Startup Repair in recovering Windows startup functionality.
* Discussed when Startup Repair should be used during troubleshooting.

## Skills Gained

* Startup Repair Awareness
* Recovery Tool Familiarity
* Windows Startup Troubleshooting Concepts

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=5S9nVxuuLvY

---

# Overall Practical Summary

This practical provided hands-on exposure to Windows startup troubleshooting tools and recovery options.

### Areas Covered

| Area                 | Tool / Method  |
| -------------------- | -------------- |
| Startup Analysis     | Task Manager   |
| Log Analysis         | Event Viewer   |
| Recovery Environment | WinRE          |
| Startup Diagnostics  | Safe Mode      |
| Recovery Tools       | Startup Repair |

Through this practical, I gained a better understanding of how Windows startup issues can be investigated and how built-in recovery tools support troubleshooting in real-world IT support scenarios.

---

# Tools Used

| Tool                                 | Purpose                       |
| ------------------------------------ | ----------------------------- |
| Task Manager                         | Analyze startup applications  |
| Event Viewer                         | Review startup-related events |
| Windows Recovery Environment (WinRE) | Access recovery tools         |
| Safe Mode                            | Troubleshoot startup issues   |
| Startup Repair                       | Diagnose startup problems     |
| Windows OS                           | Practical environment         |

---

# Key Takeaways

* Startup applications can affect system startup performance.
* Event Viewer provides useful information for troubleshooting startup issues.
* WinRE offers several recovery and troubleshooting tools.
* Safe Mode helps isolate software and driver-related problems.
* Startup Repair is one of the primary recovery options for startup failures.
* A structured troubleshooting approach is important in IT support.

---

# Repository Structure

```text
Practical-02-Boot-Troubleshooting/
│
├── README.md
├── Boot Troubleshooting Infographics.png
├── Startup Apps Analysis.png
├── Event Viewer Analysis.png
├── WinRE Main Menu.png
├── WinRE Advanced Options.png
```

---

# Author

**Himadri Singh**

---

# License

This practical is intended for educational and learning purposes only.
