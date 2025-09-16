*Task 4: The File System*

## 📑 Table of Contents
1. [Introduction](#introduction)  
2. [File Systems Before NTFS](#file-systems-before-ntfs)  
3. [What is NTFS?](#what-is-ntfs)  
4. [Features of NTFS](#features-of-ntfs)  
5. [NTFS Permissions](#ntfs-permissions)  
6. [How to View Permissions](#how-to-view-permissions)  
7. [Alternate Data Streams (ADS)](#alternate-data-streams-ads)  
8. [Answer](#answer)  

---

## 📖 Introduction
- Modern versions of Windows use **NTFS (New Technology File System)**.  
- Before NTFS, Windows used **FAT16/FAT32 (File Allocation Table)** and **HPFS (High Performance File System)**.  
- FAT partitions are still common in USB drives, MicroSD cards, etc., but not usually on Windows OS drives.

---

## 📂 File Systems Before NTFS
- **FAT16 / FAT32**  
- **HPFS (High Performance File System)**  

> 📌 FAT is still widely used in portable storage devices like USB and SD cards.  

---

## 💡 What is NTFS?
- **NTFS = New Technology File System**  
- A **journaling file system** → can repair folders/files using log information in case of failure.  
- FAT cannot do this.  

---

## ✨ Features of NTFS
- Supports files larger than **4 GB**.  
- Allows **permissions** on files/folders.  
- **File/folder compression**.  
- **Encryption (EFS – Encryption File System)**.  

---

## 🔒 NTFS Permissions
Permissions that can be applied to files and folders:  

- **Full Control**  
- **Modify**  
- **Read & Execute**  
- **List folder contents**  
- **Read**  
- **Write**  

For detailed behavior, refer to Microsoft docs on **Special Permissions**.  

---

## 👀 How to View Permissions
1. Right-click the file/folder → **Properties**.  
2. Go to the **Security** tab.  
3. Select the **user, computer, or group** to view permissions.  

---

## 🗂️ Alternate Data Streams (ADS)
- Specific to **NTFS**.  
- Every file has at least one stream (`$DATA`).  
- ADS allows files to contain **more than one data stream**.  
- Not visible in Windows Explorer.  

### 🔐 Security Perspective:
- Malware can use ADS to hide data.  
- Legit use: downloaded files store identifiers in ADS to mark origin (e.g., "downloaded from the Internet").  

📌 Links:  
- Hands-on practice: [Day 21 — Advent of Cyber 2][tryhackme]  
- ADS description on [MalwareBytes][mb]

[ps]: https://learn.microsoft.com/en-us/powershell/scripting/overview?view=powershell-7.5&viewFallbackFrom=powershell-7.1
[tryhackme]: https://tryhackme.com/room/adventofcyber2
[mb]: https://www.malwarebytes.com/blog/101/2015/07/introduction-to-alternate-data-streams


---

## ✅ Answer
**Q: What is the meaning of NTFS?**  
**A: New Technology File System**  

---
