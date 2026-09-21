<h1 align="center">🔐 Networkwalks Cybersecurity — Week 03</h1>

<div align="center">

### Password Cracking & Hash Analysis Lab

**John the Ripper (JtR) • Johnny • Networkwalks Password Cracker**

</div>

<p align="center">

<img src="https://img.shields.io/badge/Program-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
<img src="https://img.shields.io/badge/Batch-B083-0070C0?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Week-03%20Final-238F89?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/John%20the%20Ripper-Password%20Cracking-C00000?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Johnny-GUI-404040?style=flat-square&labelColor=0070C0" />
<img src="https://img.shields.io/badge/Hash%20Analysis-Lab-238F89?style=flat-square&labelColor=000000" />
<img src="https://img.shields.io/badge/Authorized-Training%20Lab-C00000?style=flat-square&labelColor=000000" />

</p>

---

## 📖 Table of Contents

* [Project Overview](#-project-overview)
* [Objectives](#-objectives)
* [Tools & Resources](#-tools--resources)
* [Module 01 — John the Ripper](#-module-01--password-cracking-with-john-the-ripper)

  * [Task Overview](#task-overview)
  * [John the Ripper Installation](#1-john-the-ripper-installation)
  * [Johnny GUI Configuration](#2-johnny-gui-configuration)
  * [PDF Hash Extraction](#3-pdf-hash-extraction)
  * [Password Cracking](#4-password-cracking)
  * [Results](#5-results)
* [Module 02 — Networkwalks Password Cracking Tools](#-module-02--networkwalks-password-cracking-tools)

  * [Hash Calculation](#1-hash-calculation)
  * [Password Cracking](#2-password-cracking)
  * [PDF Decryption](#3-pdf-decryption)
* [Results Summary](#-results-summary)
* [Key Learning Outcomes](#-key-learning-outcomes)
* [Security Notes](#-security-notes)
* [Evidence](#-evidence)
* [Author](#-author)
* [Project Information](#-project-information)

---

## 📌 Project Overview

**Week 03** focused on practical **password-cracking and hash-analysis techniques** using John the Ripper, Johnny GUI, and Networkwalks-provided password-cracking tools.

The exercises were performed against the **provided password-protected PDF training files** as part of the Networkwalks cybersecurity program.

The practical workflow covered the complete process from **PDF hash extraction → hash analysis → password recovery → PDF decryption and verification**.

---

## 🎯 Objectives

The main objectives of this week's practical work were:

* Understand password-protected PDF files and their associated hashes.
* Extract password hashes from encrypted PDF files.
* Use **John the Ripper (JtR)** for password recovery.
* Configure and use the **Johnny GUI**.
* Verify recovered passwords against encrypted PDF files.
* Use the **Networkwalks Hash Calculator**.
* Use the **Networkwalks Password Cracker**.
* Understand password-cracking workflows and attack concepts.
* Understand the importance of password complexity.
* Document practical password-security testing activities.

---

## 🛠️ Tools & Resources

### John the Ripper

**Official Website:**
https://www.openwall.com/john/

**Official Download:**
https://distro.ibiblio.org/openwall/projects/john/1.9.0/

### Johnny

**Official Resource:**
https://openwall.info/wiki/john/johnny

### PDF Hash Extraction

**Online PDF Hash Extractor:**
https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php

### Networkwalks Tools

**Hash Calculator:**
https://networkwalks.com/hash-calculator/

**Password Cracker:**
https://networkwalks.com/password-cracker/

---

# 🔐 Module 01 — Password Cracking with John the Ripper

## Task Overview

The first module focused on recovering passwords from the provided encrypted PDF training files using **John the Ripper** and its graphical interface, **Johnny**.

### Environment

| Item                 | Details                      |
| -------------------- | ---------------------------- |
| **Operating System** | Windows                      |
| **Primary Tool**     | John the Ripper              |
| **GUI Tool**         | Johnny                       |
| **Target**           | Password-protected PDF files |
| **Hash Type**        | PDF password hash            |
| **Activity Type**    | Authorized training exercise |

---

## 1. John the Ripper Installation

The official John the Ripper package was downloaded and installed on the Windows PC.

After installation, the `john.exe` executable was located inside the `run` directory.

### Installation Structure

```text
John the Ripper
└── run
    └── john.exe
```

The `run` directory contains the executable and supporting files required to perform password-recovery operations.

### Verification

The installation was verified by locating the `john.exe` executable and preparing it for use with Johnny.

---

## 2. Johnny GUI Configuration

**Johnny** was installed and configured to use the John the Ripper executable.

### Configuration Steps

1. Open **Johnny**.
2. Open **Settings**.
3. Select **Browse**.
4. Locate the John the Ripper installation directory.
5. Navigate to the `run` directory.
6. Select `john.exe`.
7. Save the configuration.

### Configuration Flow

```text
Johnny GUI
    ↓
Settings
    ↓
Browse
    ↓
John the Ripper
    ↓
run/
    ↓
john.exe
    ↓
Save Configuration
```

---

## 3. PDF Hash Extraction

The provided encrypted PDF file was processed using a PDF hash extraction tool.

The generated hash began with the PDF hash identifier:

```text
$pdf$
```

The complete extracted hash was copied and saved into a text file named:

```text
hash1.txt
```

### Hash Extraction Workflow

```text
Encrypted PDF
      ↓
PDF Hash Extractor
      ↓
$pdf$... Hash
      ↓
hash1.txt
      ↓
Johnny / John the Ripper
      ↓
Recovered Password
      ↓
Decrypted PDF
```

### Hash File

```text
hash1.txt
```

The hash file was then used as the input for the password-recovery process.

---

## 4. Password Cracking

The extracted PDF hash was loaded into Johnny for password recovery.

### Procedure

1. Open **Johnny**.
2. Select **Open password file**.
3. Select `hash1.txt`.
4. Load the hash file.
5. Select **Start new attack**.
6. Allow the password-recovery process to run.
7. Monitor the cracking process.
8. Obtain the recovered password.
9. Use the recovered password to open the encrypted PDF.
10. Verify successful decryption.

### Attack Workflow

```text
hash1.txt
    ↓
Johnny
    ↓
Load Hash
    ↓
Start New Attack
    ↓
Password Recovery
    ↓
Recovered Password
    ↓
PDF Decryption
    ↓
Verification
```

---

## 5. Results

### PDF 01

The first provided PDF was successfully decrypted.

**Result:**

```text
Password recovered successfully
PDF decrypted successfully
```

**Training Flag:**

```text
nw{networkwalks_flag1_jtr_270521_1}
```

---

### PDF 02

The second provided PDF was successfully decrypted.

The same password was applicable because the PDF contained the same hash.

**Training Flag:**

```text
nw{networkwalks_persistence_jtr_270521}
```

---

### PDF 03

A separate PDF hash was extracted and saved as:

```text
hash3.txt
```

The password recovered through John the Ripper was:

```text
1qaz2wsx
```

The decrypted PDF contained the following training flag:

```text
nw{networkwalks_flag_260821_1}
```

---

# 🌐 Module 02 — Networkwalks Password Cracking Tools

## Task Overview

The second module focused on using the **Networkwalks Hash Calculator** and **Networkwalks Password Cracker** to process the provided encrypted PDF file.

The workflow involved extracting the PDF password hash, submitting the hash to the password-cracking tool, and verifying the recovered password against the encrypted document.

---

## 1. Hash Calculation

The Networkwalks Hash Calculator was opened:

https://networkwalks.com/hash-calculator/

The provided locked PDF was uploaded to the tool.

The tool generated a PDF password hash beginning with:

```text
$pdf$
```

The complete hash was copied for use in the next stage.

### Workflow

```text
Locked PDF
    ↓
Networkwalks Hash Calculator
    ↓
$pdf$... Hash
    ↓
Copy Complete Hash
```

---

## 2. Password Cracking

The Networkwalks Password Cracker was opened:

https://networkwalks.com/password-cracker/

The extracted PDF hash was pasted into the Password Cracker.

The password-recovery process was then started to identify the corresponding password.

### Workflow

```text
$pdf$... Hash
      ↓
Networkwalks Password Cracker
      ↓
Password Recovery
      ↓
Recovered Password
```

---

## 3. PDF Decryption

After obtaining the recovered password, it was entered into the locked PDF to verify whether the document could be successfully decrypted.

### Verification Workflow

```text
Recovered Password
        ↓
    Locked PDF
        ↓
Password Accepted
        ↓
Successful Decryption
```

> **Note:** The available Module 02 notes do not include the final recovered password or flag. Therefore, no additional result is claimed for this section.

---

# 📊 Results Summary

| Module    | Tool                          | Activity                    | Result             |
| --------- | ----------------------------- | --------------------------- | ------------------ |
| Module 01 | John the Ripper               | PDF password recovery       | Successful         |
| Module 01 | Johnny                        | GUI-based password recovery | Successful         |
| Module 01 | JtR                           | PDF 01                      | Password recovered |
| Module 01 | JtR                           | PDF 02                      | Password recovered |
| Module 01 | JtR                           | PDF 03                      | Password recovered |
| Module 02 | Networkwalks Hash Calculator  | PDF hash extraction         | Completed          |
| Module 02 | Networkwalks Password Cracker | Password recovery           | Performed          |
| Module 02 | PDF Reader                    | Password verification       | Performed          |

---

# 🧠 Key Learning Outcomes

Through this week's practical work, I gained hands-on experience with:

* PDF password hash extraction.
* Understanding PDF password hashes beginning with `$pdf$`.
* John the Ripper password-recovery workflows.
* Johnny GUI configuration and usage.
* Hash-based password recovery.
* Password attack workflows.
* Password complexity concepts.
* Web-based hash calculation.
* Networkwalks password-cracking tools.
* Verification of recovered credentials against encrypted documents.
* Practical cybersecurity lab documentation.
* Maintaining evidence of security-testing activities.

---

# 🔒 Security Notes

Password-cracking techniques can be used for legitimate security testing as well as unauthorized access.

All activities documented in this project were performed against the **provided training files** within the assigned Networkwalks cybersecurity lab.

No unauthorized accounts, systems, or third-party files were targeted.

The techniques documented here should only be used against systems and files for which appropriate authorization has been provided.

---

# 📸 Evidence

Screenshots and supporting evidence should be stored inside the repository's `evidence/` directory.

### Recommended Evidence Structure

```text
evidence/
├── 01-john-installation.png
├── 02-johnny-configuration.png
├── 03-pdf-hash-extraction.png
├── 04-hash1-file.png
├── 05-johnny-cracking-process.png
├── 06-pdf01-decryption.png
├── 07-pdf02-decryption.png
├── 08-pdf03-hash.png
├── 09-pdf03-password-recovery.png
├── 10-networkwalks-hash-calculator.png
├── 11-networkwalks-password-cracker.png
└── 12-pdf-decryption-verification.png
```

### Evidence Index

| No. | Evidence                         |
| --: | -------------------------------- |
|  01 | John the Ripper installation     |
|  02 | Johnny configuration             |
|  03 | PDF hash extraction              |
|  04 | `hash1.txt` configuration        |
|  05 | Johnny password-cracking process |
|  06 | First PDF decrypted              |
|  07 | Second PDF decrypted             |
|  08 | Third PDF hash                   |
|  09 | Third PDF password recovery      |
|  10 | Networkwalks Hash Calculator     |
|  11 | Networkwalks Password Cracker    |
|  12 | PDF decryption verification      |

### Evidence Example

Replace the placeholders below with your actual screenshots:

```md
### 01 — John the Ripper Installation

![John the Ripper Installation](evidence/01-john-installation.png)

### 02 — Johnny Configuration

![Johnny Configuration](evidence/02-johnny-configuration.png)

### 03 — PDF Hash Extraction

![PDF Hash Extraction](evidence/03-pdf-hash-extraction.png)
```

> **Evidence Hygiene:** Avoid uploading unnecessary sensitive information, personal credentials, real passwords, private keys, tokens, or unrelated system information to the repository.

---

# 👤 Author

<div align="center">

### Tanjan Singh Karki

**Cybersecurity Trainee | B083**

**Networkwalks Cybersecurity Program**

</div>

---

# 📌 Project Information

<div align="center">

| Information       | Details                                                           |
| ----------------- | ----------------------------------------------------------------- |
| **Program**       | Cybersecurity Program at Networkwalks                             |
| **Batch**         | B083                                                              |
| **Week**          | 03                                                                |
| **Modules**       | Password Cracking with JtR + Networkwalks Password Cracking Tools |
| **Project Area**  | Password Security, Hash Extraction & Password Cracking            |
| **Documentation** | GitHub Markdown                                                   |

</div>

---

<h2 align="center">— End —</h2>

<div align="center">

**Networkwalks Cybersecurity Program — Batch B083**

**Week 03 — Password Cracking & Hash Analysis Lab**

</div>
