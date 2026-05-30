# Application Crash Troubleshooting Guide

This guide outlines a structured process for troubleshooting Windows applications that crash, freeze, fail to open, or display repeated error messages. Application issues may be caused by updates, corrupt settings, missing dependencies, permissions, add-ins, user profile issues, or system resource problems.

---

## Issue Overview

A user reports that an application is crashing, freezing, not opening, closing unexpectedly, or displaying an error message.

---

## Common Symptoms

* Application will not open
* Application opens and immediately closes
* Application freezes during use
* Error message appears when launching the application
* Application crashes after signing in
* Application crashes when opening a specific file
* Application runs slowly or becomes unresponsive
* Application works for one user but not another
* Application works on one computer but not another

---

## Possible Causes

* Corrupt application installation
* Missing or damaged application files
* Recent software update
* Windows update compatibility issue
* Add-in or extension problem
* Corrupt user profile
* Permission issue
* Licensing or sign-in issue
* Insufficient system resources
* Antivirus or security tool interference
* Corrupt cached data
* Outdated application version

---

## Initial Questions to Ask the User

* What application is crashing?
* When did the issue start?
* Does the application show an error message?
* Does it crash during launch or while doing a specific task?
* Does the issue happen with one file or all files?
* Does the issue happen for other users?
* Has the application or Windows recently updated?
* Have you already restarted the computer?

---

## Troubleshooting Steps

### 1. Confirm the Application and Error

Document the key details before making changes.

Information to collect:

* Application name
* Application version, if available
* Error message
* Screenshot, if available
* When the crash happens
* Whether the issue is user-specific or device-specific

Accurate error details help determine whether the issue is related to the application, Windows, user profile, licensing, or network access.

---

### 2. Restart the Application and Computer

Start with a clean restart.

Steps:

1. Close the application.
2. End stuck processes in Task Manager if needed.
3. Restart the computer.
4. Open the application again.
5. Test the same action that caused the issue.

A restart can clear temporary issues, locked files, stuck processes, and memory-related problems.

---

### 3. Check for System Resource Issues

Open Task Manager and review:

* CPU usage
* Memory usage
* Disk usage
* Application process status
* Background applications

If the computer is low on resources, the application may crash or freeze because the system cannot provide enough memory or processing capacity.

---

### 4. Test Another File or Workflow

If the application crashes when opening a specific file, test a different file.

If only one file crashes, possible causes include:

* Corrupt file
* Unsupported format
* File stored in a problematic location
* Permission issue
* OneDrive or shared storage sync issue

If all files crash, the issue is more likely application-wide.

---

### 5. Check for Updates

Review available updates for:

* The affected application
* Windows
* Microsoft Store apps, if applicable
* Drivers, if graphics or hardware acceleration is involved

Do not install updates outside company policy or without approval.

---

### 6. Disable Add-ins or Extensions

Some applications crash because of add-ins or extensions.

Common examples include:

* Outlook add-ins
* Browser extensions
* Office plug-ins
* PDF toolbars
* Third-party integrations

If the application works with add-ins disabled, re-enable them one at a time to identify the problem add-in.

---

### 7. Clear Application Cache or Temporary Data

Some applications store cached data that can become corrupt.

Examples include:

* Teams cache
* Browser cache
* Office temporary files
* AppData cache folders
* Locally stored sign-in tokens

Only clear cache using approved procedures, especially for business applications.

---

### 8. Repair or Reinstall the Application

If basic steps fail, repair or reinstall the application if approved.

Possible actions:

* Use the Apps & Features repair option
* Run a Microsoft Office repair
* Uninstall and reinstall the application
* Reinstall using company software deployment tools
* Confirm licensing after reinstall

---

### 9. Test with Another User Profile

If the application works for another user on the same device, the issue may be profile-specific.

Possible profile-related causes include:

* Corrupt user settings
* Bad cached credentials
* AppData corruption
* User-specific add-ins
* User-specific permissions

---

## Resolution Notes

Document the final cause and fix.

Example:

The application was crashing during startup because a third-party add-in was failing to load. The add-in was disabled, the application was restarted, and the user confirmed that the application opened successfully.

---

## Escalation Points

Escalate the issue if:

* Application logs show repeated critical errors
* Multiple users are affected
* The application requires vendor support
* Licensing or permissions need administrator review
* The application crashes after reinstall
* The issue involves business-critical software
* Data corruption or data loss is suspected

---

## User-Facing Response Example

Hello,

I reviewed the application issue and found that the program was crashing because an add-in was not loading correctly. I disabled the problem add-in, restarted the application, and confirmed that it opened successfully.

Please continue using the application and let us know if the issue returns.
