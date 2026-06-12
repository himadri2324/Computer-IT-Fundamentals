# Practical 3: Disk Management & Storage Handling in Windows

## Overview

This practical focuses on understanding how Windows manages storage using the built-in Disk Management utility.

The goal of this exercise was to explore the storage layout of a Windows system, identify different partitions, review disk and volume properties, understand how partition creation works, and learn basic storage management practices used in real-world environments.

All demonstrations were performed on a production Windows system. To avoid making changes to the operating system, potentially destructive operations such as partition creation and drive formatting were explained conceptually rather than executed.

This practical helps build foundational knowledge useful for IT Support, System Administration, SOC Operations, and Cybersecurity roles.

<p align="center">
  <img src="./Disk management overview.png"
       alt="Disk Management Overview"
       width="900"/>
</p>

---

## Learning Objectives

After completing this practical, I was able to:

* Navigate and use the Windows Disk Management utility.
* Identify system partitions and understand their purpose.
* Review disk and volume properties.
* Understand storage capacity and utilization information.
* Explain the partition creation workflow.
* Understand common Windows file systems.
* Apply basic storage management best practices.

---

## 🎬 Demonstration
<p align="center">
  <a href="https://www.youtube.com/watch?v=fbbW4tLs5QU" target="_blank">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo" />
    <br>
    <strong>Click to watch the demonstration video</strong>
  </a>
</p>

---

# Part 1: Introduction to Disk Management & Partitions

## Objective

To explore the Windows Disk Management utility and identify the partitions present on the system.

## Topics Covered

* Opening Disk Management
* Understanding Disk 0
* EFI System Partition
* Windows (C:) Partition
* Recovery Partition
* Storage Layout Overview

## What Was Observed

The system contained a single physical disk identified as Disk 0.

Three partitions were visible:

| Partition              | Purpose                                                     |
| ---------------------- | ----------------------------------------------------------- |
| EFI System Partition   | Stores boot files required to start Windows                 |
| Windows (C:) Partition | Contains the operating system, applications, and user data  |
| Recovery Partition     | Contains recovery tools used for troubleshooting and repair |

## Skills Developed

* Disk Identification
* Partition Recognition
* Windows Storage Fundamentals

### Video Demonstration

https://www.youtube.com/watch?v=4Me-YwBQeNc

---

# Part 2: Disk Properties & Storage Information

## Objective

To examine storage information and understand how Windows reports disk and volume details.

## Topics Covered

* Drive Properties
* Used Space
* Free Space
* Capacity Information
* NTFS File System
* Disk Properties
* Volume Information

## What Was Observed

The Windows (C:) drive properties were examined to review storage utilization.

The following information was reviewed:

| Property    | Description                |
| ----------- | -------------------------- |
| Capacity    | Total size of the volume   |
| Used Space  | Storage currently occupied |
| Free Space  | Available storage          |
| File System | NTFS                       |

Disk properties were also reviewed to examine storage configuration and volume information.

## Skills Developed

* Storage Capacity Analysis
* File System Identification
* Storage Information Review

### Video Demonstration

https://www.youtube.com/watch?v=B3-iT5qsO8o

---

# Part 3: Partition Creation Workflow

## Objective

To understand how new partitions can be created using Disk Management.

## Topics Covered

* Shrink Volume
* Unallocated Space
* New Simple Volume
* Drive Letter Assignment
* Volume Creation Workflow

## What Was Demonstrated

Since this practical was performed on a production Windows installation, no actual partitions were created.

Instead, the partition creation workflow was reviewed by opening the Shrink Volume option and examining the process used by Windows to calculate available shrink space.

The following workflow was discussed:

1. Shrink an existing volume.
2. Create unallocated space.
3. Create a New Simple Volume.
4. Assign a drive letter.
5. Format the volume.

## Skills Developed

* Partition Planning
* Storage Allocation Concepts
* Volume Management Fundamentals

### Video Demonstration

https://www.youtube.com/watch?v=VhFSs1UApEk

---

# Part 4: Drive Formatting & Storage Management Best Practices

## Objective

To understand formatting concepts and review storage management practices commonly used in enterprise environments.

## Topics Covered

* Drive Formatting
* NTFS
* FAT32
* exFAT
* Storage Capacity Monitoring
* Backup Practices
* Disk Usage Monitoring

## What Was Discussed

Formatting was discussed conceptually without performing any formatting operations.

The following file systems were reviewed:

| File System | Common Usage                                 |
| ----------- | -------------------------------------------- |
| NTFS        | Default Windows file system                  |
| FAT32       | Compatibility with older systems and devices |
| exFAT       | External drives and removable media          |

Storage utilization was also reviewed through File Explorer to examine available and used storage space.

## Storage Management Best Practices

* Monitor disk usage regularly.
* Maintain sufficient free space.
* Perform regular backups.
* Monitor storage device health.
* Review storage utilization periodically.

## Skills Developed

* Storage Administration Fundamentals
* File System Awareness
* Capacity Monitoring
* Storage Best Practices

### Video Demonstration

https://www.youtube.com/watch?v=wNVgkByetl0

---

# Overall Practical Summary

This practical provided hands-on exposure to Windows Disk Management and basic storage administration concepts.

### Areas Covered

| Area                | Description                                                      |
| ------------------- | ---------------------------------------------------------------- |
| Disk Management     | Exploring storage devices and partitions                         |
| Partition Analysis  | Understanding EFI, Windows, and Recovery partitions              |
| Storage Information | Reviewing capacity, free space, and file system details          |
| Partition Workflow  | Understanding the process of creating new volumes                |
| Formatting Concepts | Learning how formatting works and when it is used                |
| Storage Management  | Reviewing best practices for maintaining healthy storage systems |

By completing this practical, foundational knowledge of Windows storage management was developed through observation, analysis, and guided demonstrations using built-in Windows tools.

<p align="center">
  <img src="./Disk Management.png"
       alt="Disk Management"
       width="900"/>
</p>

---

## Tools Used

| Tool                     | Purpose                                           |
| ------------------------ | ------------------------------------------------- |
| Disk Management          | View disks, partitions, and storage configuration |
| File Explorer            | Review storage utilization and drive properties   |
| Windows Operating System | Platform used for the practical                   |

---

## Key Takeaways

* Disk Management is the primary Windows utility for storage administration.
* Understanding partition structure is important for troubleshooting and system maintenance.
* Storage capacity should be monitored regularly to avoid performance issues.
* NTFS is the default file system used by modern Windows systems.
* Partition creation involves shrinking an existing volume and allocating new space.
* Formatting should only be performed after verifying backups and understanding data impact.

---

## Repository Structure

```text
Practical-03-Disk-Management/
│
├── README.md
├── Disk management overview.png
├── Disk Management.png
```

---

## Author

**Himadri Singh**

---

## License

This practical is created for educational and learning purposes.
