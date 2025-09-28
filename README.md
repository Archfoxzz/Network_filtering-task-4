# Network_filtering-task-4

# Task 4: Firewall Configuration on Windows

This repository contains the deliverables for Task 4 of the Elevate Labs Cyber Security Internship, focusing on firewall setup and use.

---

## Objective

The objective was to configure and test basic firewall rules to allow or block network traffic using built-in system tools.

---

## Tool Used

* **Tool:** Windows Defender Firewall with Advanced Security

---

## Steps Performed

1.  Accessed the "Windows Defender Firewall with Advanced Security" utility.
2.  Listed the currently active inbound rules to understand the baseline configuration.
3.  Added a new inbound rule to explicitly **block TCP port 23 (Telnet)**.
4.  Tested the rule using PowerShell's `Test-NetConnection` to confirm that connections to port 23 were successfully blocked.
5.  Removed the temporary test rule for port 23 to restore the system to its original state.
6.  All steps and GUI actions were documented via screenshots.

---

## How a Firewall Filters Traffic

A firewall filters traffic by inspecting each data packet that attempts to cross it. It compares the information in the packet's header (such as source IP address, destination IP address, source port, destination port, and protocol) against a list of configured rules. If the packet matches a rule, the firewall takes the corresponding action, which is typically to **Allow** or **Deny** the packet. Stateful firewalls add another layer by also considering whether the packet is part of an established, legitimate connection.

---

## Evidence

The screenshots demonstrating the above steps are located in the `screenshots_task4` folder in this repository.
