# Investigation Findings

## 1. Thunderbird Was Downloaded, Installed, and Used

A Mozilla Thunderbird installer was located in Charlie's Downloads folder.

A Zone.Identifier with `ZoneId=3` indicated that Windows classified the installer as originating from the Internet Zone.

An installation log confirmed that Thunderbird was installed, and recovered email artifacts showed that Charlie later used the application for email communication.

---

## 2. Quantum Cryptography Directory Appeared Between Images

The `Quantum Cryptography` directory was not present in the November 12 disk image.

It was present in the December 11 image with a filesystem creation timestamp of December 4, 2009.

A Recent Documents artifact also showed later access to the directory.

---

## 3. WIPO Download Activity Was Correlated With a File on Disk

Firefox download records showed activity involving `wipo.int`.

A corresponding downloaded file was located inside Charlie's `Quantum Cryptography` directory.

This allowed browser history to be correlated with an actual filesystem artifact.

---

## 4. Technical Web Searches Were Identified

Browser artifacts showed searches involving:

- steganography
- steganography tools
- 7-Zip
- hex editors

These searches provide context for technical activity on the workstation but do not prove that any particular technique was used.

---

## 5. Removable Storage Devices Were Connected

Windows artifacts identified multiple removable-storage devices, including a SanDisk Cruzer Micro U3 flash drive.

Recent Documents also referenced files on an `F:\` drive.

The available evidence did not conclusively identify which removable device was assigned that drive letter.

---

## 6. Deleted Files Were Reviewed

Deleted filesystem entries were examined.

The largest deleted files reviewed were primarily system, antivirus, or application files and did not provide a meaningful user-activity finding.

---

## Overall Finding

Comparison of the November and December disk images identified changes in software, email activity, browser activity, files, directories, and removable-storage usage.

The investigation demonstrates how multiple forensic artifacts can be correlated to reconstruct activity on a workstation.
