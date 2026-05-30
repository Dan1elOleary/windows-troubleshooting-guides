# Disk Space Cleanup Guide

This guide outlines a structured process for troubleshooting low disk space on Windows computers. Low storage can cause slow performance, failed updates, application crashes, profile problems, and general system instability.

---

## Issue Overview

A user reports that their computer is low on storage, receiving disk space warnings, running slowly, failing updates, or unable to save files.

---

## Common Symptoms

* Low disk space warning
* C: drive is nearly full
* Computer runs slowly
* Windows updates fail
* Applications crash or freeze
* User cannot save files
* Downloads fail
* Temporary files consume large amounts of space
* OneDrive sync errors appear
* Profile issues occur during login

---

## Possible Causes

* Large Downloads folder
* Full Recycle Bin
* Temporary files
* Old Windows update files
* Large user profile
* Large videos, photos, or ISO files
* Duplicate files
* OneDrive sync data
* Old application installers
* Browser cache
* Unused applications
* System restore points or shadow copies

---

## Initial Questions to Ask the User

* Are you receiving a low disk space warning?
* Are you unable to save files?
* Did the issue start recently?
* Do you store large files locally?
* Are you using OneDrive or another sync tool?
* Has the computer recently installed updates?
* Is the issue affecting performance or only storage?

---

## Troubleshooting Steps

### 1. Check Available Storage

Open File Explorer and review the C: drive.

Check:

* Total storage size
* Free space available
* Percentage of drive used
* Whether other drives are available

You can also check storage from:

Settings > System > Storage

---

### 2. Review Storage Usage

Use Windows Storage settings to identify what is using space.

Common categories include:

* Apps
* Temporary files
* Documents
* Pictures
* Videos
* Downloads
* Other users
* System files

This helps determine where cleanup should begin.

---

### 3. Empty the Recycle Bin

The Recycle Bin can hold a large amount of data.

Before emptying it, confirm there is no company policy requiring review or retention.

---

### 4. Clean Temporary Files

Use Windows Storage settings or Disk Cleanup to remove safe temporary files.

Common cleanup options include:

* Temporary files
* Windows update cleanup
* Delivery optimization files
* Temporary internet files
* DirectX shader cache
* Thumbnails
* Recycle Bin

Avoid deleting user files unless confirmed.

---

### 5. Review the Downloads Folder

The Downloads folder often contains old installers, PDFs, ZIP files, videos, and duplicate files.

Before deleting:

* Ask the user to review important files.
* Move business files to approved storage.
* Delete only files that are no longer needed.
* Follow company data retention policy.

---

### 6. Review Large Files

Search for large files that may be consuming disk space.

Examples include:

* Videos
* ISO files
* ZIP files
* Old installers
* Database exports
* Large log files
* Backup files

Large files should be deleted, moved, or archived only with user or policy approval.

---

### 7. Check Installed Applications

Review installed applications for unused or unauthorized software.

Possible actions:

* Remove unused applications if approved
* Remove old versions after confirming they are not needed
* Avoid removing business-required software
* Document any software removed

---

### 8. Check OneDrive or Sync Issues

OneDrive or other sync tools may store files locally.

Review:

* Sync status
* Locally available files
* Files marked to always keep on this device
* Large synced folders
* Sync errors

If allowed, use Files On-Demand to reduce local storage usage.

---

### 9. Restart and Recheck Storage

After cleanup:

1. Restart the computer.
2. Recheck available disk space.
3. Confirm performance has improved if slowness was reported.
4. Confirm the user can save files or run updates.

---

## Resolution Notes

Document the final cause and fix.

Example:

The device had low disk space due to temporary files, old installers in the Downloads folder, and a full Recycle Bin. Temporary files were removed, the Recycle Bin was emptied, and unnecessary installers were deleted with user approval. Available storage increased and the user confirmed that performance improved.

---

## Escalation Points

Escalate the issue if:

* Disk space fills up again quickly
* Unknown files are consuming storage
* Windows update cleanup fails
* The drive is too small for business use
* Storage issues are caused by application logs
* Multiple user profiles are consuming excessive space
* There may be malware or abnormal file growth
* Hardware replacement or storage upgrade may be needed

---

## User-Facing Response Example

Hello,

I reviewed the storage issue and found that the computer was low on available disk space due to temporary files, old downloads, and a full Recycle Bin. I cleaned up approved temporary files and removed unnecessary items with confirmation.

The computer now has more available storage. Please let us know if the low disk space warning returns.
