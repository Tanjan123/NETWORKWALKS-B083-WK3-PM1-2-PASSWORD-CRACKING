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

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Tools & Resources](#-tools--resources)
- [Module 01 — John the Ripper](#-module-01--password-cracking-with-john-the-ripper)
  - [Task Overview](#task-overview)
  - [JtR Installation](#1-john-the-ripper-installation)
  - [Johnny Configuration](#2-johnny-gui-configuration)
  - [PDF Hash Extraction](#3-pdf-hash-extraction)
  - [Password Cracking](#4-password-cracking)
  - [Results](#5-results)
- [Module 02 — Networkwalks Tools](#-module-02--networkwalks-password-cracking-tools)
  - [Hash Calculator](#1-hash-calculation)
  - [Password Cracker](#2-password-cracking)
  - [PDF Verification](#3-pdf-decryption)
- [Results Summary](#-results-summary)
- [Key Learning Outcomes](#-key-learning-outcomes)
- [Security Notes](#-security-notes)
- [Evidence](#-evidence)
- [Author](#-author)
- [Project Information](#-project-information)

---

## 📌 Project Overview

**Week 03** focused on practical **password-cracking and hash-analysis techniques** using John the Ripper, Johnny GUI, and Networkwalks-provided password-cracking tools.

The exercises were performed against the **provided password-protected PDF training files** as part of the Networkwalks cybersecurity program.

---

## 🎯 Objectives

The main objectives of this week's practical work were:

- Understand password-protected PDF files and their hashes.
- Extract PDF password hashes.
- Use **John the Ripper** to perform password recovery.
- Configure and use the **Johnny GUI**.
- Verify recovered passwords against encrypted PDF files.
- Use the **Networkwalks Hash Calculator**.
- Use the **Networkwalks Password Cracker**.
- Understand the importance of password complexity and attack strategies.

---

# 🔐 Module 01 — Password Cracking with John the Ripper

## Task Overview

**Task:** Crack the passwords of the provided encrypted PDF files using **John the Ripper** and **Johnny** on a Windows PC.

### Environment

| Item | Details |
|---|---|
| Operating System | Windows |
| Primary Tool | John the Ripper |
| GUI Tool | Johnny |
| Target | Password-protected PDF files |
| Hash Type | PDF password hash |
| Activity Type | Authorized training exercise |

---

## 🛠️ Tools & Resources

### John the Ripper

Official website:

[John the Ripper](https://www.openwall.com/john/)

Official download:

[John the Ripper Downloads](https://distro.ibiblio.org/openwall/projects/john/1.9.0/)

### Johnny

Official resource:

[Johnny GUI](https://openwall.info/wiki/john/johnny)

### PDF Hash Extraction

[Online PDF Hash Extractor](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)

---

## 1. John the Ripper Installation

The official John the Ripper package was downloaded and installed on the Windows PC.

After installation, the `john.exe` executable was located inside the `run` directory.

```text
John the Ripper
└── run
    └── john.exe
