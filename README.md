# 🏢 Enterprise Windows Server Infrastructure Lab

<p align="center">

![Windows Server](https://img.shields.io/badge/Windows%20Server-2019-blue?style=for-the-badge&logo=windows)
![Active Directory](https://img.shields.io/badge/Active%20Directory-Implemented-success?style=for-the-badge)
![DNS](https://img.shields.io/badge/DNS-Configured-green?style=for-the-badge)
![DHCP](https://img.shields.io/badge/DHCP-Failover-orange?style=for-the-badge)
![VPN](https://img.shields.io/badge/VPN-RRAS-red?style=for-the-badge)
![File Server](https://img.shields.io/badge/File%20Server-Deployed-blueviolet?style=for-the-badge)

</p>

---

## 📖 Overview

This project demonstrates the deployment of a complete **Enterprise Windows Server Infrastructure** designed to simulate a real-world corporate environment.

The infrastructure includes:

✅ Active Directory Domain Services (AD DS)

✅ DNS Server

✅ VPN Server (RRAS)

✅ File Server

✅ DHCP Failover Cluster

✅ Group Policy Management

✅ Folder Redirection

✅ Drive Mapping

✅ Access Control & Security Policies

The project focuses on centralized administration, secure remote connectivity, high availability, and enterprise-level user management.

---

## 🎯 Project Objectives

- 🏢 Build an Enterprise Network Environment
- 🔐 Implement Secure Authentication
- 🌐 Configure VPN Remote Access
- 📂 Centralize File Storage
- 👥 Manage Users & Organizational Units
- ⚙️ Apply Group Policy Objects (GPO)
- 📡 Configure DHCP Failover
- 🛡️ Enforce Security Policies
- 🔄 Provide High Availability Services

---

## 🖥️ Infrastructure Diagram

| Device | IP Address |
|----------|------------|
| 🏢 Domain Controller + DNS + VPN | 192.168.2.2 |
| 📂 File Server | 192.168.2.6 |
| 💻 PC1 (Domain Joined) | 192.168.2.7 |
| 🌍 PC2 (External Client) | 41.0.0.3 |
| 🔐 VPN External Interface | 41.0.0.2 |

---

## 🏢 Active Directory Structure

### 📁 Sales OU

👤 Alumed

👤 Wael

### 📁 HR Manager OU

👤 Mohamed

👤 Karim

#### 📁 HR Sub-OU

👤 Maged

---

## 🔐 Security Policies

### Password Policy

✔️ Minimum Password Length: 10 Characters

✔️ Password Complexity Enabled

✔️ Minimum Password Age: 7 Days

✔️ Maximum Password Age: 72 Days

✔️ Password History Disabled

---

## ⚙️ Group Policy Configuration

- 🚫 Hide Desktop Icons
- 🚫 Disable DVD Access
- 🚫 Disable Right Click on PC1
- 🔒 Apply Password Policies
- 🖥️ User Environment Restrictions

---

## 📂 File Server Configuration

### Shared Folders

#### 📁 Sales

Access Granted To:

- 👤 Alumed
- 👤 Mohamed

#### 📁 HR

Access Granted To:

- 👤 Wael
- 👤 Karim

---

## 🔄 Folder Redirection

Documents folder redirected to:

```text
\\FileServer\Desktop\Documents
