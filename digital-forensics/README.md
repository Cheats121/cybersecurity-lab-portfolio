# Digital Forensic Investigation

## Overview

This project involved conducting a digital forensic investigation on a seized virtual machine in a controlled laboratory environment.

The investigation focused on preserving evidence integrity, creating forensic disk images, identifying suspicious files and activity, recovering protected content, and documenting the investigation process.

## Objectives

The main objectives of the investigation were to:

- Acquire forensic images of the provided virtual disk evidence
- Verify evidence integrity using cryptographic hashes
- Analyze the disk image for suspicious and relevant files
- Identify manipulated or disguised files
- Recover password-protected documents
- Extract embedded data and files
- Maintain documentation of evidence handling

## Tools Used

- FTK Imager
- GuyMager
- Autopsy
- John the Ripper
- Hashcat
- HexEdit
- Binwalk
- VMware Workstation
- Windows
- Ubuntu

## Investigation Process

### 1. Evidence Acquisition

Forensic images were created using both FTK Imager and GuyMager.

The E01 format was used, and generated hashes were used to verify the integrity of the forensic images.

### 2. Forensic Analysis

The forensic image was loaded into Autopsy for analysis.

Relevant directories and files were identified and tagged for further examination.

### 3. File Extension Analysis

Several files were discovered with extensions that did not match their actual file signatures.

Hexadecimal header analysis was used to identify the true file formats.

### 4. Password Recovery

Some documents were password protected.

John the Ripper was used to extract password hashes, which were then processed using Hashcat and a wordlist-based attack.

### 5. File Carving and Extraction

Some files contained embedded data that could not be extracted directly through Autopsy.

HexEdit and Binwalk were used to identify file signatures and recover embedded images, audio, and text content.

### 6. Chain of Custody

The investigation included chain-of-custody documentation to record how the evidence was transferred, imaged, analyzed, and handled during the investigation.

## Skills Demonstrated

- Forensic evidence acquisition
- Forensic image creation
- Hash verification
- Evidence integrity validation
- Disk image analysis
- File signature analysis
- Password recovery
- File carving
- Embedded file extraction
- Evidence handling
- Chain-of-custody documentation
- Multi-tool forensic workflows

## Key Takeaway

One of the main lessons from this investigation was that no single forensic tool is sufficient for every stage of an investigation.

Combining specialized tools made it possible to perform deeper analysis, recover protected information, identify file manipulation, and extract embedded evidence.

## Report

[View the full Digital Forensics Investigation Report](./Digital_Forensics_Investigation_Report.pdf)

## Disclaimer

This investigation was conducted entirely within an authorized educational lab environment using simulated forensic evidence.

No real-world systems or unauthorized data were accessed.
