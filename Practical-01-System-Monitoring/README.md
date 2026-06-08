# Practical 1: System Monitoring & Performance Analysis in Windows

## Overview

This practical focuses on understanding how Windows utilizes system resources in real time using **Task Manager** and **Resource Monitor**.

The objective was to observe active processes, monitor CPU, memory, and disk usage, and understand how Windows presents performance-related information. This exercise provides a foundation for troubleshooting and performance analysis, which are important skills in IT Support, System Administration, SOC Operations, and Cybersecurity.

<p align="center">
  <img src="./System monitoring infographic.png"
       alt="System Monitoring Infographic"
       width="900"/>
</p>

---

# Learning Objectives

After completing this practical, I was able to:

* Navigate different sections of Windows Task Manager.
* Identify running applications and background processes.
* Monitor CPU utilization in real time.
* Analyze memory usage and available RAM.
* Observe disk activity and storage performance metrics.
* Use Resource Monitor for more detailed system analysis.
* Understand how system resources are consumed by processes and services.

---

## 🎬 Demonstration
<p align="center">
  <a href="https://www.youtube.com/watch?v=60Z6rrYAa00" target="_blank">
    <img src="https://img.icons8.com/color/96/video.png" alt="Watch Demo" />
    <br>
    <strong>Click to watch the demonstration video</strong>
  </a>
</p>

---

# Practical Summary

| Area                | Activity Performed                                     | Tool Used        | Learning Outcome                                    |
| ------------------- | ------------------------------------------------------ | ---------------- | --------------------------------------------------- |
| Process Monitoring  | Reviewed running applications and background processes | Task Manager     | Understood how Windows manages active processes     |
| CPU Analysis        | Monitored processor utilization and performance graphs | Task Manager     | Learned how CPU activity changes over time          |
| Memory Analysis     | Reviewed memory consumption and available memory       | Task Manager     | Understood RAM allocation and utilization           |
| Disk Monitoring     | Observed disk activity and transfer rates              | Task Manager     | Learned how storage resources are used              |
| Advanced Monitoring | Examined detailed resource information                 | Resource Monitor | Gained deeper visibility into system resource usage |

---

# Part 1: Exploring Task Manager & Active Processes

## Objective

To become familiar with the Task Manager interface and understand how Windows displays running applications, background processes, and resource consumption.

## Activities Performed

* Opened Windows Task Manager.
* Explored the **Processes** tab.
* Reviewed currently running applications.
* Observed background processes running in the system.
* Examined CPU, Memory, and Disk usage values for individual processes.
* Identified applications consuming more system resources.

<p align="center">
  <img src="./Task Manager Processes.png"
       alt="Task Manager Processes"
       width="900"/>
</p>

## Key Observations

| Observation          | Description                                                               |
| -------------------- | ------------------------------------------------------------------------- |
| Running Applications | Multiple user applications were visible in the Apps section.              |
| Background Processes | Windows services and supporting processes were running in the background. |
| Resource Usage       | Each process displayed its current CPU, Memory, and Disk consumption.     |
| Process Visibility   | Task Manager provided a quick overview of system activity.                |

## Skills Developed

* Process Identification
* Basic Performance Monitoring
* Resource Usage Analysis

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=JDDLWTWSuu4

---

# Part 2: CPU Monitoring & Analysis

## Objective

To understand CPU utilization information available in Task Manager and observe processor activity in real time.

## Activities Performed

* Opened the **Performance** tab.
* Selected the **CPU** section.
* Observed the CPU utilization graph.
* Reviewed processor specifications displayed by Windows.
* Monitored CPU usage percentage and processor speed.
* Examined information such as processes, threads, handles, and uptime.

<p align="center">
  <img src="./CPU Monitoring.png"
       alt="CPU Monitoring"
       width="900"/>
</p>

## Key Observations

| Observation           | Description                                                          |
| --------------------- | -------------------------------------------------------------------- |
| CPU Utilization       | Real-time processor usage was displayed through a performance graph. |
| Processor Information | Windows displayed CPU model, core count, and logical processors.     |
| System Activity       | CPU usage fluctuated based on running tasks and background activity. |
| Performance View      | Historical CPU usage was visible over the previous 60 seconds.       |

## Skills Developed

* CPU Performance Monitoring
* Performance Graph Interpretation
* System Resource Analysis

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=6yCZnJb1RW4

---

# Part 3: Memory Utilization Analysis

## Objective

To understand how Windows reports memory utilization and how RAM is allocated across the system.

## Activities Performed

* Opened the **Memory** section under the Performance tab.
* Reviewed total installed memory.
* Observed memory currently in use.
* Examined available and cached memory values.
* Reviewed memory speed and hardware-related information.

<p align="center">
  <img src="./Memory Monitoring.png"
       alt="Memory Monitoring"
       width="900"/>
