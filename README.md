# Linux System Information and Network Connectivity Analysis

This repository contains the setup, execution, and output analysis for a Linux system administration and networking assignment. It details system information gathering, hardware resource inspection, and basic network connectivity testing performed on a Kali Linux virtual machine. The project demonstrates foundational command-line operations and network diagnostic techniques using standard Linux utilities.

## Table of Contents

* Project Overview
* Network Topology
* Tools and Technologies
* Configuration Steps
* Results and Findings
* Author

## Project Overview

The objective of this project is to perform basic Linux system administration tasks and evaluate network reachability using command-line tools. The assignment is split into two core sections: inspecting system identity, kernel parameters, and storage allocation, and conducting ICMP network diagnostics to analyze latency and domain name resolution.

## Network Topology

The environment comprises a single **Kali Linux** virtual host operating inside **Oracle VirtualBox**. The virtual machine uses the host machine's network stack to communicate with external IP endpoints. Diagnostic tests target remote public destinations, specifically the public DNS resolver (`8.8.8.8`) and domain web servers (`google.com` at IPv4 address `142.250.129.138`), to evaluate external routing and name resolution performance.

## Tools and Technologies

* **Kali Linux** - Security-focused Linux operating system running within a virtual environment.


* **Oracle VirtualBox** - Desktop virtualization hypervisor hosting the Linux operating system.


* **Linux Command Line Interface (CLI)** - Terminal interface used to execute system and networking commands.


* **System Inspection Utilities** - Tools including `whoami`, `hostname`, `pwd`, `uname`, `free`, `df`, and `uptime` used for gathering system specifications.


* **Ping Utility (ICMP)** - Network testing tool used to send echo request packets to target network interfaces.



## Configuration Steps

1. Executed environment identity commands `whoami`, `hostname`, and `pwd` to confirm the active user profile and system path.


2. Checked operating system and kernel build details using `uname -a`.


3. Audited available RAM and disk partition storage using `free -h` and `df -h`.


4. Checked system runtime and system load averages using `uptime`.


5. Initiated direct IP connectivity and latency testing using `ping -c 2 8.8.8.8`.


6. Tested domain name resolution and round-trip time variations using `ping -c 4 google.com`.



## Results and Findings

* **System Identity**: Confirmed active username as `anthony`, system hostname as `vbox`, and home directory path as `/home/anthony`.


* **Kernel & OS Details**: Verified the system runs Linux kernel version `6.19.14+kali-amd64` on an `x86_64` architecture.


* **Resource Inventory**: Recorded total system memory of **2.8Gi** RAM and primary root partition (`/`) available disk space of **31G** out of **48G**.


* **Direct IP Connectivity**: Pinging `8.8.8.8` succeeded with 0% packet loss and an average round-trip time of **187.717 ms**.


* **DNS Resolution & Routing**: Pinging `google.com` successfully resolved to IP `142.250.129.138` with 0% packet loss and an average round-trip time of **159.798 ms**. The observed latency variation compared to `8.8.8.8` demonstrates differences in network routes and target infrastructure.



## Author

* **Name**: Anthony Aleke Chukwuebuka


* **Email**: `LOUISANTHONY128@GMAIL.COM`

* **Student ID**: CS-C26-07-EU-011


* **Date**: August 27, 2026
