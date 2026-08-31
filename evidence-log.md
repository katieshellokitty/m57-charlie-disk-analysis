## Finding 009 - Invisible Secrets 2.1 Identified

**Data Source:**  
charlie-2009-12-11.E01

**Application:**  
Invisible Secrets 2.1

**Artifact:**  
readme.txt

**Location:**  
C:\Program Files\Invisible Secrets 2.1\readme.txt

**Accessed:**  
2009-11-19 13:43:31 EST

**Finding:**  
A README file for Invisible Secrets 2.1 was located in the Program Files directory. The documentation describes the application as an encryption/steganography program capable of using JPG, PNG, and BMP images as carrier files.

The README was accessed shortly after web searches involving steganography and steganography tools.

**Significance:**  
This confirms that steganography-capable software was present on the workstation.

---

## Finding 010 - Invisible Secrets 2.1 Execution Confirmed

**Data Source:**  
charlie-2009-12-11.E01

**Program:**  
ISECRETS2.EXE

**Path:**  
C:\Program Files\Invisible Secrets 2.1

**Date/Time:**  
2009-11-30 11:48:17 EST

**Prefetch Run Count:**  
4

**Source:**  
Windows Prefetch Analyzer

**Finding:**  
A Windows Prefetch artifact for `ISECRETS2.EXE` was identified in Autopsy's Run Programs results.

Autopsy reported a run count of 4, confirming that Invisible Secrets 2.1 was executed on the workstation.

**Significance:**  
The evidence confirms execution of steganography-capable software. However, the reviewed artifacts do not establish that a particular file was used to conceal data.

---

## Finding 011 - Work Assignment Explains Quantum Cryptography Research

**Data Source:**  
charlie-2009-12-11.E01

**Email Subject:**  
Re: New business

**Participants:**  
- Charlie: charlie@m57.biz
- Pat: pat@m57.biz
- Jo: jo@m57.biz

**Email Date:**  
2009-11-30 11:46:08 EST

**Finding:**  
An email thread contained instructions to begin researching quantum cryptography and patents related to the subject for a new company contract.

**Correlation:**  
Following the email:

- The `Quantum Cryptography` directory was created on December 4.
- A Recent Documents artifact showed access to the directory on December 7.
- Patent and WIPO-related files were downloaded into the directory on December 10.

**Significance:**  
The email provides context for the later quantum cryptography research and supports that the activity was related to a work assignment.
