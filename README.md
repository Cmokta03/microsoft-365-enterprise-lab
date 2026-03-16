# Microsoft 365 Enterprise Administration Lab

## Overview
This project demonstrates hands-on implementation of Microsoft 365 enterprise services including identity management, device management, collaboration tools and security compliance.

The lab simulates a small enterprise environment using Microsoft 365 services.

## Technologies Used

- Microsoft Entra ID
- Microsoft Intune
- Microsoft 365 Admin Center
- Exchange Online
- SharePoint Online
- Microsoft Teams
- Microsoft Defender
- Microsoft Purview

## Project Phases

### Phase 1 – Identity & Access (Entra ID)
- User creation
- Security groups
- License assignment
- Multi-Factor Authentication
- Conditional Access

### Phase 2 – Microsoft 365 Admin Setup
- Tenant configuration
- Admin roles
- Service configuration

### Phase 3 – Endpoint Management (Intune)
- Windows device enrollment
- iPhone enrollment
- Win32 application deployment
- BitLocker policy
- Attack Surface Reduction rules

### Phase 4 – Collaboration Services
- SharePoint site creation
- OneDrive configuration
- Microsoft Teams collaboration

### Phase 5 – Security & Compliance
- Microsoft Defender policies
- Data Loss Prevention
- eDiscovery cases

## Skills Demonstrated

- Cloud Identity Management
- Endpoint Security
- Enterprise Collaboration
- Microsoft 365 Administration
- Security & Compliance


## 🛠 Phase 1: Identity & Access Management (Entra ID)
In this phase, I built the identity foundation. I configured a custom domain, managed user lifecycles, and verified cloud identity integration.

### What I Accomplished:
* **Domain Setup:** Added and verified a custom domain for a corporate identity.
* **User Management:** Created bulk users via CSV and manual admin accounts (John Support).
* **Licensing:** Assigned M365 Business Premium/E5 licenses to active users.
* **Device Join:** Successfully performed an **Entra ID Join** for a Windows 11 VM.

### Phase 1 Proof:
![Phase 1 Proof](screenshots%20(Phase1)/11_Entra_ID_Join_Confirmation.png)
---
## 📱 Phase 2: Endpoint Management & Security (Intune)

In this phase, I moved beyond identity to manage and secure Windows 11 and iOS endpoints. I focused on security baselines, disk encryption, and automated software deployment.

### Key Achievements:
* **Endpoint Security:** Implemented **BitLocker** encryption and **Attack Surface Reduction (ASR)** policies.
* **Compliance & Access:** Configured **Conditional Access** policies to ensure only compliant devices can access corporate resources.
* **Win32 App Packaging:** Successfully packaged and deployed .exe/msi applications (7-Zip) using the **Intune Win32 Content Prep Tool**.
* **Mobile Management (MAM):** Deployed business applications (Teams) to mobile devices via the Company Portal.

### Phase 2 Evidence:
![Intune Enrollment Success](Screenshots_Phase2/01_Windows_Intune_Enrollment.png)
![BitLocker Verification](Screenshots_Phase2/09_BitLocker_PowerShell_Verification.png)

---
## 📧 Phase 3: Messaging & Collaboration (Exchange Online)

In this phase, I configured the enterprise email environment, focusing on mail flow security, resource management, and administrative auditing.

### Key Technical Achievements:
* **Mail Flow Management:** Created **Transport Rules** to apply "External Email" warning tags to prevent phishing.
* **Shared Resources:** Configured **Shared Mailboxes** and **Room/Resource Mailboxes** with proper delegation (Full Access/Send As).
* **Security & Compliance:** Implemented **Anti-Spam policies** and performed **Message Traces** to troubleshoot delivery issues.
* **Automation:** Developed **Dynamic Distribution Groups** to automate membership based on user attributes.
* **Modern Scheduling:** Deployed **Microsoft Bookings** for automated appointment scheduling.

### Phase 3 Evidence:
![Message Trace Proof](Screenshots_Phase3/16_Exchange_Message_Trace_Troubleshooting.png)
![Transport Rule Verification](Screenshots_Phase3/13_Transport_Rule_Verification.png)

---
## 🏗️ Phase 4: SharePoint Online & Content Governance

In this phase, I designed a SharePoint architecture focused on internal communication, collaboration, and strict document lifecycle management.

### Key Technical Achievements:
* **Site Architecture:** Deployed **Team Sites** for departmental collaboration and **Communication Sites** for company-wide news.
* **Hub Site Integration:** Registered sites as **Hub Sites** to centralize navigation and search across the tenant.
* **Security & Permissions:** Implemented **Granular Access Control**, successfully verifying "Access Denied" scenarios for unauthorized users (e.g., John).
* **Compliance Workflow:** Configured **Document Versioning** and **Content Approval** workflows to ensure document integrity and administrative oversight.

### Phase 4 Evidence:
![SharePoint Permissions](Screenshots_Phase4/06_Permission_Verification_Access_Denied.png)
![Versioning Workflow](Screenshots_Phase4/09_Content_Approval_Workflow_Success.png)

---
## ☁️ Phase 5: Cloud Storage Governance (OneDrive & SharePoint)

In this phase, I implemented data governance and security controls for cloud storage to prevent data leakage and manage tenant resources.

### Key Technical Achievements:
* **Sync Governance:** Restricted OneDrive sync to specific joined domains and blocked unauthorized file types (.exe) from cloud synchronization.
* **Storage Optimization:** Configured **Storage Quotas** to manage tenant capacity and ensure fair resource distribution.
* **Data Retention:** Implemented **Retention Policies** to meet compliance requirements for data preservation.
* **Sharing Security:** Configured **External Sharing** settings to restrict guest access and enforce corporate data boundaries.
* **Administrative Delegation:** Performed delegated access procedures to manage user-specific storage for auditing purposes.

### Phase 5 Evidence:
![Sync Block Proof](Screenshots_Phase5/02_File_Extension_Sync_Block_EXE.png)
![Sharing Governance](Screenshots_Phase5/03_SharePoint_External_Sharing_Governance.png)

---
## 🛡️ Phase 6: Endpoint Security & Response (Microsoft Defender for Endpoint)

In this final advanced phase, I configured a full Security Operations (SecOps) environment to detect, investigate, and respond to advanced threats.

### Key Technical Achievements:
* **Endpoint Detection & Response (EDR):** Onboarded Windows endpoints to **Defender for Endpoint** and monitored device health/exposure scores.
* **Threat & Vulnerability Management (TVM):** Performed software inventory audits and initiated remediation requests for high-risk vulnerabilities.
* **Active Incident Response:** Demonstrated containment capabilities by performing **Device Isolation** to stop lateral movement during a simulated breach.
* **Automated Investigation (AIR):** Leveraged XDR capabilities to manage automated forensic investigations and remediation.
* **Network Security:** Implemented **Web Content Filtering** to block high-risk domains and enforced host-based Firewall policies.

### Phase 6 Evidence:
![Device Isolation Proof](Screenshots_Phase6/10_Device_Isolation_Network_Block_Verification.png)
![Vulnerability Assessment](Screenshots_Phase6/06_Threat_and_Vulnerability_Management_Inventory.png)
