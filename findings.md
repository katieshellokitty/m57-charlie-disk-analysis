# Investigation Findings

## 1. Thunderbird Was Downloaded, Installed, and Used

A Mozilla Thunderbird installer was located in Charlie's Downloads folder.

The installer contained a `Zone.Identifier` with `ZoneId=3`, indicating that Windows classified the file as originating from the Internet Zone.

An installation log confirmed that Thunderbird was installed on the workstation. Email artifacts recovered from Charlie's Thunderbird profile also confirmed that the program was used for email communication.

---

## 2. Quantum Cryptography Research Was Related to a Work Assignment

An email dated November 30, 2009 instructed Charlie and Jo to begin researching quantum cryptography and related patents for a new company contract.

The activity that followed included:

- Creation of the `Quantum Cryptography` directory on December 4
- Recent Documents activity showing access to the directory on December 7
- Patent and WIPO-related downloads on December 10
- Multiple keyword-search results related to quantum cryptography

These artifacts provide context for the research activity and show a progression from the work assignment to later filesystem and browser activity.

---

## 3. WIPO Downloads Were Correlated With Files on Disk

Firefox download artifacts showed files being downloaded from the World Intellectual Property Organization (`wipo.int`).

One recovered file, `GB2009000189_11092009.xml.gz`, was located inside Charlie's `Quantum Cryptography` directory.

The browser download timestamp and filesystem timestamp occurred only seconds apart, allowing the browser record to be correlated with the actual downloaded file.

---

## 4. Steganography Research Was Identified

Browser artifacts showed searches involving:

- steganography
- steganography tool free
- 7zip
- hex editor
- open source hex editor

Keyword searching produced additional steganography-related browser and file artifacts.

These searches demonstrate technical research activity but do not by themselves prove that steganography was used.

---

## 5. Invisible Secrets 2.1 Was Installed

Keyword analysis identified files belonging to `Invisible Secrets 2.1` under:

`C:\Program Files\Invisible Secrets 2.1`

The application's README described it as an encryption/steganography program capable of using JPG, PNG, and BMP images as carrier files.

This confirmed that steganography-capable software was present on the workstation.

---

## 6. Invisible Secrets 2.1 Was Executed

Windows Prefetch evidence identified:

`ISECRETS2.EXE`

from the Invisible Secrets 2.1 installation directory.

Autopsy reported a run count of **4**, confirming that the application was executed on the workstation.

Although execution was confirmed, the evidence reviewed does not establish that a specific file was used to conceal information.

---

## 7. Removable Storage Devices Were Connected

Windows artifacts identified multiple removable-storage devices, including:

- SanDisk Cruzer Micro U3
- Alcor Micro Corp. Flash Drive
- LaCie Rugged Triple Interface Mobile Hard Drive

Recent Documents also referenced files located on an `F:\` drive.

The available evidence did not conclusively identify which removable device was assigned that drive letter.

---

## 8. Deleted Files Were Reviewed

Deleted filesystem entries were examined during the investigation.

The largest deleted files reviewed were primarily operating system, antivirus, and application-related files and did not provide a significant user-activity finding.

---

## Overall Finding

Comparison of the November 12 and December 11 disk images revealed changes in software, email communication, browser activity, files, directories, removable-storage activity, and program execution.

The analysis demonstrated how multiple forensic artifacts can be correlated to reconstruct user activity. In particular, email and filesystem evidence provided context for the quantum cryptography research, while browser, application, and Prefetch artifacts established that steganography-capable software was researched, installed, and executed.

The available evidence does not establish that a specific file was concealed using steganography.
