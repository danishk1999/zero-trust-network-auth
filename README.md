# 🔐 Zero Trust Network Authentication
**Course:** CMPT 480 — Computer Network Security  
**Date:** August 2024  
**Client:** Universal Rail Systems (Work Integrated Learning Project)  
**Status:** ✅ Completed  
**Team:** Aidan Mark, Danish Kumar, Mohammad Mohammad, Mahmoud Modo

## Overview
Designed and implemented a Zero Trust Architecture (ZTA) for a real-world client 
— Universal Rail Systems — as part of a work-integrated learning project. The 
solution enforces the principle of "never trust, always verify" across all users, 
devices, and traffic within the client's network.

## My Contributions
- Designed the network topology and virtual infrastructure layout
- Configured Proxmox VE virtualization environment and VyOS router
- Set up Active Directory (AD) Domain Controller and Certificate Authority (CA)
- Implemented mTLS authentication across servers
- Documented configuration steps and security recommendations

## Technologies Used
- Proxmox VE (Virtualization)
- VyOS Router
- Windows Server 2022
- Active Directory & Certificate Authority (AD CS)
- Mutual TLS (mTLS)
- IIS Reverse Proxy
- SQL Server with forced encryption
- Remote Desktop Protocol (RDP) with certificate-based auth
- VLAN Segmentation & Firewall Rules
- IPSec

## Architecture Highlights
- **Network Topology:** Segmented internal network (192.168.1.0/24) with DMZ
- **4 Virtualized Servers:** Active Directory, File/Print Server, SQL Server, Application Server
- **Certificate-Based Auth:** Enterprise Root CA issues certs to all domain-joined devices
- **Zero Trust Principles Applied:** Least privilege, micro-segmentation, continuous monitoring, MFA

## Key Security Implementations
- Mutual TLS (mTLS) for all server-to-server communication
- Role-Based Access Control (RBAC) via Active Directory
- VLAN isolation for printers and DMZ
- Firewall rules restricting traffic to essential ports only
- Secure RDP with Group Policy hardening
- IPSec encryption between network segments

## 📄 Report
The full project report is included in this repository

## Note
This project was completed in a controlled lab environment using virtualized 
infrastructure. No real client data or production systems are included in this repository.
