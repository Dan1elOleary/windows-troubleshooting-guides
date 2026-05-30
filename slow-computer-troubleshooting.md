# Slow Computer Troubleshooting Guide

This guide outlines a structured process for troubleshooting a Windows computer that is running slowly. Slow performance issues can be caused by resource usage, startup applications, storage problems, malware, updates, hardware limitations, or user profile issues.

---

## Issue Overview

A user reports that their Windows computer is slow, freezing, taking a long time to start, or responding slowly when opening applications.

---

## Common Symptoms

* Computer takes a long time to boot
* Applications open slowly
* System freezes or becomes unresponsive
* High CPU, memory, or disk usage
* Slow login process
* Delayed typing or mouse response
* Browser tabs or Microsoft Office applications lag
* File Explorer takes a long time to load

---

## Possible Causes

* Too many startup applications
* High CPU or memory usage
* Low disk space
* Windows updates running in the background
* Malware or unwanted software
* Outdated drivers
* Corrupt user profile
* Too many browser extensions
* Insufficient RAM
* Background sync tools consuming resources
* Failing hard drive or storage issue

---

## Initial Questions to Ask the User

* When did the slowness start?
* Is the issue constant or does it happen only at certain times?
* Does the issue happen after logging in, opening a certain program, or connecting to the network?
* Has anything changed recently, such as software installs, updates, or new hardware?
* Are other users or devices having the same problem?
* Has the computer been restarted recently?

---

## Troubleshooting Steps

### 1. Confirm Basic System Information

Check the device name, Windows version, logged-in user, uptime, and available storage.

Useful areas to review:

* Settings > System > About
* Task Manager > Performance
* Task Manager > Startup apps
* File Explorer > This PC
* Windows Update history

---

### 2. Restart the Computer

If the computer has not been restarted recently, perform a restart.

A restart can clear stuck processes, pending updates, memory usage, and temporary performance issues.

---

### 3. Check Task Manager

Open Task Manager and review:

* CPU usage
* Memory usage
* Disk usage
* Startup applications
* Processes using high resources

Common findings:

* Browser using high memory
* OneDrive or Teams syncing heavily
* Windows Update running
* Antivirus scan in progress
* Disk usage stuck near 100%

---

### 4. Review Startup Applications

Disable unnecessary startup applications if approved by policy.

Examples of apps to review:

* Chat applications
* Updaters
* Vendor utilities
* Non-business applications
* Unused background tools

Avoid disabling security tools, backup tools, RMM agents, or business-required applications.

---

### 5. Check Available Disk Space

Low disk space can cause performance issues.

Check:

* Free space on the C: drive
* Downloads folder
* Recycle Bin
* Temporary files
* Old user profiles
* Large unused files

If disk space is low, follow the disk cleanup process.

---

### 6. Check for Windows Updates

Review whether Windows updates are pending, downloading, installing, or failing.

Pending updates may cause slow performance until the update cycle completes.

---

### 7. Scan for Malware or Unwanted Software

Run a security scan using approved tools.

Check for:

* Unknown applications
* Browser extensions
* Unwanted startup items
* Suspicious processes
* Security alerts

---

### 8. Test with Another User Profile

If the issue only affects one user, test another profile if possible.

If another user profile works normally, the issue may be related to:

* Corrupt profile
* Large profile data
* Login scripts
* User-specific startup apps
* Profile sync issues

---

## Resolution Notes

Document the final cause and what resolved the issue.

Example:

The workstation was running slowly due to low disk space and multiple unnecessary startup applications. Temporary files were removed, the Recycle Bin was emptied, startup applications were reviewed, and the device was restarted. Performance improved after cleanup.

---

## Escalation Points

Escalate the issue if:

* Disk usage remains at 100%
* The hard drive may be failing
* Malware is suspected
* The issue affects multiple users
* The system freezes after basic troubleshooting
* Windows updates repeatedly fail
* The device may need hardware upgrades

---

## User-Facing Response Example

Hello,

I reviewed the computer performance issue and found that the device was low on available storage and had several background applications running at startup. I cleared temporary files, reviewed startup items, and restarted the workstation. Performance appears to have improved after these steps.

Please monitor the computer and let us know if the slowness returns.
