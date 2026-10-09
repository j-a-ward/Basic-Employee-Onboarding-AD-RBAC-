# Basic Employee Onboarding (AD) (RBAC)

## Problem Statement
Northstar Medical Group (fictional company) hired a managed service provider (MSP) to handle its access management. The MSP set up a flat, unsegmented Active Directory infrastructure without standardized role-based access control (RBAC). As the organization grew to more than 200 user accounts, the lack of fine-grained access controls led to extensive overprovisioning and violations of the principle of least privilege (PoLP). In addition, the absence of automated deprovisioning workflows left accounts active after employees departed. Unmonitored access pathways and stale accounts increased the company’s risk of noncompliance with the HIPAA Security Rule.

## Solution Overview
To address these access control flaws, I designed and implemented a new Active Directory domain with an organizational unit (OU) hierarchy aligned with the company’s functional divisions. I created specialized security groups within the OUs to implement role-based access control (RBAC) consistent with the principle of least privilege (PoLP). By mapping permissions to job responsibilities and operational requirements, I limited each user’s access to what their role required. This structured approach removed unapproved access pathways, standardized user provisioning, and reduced overprovisioning and directory sprawl. The remediation also addressed the security risks posed by orphaned accounts and strengthened compliance with the HIPAA Security Rule.

## Video Walkthrough
[Add your video walkthrough link placeholder here. You will record this tomorrow and update this link so visitors can see a live demonstration of your lab environment.]

## Tools and Methodologies
* Windows Server
* Active Directory Domain Services (AD DS)
* Oracle VM VirtualBox
* Principle of Least Privilege (PoLP)
* Role-Based Access Control (RBAC)
* Linux (Bodhi Linux / Ubuntu LTS)

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Designed department-based OU structure (Finance, HR, IT, Operations)
* Implemented RBAC with security groups mapped to each department
* Provisioned 15 user accounts with consistent naming conventions and attribute standards
* Diagnosed and resolved a multi-cause access issue (wrong OU + missing group membership)
* Documented full incident resolution with root cause analysis

