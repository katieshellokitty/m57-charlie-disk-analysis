# M57 Charlie Disk Image Analysis

## Overview

This project documents a forensic analysis of two disk images from the M57 forensic dataset using Autopsy.

The goal of the investigation was to compare two snapshots of Charlie's workstation and identify changes in user activity between November 12, 2009 and December 11, 2009.

## Investigation Question

What user activity, files, programs, and Internet activity appeared or changed on Charlie's workstation between the November 12 and December 11 disk images?

## Tools Used

- Autopsy 4.23.1
- Windows
- M57 forensic disk images

## Evidence Sources

- charlie-2009-11-12.E01
- charlie-2009-12-11.E01

The original disk images are not included in this repository.

## Skills Demonstrated

- Disk image analysis
- File system examination
- Browser artifact analysis
- Email artifact analysis
- Windows artifact analysis
- USB/removable storage analysis
- Timeline reconstruction
- Deleted file review
- Artifact correlation
- Digital forensic documentation

## Key Findings

Findings from the investigation include software installation and use, email activity, technical web searches, removable storage activity, and changes to files and directories between the two disk images.

A more detailed breakdown is available in `findings.md`.

## Methodology

1. Loaded both E01 forensic images into Autopsy.
2. Examined the user file system.
3. Reviewed browser history and downloads.
4. Examined email artifacts.
5. Reviewed Recent Documents.
6. Examined removable storage artifacts.
7. Reviewed deleted files.
8. Compared artifacts between the two disk images.
9. Correlated timestamps to reconstruct user activity.
10. Documented relevant findings.

## Evidence Screenshots

### Autopsy Case Overview

Both forensic disk images were loaded into the same Autopsy case for comparison.

![Autopsy Case Overview](screenshots/02-autopsy-case-overview.png)

### Thunderbird Internet Download

The Thunderbird installer contained a Zone.Identifier with `ZoneId=3`, indicating that Windows classified the file as originating from the Internet Zone.

![Thunderbird Zone Identifier](screenshots/06-thunderbird-zone-identifier.png)

### Thunderbird Installer Metadata

Autopsy was used to review the Thunderbird installer and its filesystem metadata.

![Thunderbird Installer Metadata](screenshots/08-thunderbird-installer-metadata.png)

### Thunderbird Installation

The Thunderbird installation log confirmed installation of Mozilla Thunderbird on the workstation.

![Thunderbird Installation Log](screenshots/10-thunderbird-install-log.png)

### Thunderbird Email Usage

A recovered sent-mail artifact originated from Charlie's Thunderbird profile.

![Thunderbird Email Usage](screenshots/17-thunderbird-sent-email-source.png)

### WIPO Download Activity

Firefox download artifacts showed a file from WIPO being saved into Charlie's Quantum Cryptography directory.

![WIPO Download](screenshots/21-wipo-data-artifact.png)

### Downloaded WIPO File

The corresponding WIPO file was located on the filesystem.

![WIPO File Metadata](screenshots/23-wipo-file-metadata.png)

### November Disk Image Baseline

The Quantum Cryptography folder was absent from Charlie's My Documents directory in the November image.

![November Baseline](screenshots/24-november-my-documents-baseline.png)

### Quantum Cryptography Directory

The directory was present in the December image with a filesystem creation timestamp.

![Quantum Cryptography Folder](screenshots/26-quantum-folder-created-metadata.png)

### Removable Storage

Windows artifacts identified a SanDisk Cruzer Micro U3 removable storage device connected to the workstation.

![SanDisk USB Artifact](screenshots/33-sandisk-usb-artifact.png)

### Technical Web Searches

Browser artifacts showed searches involving steganography and file-analysis tools.

![Technical Web Searches](screenshots/37-web-searches-3.png)
