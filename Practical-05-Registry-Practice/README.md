# Practical 5: Windows Registry Practice

## Overview

This practical focuses on understanding the Windows Registry using the built-in Registry Editor (Regedit).

The goal of this exercise was to explore the Registry structure, identify major Registry hives, understand Registry keys and values, review Registry safety practices, and learn how the Registry is used in Windows administration and cybersecurity investigations.

All demonstrations were performed on a production Windows system. To avoid making changes to the operating system, Registry modifications were not performed. Instead, Registry navigation, backup options, search functionality, and Registry concepts were demonstrated safely.

This practical helps build foundational knowledge useful for IT Support, System Administration, SOC Operations, Digital Forensics, and Cybersecurity roles.

<p align="center">
  <img src="./Windows Registry Overview.png"
       alt="Windows Registry Practice Overview"
       width="900"/>
</p>

---

## Learning Objectives

After completing this practical, I was able to:

* Open and navigate Registry Editor (Regedit).
* Identify major Windows Registry hives.
* Understand Registry keys, subkeys, and values.
* Explore Registry structure safely without making modifications.
* Review Registry backup and search functionality.
* Understand Registry safety best practices.
* Recognize the importance of the Registry in IT administration and cybersecurity.

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

# Part 1: Windows Registry Basics

## Objective

To understand the purpose of the Windows Registry and explore the major Registry hives using Registry Editor.

## Topics Covered

* Opening Registry Editor (Regedit)
* Registry Interface
* Registry Hives
* HKEY_CLASSES_ROOT
* HKEY_CURRENT_USER
* HKEY_LOCAL_MACHINE
* Importance of the Windows Registry

## What Was Observed

Registry Editor was opened using the Run dialog box.

The Registry interface was explored and the following major Registry hives were examined:

| Registry Hive | Purpose |
|---------------|------------------------------------------------------------|
| HKEY_CLASSES_ROOT | Stores file association and object linking information |
| HKEY_CURRENT_USER | Stores settings for the currently logged-in user |
| HKEY_LOCAL_MACHINE | Stores system-wide hardware and software configuration |

## Skills Developed

* Registry Navigation
* Registry Hive Identification
* Windows Configuration Fundamentals

### Video Demonstration

YOUR_PART_1_VIDEO_LINK

---

# Part 2: Registry Structure

## Objective

To understand how Windows organizes configuration data using Registry keys, subkeys, and values.

## Topics Covered

* Registry Keys
* Registry Subkeys
* Registry Values
* Registry Data Types
* Registry Structure

## What Was Observed

The Registry structure was explored by navigating through **HKEY_CURRENT_USER → Control Panel → Desktop**.

The right pane was examined to understand how Registry values are displayed.

The following Registry components were reviewed:

| Component | Description |
|-----------|-------------------------------------------|
| Key | Main Registry container |
| Subkey | Child Registry container |
| Value | Stores configuration information |
| Data | Actual configuration setting |

## Skills Developed

* Registry Structure Analysis
* Registry Value Identification
* Windows Configuration Analysis

### Video Demonstration

YOUR_PART_2_VIDEO_LINK

---

# Part 3: Registry Safety

## Objective

To understand Registry safety practices and review backup and search features available in Registry Editor.

## Topics Covered

* Registry Export
* Registry Backup
* Registry Search
* Registry Safety
* Best Practices

## What Was Observed

The Export option in Registry Editor was demonstrated to understand how Registry backups can be created before making changes.

The built-in Find feature was also explored to locate Registry keys and values efficiently.

Since this practical was performed on a production Windows installation, no Registry modifications or backups were created.

## Skills Developed

* Registry Backup Awareness
* Registry Search
* Safe Registry Administration

### Video Demonstration

YOUR_PART_3_VIDEO_LINK

---

# Part 4: Registry in CyberSecurity

## Objective

To understand how the Windows Registry is used in IT administration and cybersecurity investigations.

## Topics Covered

* HKEY_LOCAL_MACHINE\SOFTWARE
* HKEY_CURRENT_USER\Software
* Software Configuration
* Registry Investigation
* SOC Investigation Scenario

## What Was Discussed

Software-related Registry locations were explored to understand where Windows and applications store configuration information.

A basic SOC investigation scenario was discussed to explain how Registry analysis can assist during security investigations by reviewing Registry locations for system configuration and software-related information.

No Registry entries were modified during the practical.

## Skills Developed

* Registry Investigation Fundamentals
* Windows Administration
* Cybersecurity Awareness
* SOC Investigation Concepts

### Video Demonstration

YOUR_PART_4_VIDEO_LINK

---

# Overall Practical Summary

This practical provided hands-on exposure to Windows Registry fundamentals using Registry Editor.

### Areas Covered

| Area | Description |
|----------------------|------------------------------------------------|
| Registry Editor | Exploring the Windows Registry |
| Registry Hives | Understanding major Registry hives |
| Registry Structure | Understanding keys, subkeys, and values |
| Registry Safety | Reviewing backup and search functionality |
| Registry Investigation | Understanding Registry usage in cybersecurity |
| Registry Best Practices | Safe Registry administration concepts |

By completing this practical, foundational knowledge of the Windows Registry was developed through safe observation, analysis, and guided demonstrations using built-in Windows tools.

<p align="center">
  <img src="./Windows Registry.png"
       alt="Registry Dashboard"
       width="900"/>
</p>

---

## Lab Environment

| Component | Details |
|-----------|--------------------------------------|
| Operating System | Windows 10 |
| Environment | Host Machine |
| Tool Used | Registry Editor (Regedit) |

---

## Tools Used

| Tool | Purpose |
|-------------------------|-----------------------------------------------|
| Registry Editor (Regedit) | View and explore the Windows Registry |
| Run Dialog | Launch Registry Editor |
| Windows Operating System | Platform used for the practical |

---

## Key Takeaways

* Windows Registry is the central configuration database of Windows.
* Registry Editor allows administrators to safely explore Registry information.
* Registry data is organized into hives, keys, subkeys, and values.
* Registry backups should always be considered before making modifications.
* The Registry plays an important role in Windows administration and cybersecurity investigations.
* Understanding Registry structure is essential for troubleshooting and system analysis.

---

## Repository Structure

```text
Practical-05-Windows-Registry/
│
├── README.md
├── Windows Registry Overview.png
├── Windows Registry.png
```

---

## Author

**Himadri Singh**

---

## License

This practical is created for educational and learning purposes.