</p>

## Key Observations

| Observation        | Description                                                         |
| ------------------ | ------------------------------------------------------------------- |
| Memory Usage       | Windows displayed current RAM utilization.                          |
| Available Memory   | Remaining memory available to the system was visible.               |
| Cached Memory      | Cached memory information was displayed separately.                 |
| Memory Composition | Task Manager provided a visual representation of memory allocation. |

## Skills Developed

* Memory Monitoring
* RAM Utilization Analysis
* Performance Observation

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=Ej5Fs2gzOak

---

# Part 4: Disk Activity Monitoring

## Objective

To observe storage performance metrics and understand disk activity information provided by Windows.

## Activities Performed

* Opened the **Disk 0 (C:)** performance section.
* Monitored disk activity graphs.
* Reviewed read and write speeds.
* Observed active time and response time metrics.
* Examined storage device information displayed by Windows.

<p align="center">
  <img src="./Disk Monitoring.png"
       alt="Disk Monitoring"
       width="900"/>
</p>

## Key Observations

| Observation         | Description                                               |
| ------------------- | --------------------------------------------------------- |
| Active Time         | Displayed how actively the storage device was being used. |
| Read/Write Activity | Real-time disk transfer activity was visible.             |
| Response Time       | Storage response metrics were displayed.                  |
| Device Information  | Disk type and capacity information were available.        |

## Skills Developed

* Disk Performance Monitoring
* Storage Activity Analysis
* System Performance Observation

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=fY2IVV1plcY

---

# Part 5: Advanced Analysis Using Resource Monitor

## Objective

To use Windows Resource Monitor for a more detailed view of resource consumption by processes and services.

## Activities Performed

* Opened Resource Monitor.
* Explored CPU-related information.
* Reviewed memory usage details.
* Examined disk activity information.
* Observed resource statistics at the process level.

---

## CPU Analysis

### Topics Reviewed

* Running Processes
* CPU Activity Information
* Process-Level Resource Usage

<p align="center">
  <img src="./Resource Monitor CPU Analysis.png"
       alt="Resource Monitor CPU Analysis"
       width="900"/>
</p>

---

## Memory Analysis

### Topics Reviewed

* Physical Memory Usage
* Available Memory
* Memory Allocation Information
* Hard Fault Statistics

<p align="center">
  <img src="./Resource Monitor Memory Analysis.png"
       alt="Resource Monitor Memory Analysis"
       width="900"/>
</p>

---

## Disk Analysis

### Topics Reviewed

* Disk Activity
* Read Operations
* Write Operations
* Process-Level Disk Usage

<p align="center">
  <img src="./Resource Monitor Disk Analysis.png"
       alt="Resource Monitor Disk Analysis"
       width="900"/>
</p>

---

## Key Learning from Resource Monitor

Resource Monitor provided a more detailed view of system activity compared to Task Manager. It allowed observation of how individual processes were utilizing memory and other system resources, making it easier to understand overall system behavior.

## Skills Developed

* Advanced Resource Monitoring
* Process-Level Analysis
* Windows Performance Observation

## Video Demonstration

**Video Link:**
https://www.youtube.com/watch?v=PPOuzXYHJ6k

---

# Overall Learning Outcome

This practical provided hands-on experience with two important Windows monitoring tools: **Task Manager** and **Resource Monitor**.

Through this exercise, I learned how to:

* Monitor running processes.
* Analyze CPU performance metrics.
* Understand memory utilization.
* Observe disk activity.
* Navigate Windows performance monitoring tools.
* Interpret resource usage information presented by Windows.

These are foundational skills that support further learning in IT Operations, System Administration, SOC Analysis, and Cybersecurity.

---

# Tools Used

| Tool                     | Purpose                                    |
| ------------------------ | ------------------------------------------ |
| Task Manager             | Monitor processes and system performance   |
| Resource Monitor         | Detailed analysis of resource utilization  |
| Windows Operating System | Environment used for monitoring activities |

---

# Key Takeaways

* Task Manager provides a quick overview of system resource usage.
* CPU performance graphs help visualize processor activity.
* Memory monitoring helps understand RAM utilization.
* Disk monitoring provides visibility into storage activity.
* Resource Monitor offers more detailed information than Task Manager.
* Understanding resource usage is an important first step in troubleshooting performance issues.

---

# Repository Structure

```text
Practical-01-System-Monitoring/
│
├── README.md
├── System monitoring infographic.png
├── Task Manager Processes.png
├── CPU Monitoring.png
├── Memory Monitoring.png
├── Disk Monitoring.png
├── Resource Monitor CPU Analysis.png
├── Resource Monitor Memory Analysis.png
├── Resource Monitor Disk Analysis.png
```

---

# Author

**Himadri Singh**

---

# License

This practical is created for educational and learning purposes.
