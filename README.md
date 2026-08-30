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

## Screenshots

Supporting screenshots are located in the `screenshots` folder.

## Disclaimer

This project was completed for educational and portfolio purposes using a publicly available forensic training dataset.