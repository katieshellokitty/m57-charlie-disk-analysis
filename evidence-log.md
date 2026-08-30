# Evidence Log

## Finding 001 - Thunderbird Internet Download

**Data Source:** `charlie-2009-11-12.E01`

**Artifact:** `Thunderbird Setup 2.0.0.23.exe`

**Location:**  
`Documents and Settings/Charlie/My Documents/Downloads`

**Created:**  
2009-11-12 20:51:55 EST

**Additional Artifact:**  
`Zone.Identifier`

**ZoneId:** `3`

**Finding:**  
The Thunderbird installer was located in Charlie's Downloads directory. Its Zone.Identifier contained `ZoneId=3`, showing that Windows classified the file as originating from the Internet Zone.

---

## Finding 002 - Thunderbird Installation

**Data Source:** `charlie-2009-11-12.E01`

**Artifact:** `install.log`

**Location:**  
`C:\Program Files\Mozilla Thunderbird`

**Version:** 2.0.0.23

**Finding:**  
The Thunderbird installation log confirmed that Mozilla Thunderbird was installed on the workstation.

**Timestamp Note:**  
The installation log displayed `2009-11-12 17:52:39`, while filesystem timestamps displayed approximately `20:52 EST`. Both values were preserved as shown by the artifacts.

---

## Finding 003 - Thunderbird Email Usage

**Data Source:** `charlie-2009-12-11.E01`

**Account:** `charlie@m57.biz`

**Source:**  
`Documents and Settings/Charlie/Application Data/Thunderbird/Profiles/4zy34x9h.default/Mail/Local Folders/Sent`

**Example Message:**  
Subject: Thanksgiving  
Date: 2009-11-24 11:48:22 EST

**Finding:**  
A sent email was recovered directly from Charlie's Thunderbird profile, confirming that Thunderbird was used for email communication.

---

## Finding 004 - WIPO Download

**Data Source:** `charlie-2009-12-11.E01`

**File:** `GB2009000189_11092009.xml.gz`

**Location:**  
`Documents and Settings/Charlie/My Documents/Quantum Cryptography`

**Browser Download Time:**  
2009-12-10 17:21:16 EST

**File Created/Modified:**  
2009-12-10 17:21:20 EST

**Finding:**  
Firefox recorded a download from `wipo.int`. The corresponding file was also located on the filesystem in Charlie's Quantum Cryptography directory.

---

## Finding 005 - Quantum Cryptography Directory

**Data Sources:**
- `charlie-2009-11-12.E01`
- `charlie-2009-12-11.E01`

**November Image:**  
The Quantum Cryptography directory was not present.

**December Image:**  
The directory was present with a creation timestamp of:

`2009-12-04 16:53:27 EST`

**Finding:**  
The directory appeared between the two forensic snapshots.

---

## Finding 006 - Recent Access to Quantum Cryptography

**Data Source:** `charlie-2009-12-11.E01`

**Artifact:** `Quantum Cryptography.lnk`

**Date Accessed:**  
2009-12-07 14:52:26 EST

**Finding:**  
A Recent Documents shortcut indicated that the Quantum Cryptography directory had been accessed.

---

## Finding 007 - Removable Storage Activity

**Data Source:** `charlie-2009-12-11.E01`

**Devices Identified:**
- SanDisk Cruzer Micro U3
- Alcor Micro Corp. Flash Drive
- LaCie Rugged Triple Interface Mobile Hard Drive

**SanDisk Device ID:**  
`43175107A4C24AD4`

**Finding:**  
Windows artifacts confirmed that multiple removable-storage devices had been connected to the workstation.

Recent Documents also referenced an `F:\` drive, although the available evidence did not conclusively identify which removable device was assigned that drive letter.

---

## Finding 008 - Technical Web Searches

**Data Source:** `charlie-2009-12-11.E01`

**Searches Identified:**
- steganography
- steganography tool free
- 7zip
- hex editor
- open source hex editor

**Finding:**  
Browser artifacts showed technical research involving steganography and file-analysis utilities.

These searches demonstrate research activity but do not prove that the tools or techniques were actually used.

---

## Deleted File Review

Deleted filesystem entries were reviewed.

The largest deleted items examined were primarily operating system, antivirus, or application-related files and did not provide a significant user-activity finding.
