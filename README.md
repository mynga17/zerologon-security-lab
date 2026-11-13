![CVE](https://img.shields.io/badge/CVE-2020--1472-red)
![Windows Server](https://img.shields.io/badge/Windows-Server-0078D4)
![Active Directory](https://img.shields.io/badge/Active_Directory-AD-4472C4)
![Netlogon](https://img.shields.io/badge/Netlogon-Security-blue)
![VMware](https://img.shields.io/badge/VMware-Lab-607078)


# 🔐 Zerologon Security Lab

A practical cybersecurity lab focused on analyzing and demonstrating the Zerologon vulnerability (CVE-2020-1472) in a controlled Active Directory environment.

The project explores the security risks associated with the Netlogon Remote Protocol and demonstrates a mitigation approach by enabling Netlogon Domain Controller Enforcement Mode.

---

## Table of Contents

- [Overview](#overview)
- [Project Objectives](#project-objectives)
- [Vulnerability Background](#vulnerability-background)
- [Lab Environment](#lab-environment)
- [Attack Demonstration](#attack-demonstration)
- [Mitigation and Prevention](#mitigation-and-prevention)
- [Video Demonstrations](#video-demonstrations)
- [Documentation](#documentation)
- [Disclaimer](#disclaimer)
---
<a id="overview"></a>
## 📌 Overview

Zerologon (CVE-2020-1472) is a critical vulnerability affecting Microsoft's Netlogon Remote Protocol. It can potentially allow an unauthenticated attacker with network access to a vulnerable Domain Controller to compromise domain security.

This project was developed as part of my Information Security studies to gain practical experience in Windows infrastructure security, vulnerability analysis, and security mitigation.

The lab covers two main activities:

- **Attack Demonstration:** Exploring the Zerologon vulnerability and its potential impact on Active Directory.
- **Mitigation Demonstration:** Enabling Netlogon Domain Controller Enforcement Mode and examining the resulting security behavior.

<a id="project-objectives"></a>
## ✨ Project Objectives

- Understand the technical background of Zerologon (CVE-2020-1472).
- Explore the security risks associated with the Netlogon Remote Protocol.
- Understand the role of Netlogon in Active Directory environments.
- Perform practical vulnerability testing in an isolated lab.
- Enable Netlogon Domain Controller Enforcement Mode.
- Examine the effectiveness of the implemented security configuration.

<a id="vulnerability-background"></a>
## 🔍 Vulnerability Background

Zerologon is a vulnerability in the Netlogon Remote Protocol caused by a weakness in its cryptographic authentication process.

The vulnerability can allow an unauthenticated attacker with network access to a vulnerable Domain Controller to impersonate a computer account and potentially gain control over the Active Directory domain.

Due to its potential impact, CVE-2020-1472 is considered a critical security vulnerability affecting Windows Server environments.

<a id="lab-environment"></a>
## 🖥️ Lab Environment

The experiment was conducted in a virtualized environment using VMware.

### Technologies & Components

| Category | Technologies |
|---|---|
| Virtualization | VMware Workstation |
| Server Platform | Windows Server |
| Directory Services | Active Directory Domain Services (AD DS) |
| Authentication Protocol | Netlogon Remote Protocol |
| Security Configuration | Netlogon Domain Controller Enforcement Mode |

*The virtual machines and complete lab environment are not included in this repository.*

<a id="attack-demonstration"></a>
## ⚔️ Attack Demonstration

The attack phase focuses on demonstrating the Zerologon vulnerability in a controlled Active Directory environment.

The experiment explores weaknesses in the Netlogon authentication process and illustrates the potential security impact on a vulnerable Domain Controller.

The demonstration is intended to provide practical insight into the risks associated with CVE-2020-1472.

<a id="mitigation-and-prevention"></a>
## 🔐 Mitigation and Prevention

### Netlogon Domain Controller Enforcement Mode

Netlogon Domain Controller Enforcement Mode was enabled as the primary mitigation measure in this lab.

This security configuration enforces stronger requirements for Netlogon secure channel connections and rejects vulnerable connection attempts that do not meet the required security conditions, subject to Microsoft's documented exceptions.

### Verification

The mitigation demonstration focuses on enabling Enforcement Mode and examining the security behavior under the updated configuration.

The practical verification process is documented in the accompanying demonstration video and project report.

<a id="video-demonstrations"></a>
## 🎬 Video Demonstrations

The following videos document the practical attack and mitigation experiments.

### 🔴 Zerologon Attack

Demonstrates the Zerologon vulnerability and its potential impact on an Active Directory environment.

**[▶ Watch Attack Demonstration](https://youtu.be/fu-3iuyvTM4)**

### 🟢 Zerologon Mitigation

Demonstrates enabling Netlogon Domain Controller Enforcement Mode and examining the resulting security behavior.

**[▶ Watch Mitigation Demonstration](https://youtu.be/KoYGaK_RSSE)**

<a id="documentation"></a>
## 📄 Documentation

The accompanying project report provides further details about the lab environment, vulnerability analysis, attack demonstration, experimental observations, and mitigation process.

- [Zerologon Demo Report](Zerologon_Demo_Report.pdf)

<a id="disclaimer"></a>
## ⚠️ Disclaimer

This project was conducted in an isolated virtual lab environment for educational and cybersecurity research purposes.

All testing activities were performed on systems under the project's control. No unauthorized systems or networks were targeted.
