# Azure-ID_GovernanceProject-
Simulating User Lock out and Password Reset using Azure VM Windows Server 
Project Overview

Objective: Provision a cloud-based Windows Server environment to simulate a corporate enterprise network, demonstrating proficiency in Azure networking, remote server management, and Active Directory user lifecycle administration.

Tech Stack: Microsoft Azure, Windows Server 2022, Active Directory Domain Services (AD DS), macOS Microsoft Remote Desktop.

Phase 1: Cloud Infrastructure & Secure Access

Scenario: Engineering the foundational server environment and establishing secure remote administration from a macOS host.

Execution: Deployed a Windows Server 2022 virtual machine via the Azure Portal. Configured the Network Security Group (NSG) to explicitly allow inbound RDP traffic (TCP 3389) while blocking unauthorized external access. Connected to the server using the native macOS Microsoft Remote Desktop client.

Screenshot: The Azure Portal dashboard showing your running VM alongside the active NSG inbound port rules.

Phase 2: Active Directory Provisioning

Scenario: Transforming a standalone server into an enterprise domain controller to manage company identities.

Execution: Utilized Windows Server Manager to install the Active Directory Domain Services (AD DS) role and promoted the server to a primary Domain Controller. Built out a logical Organizational Unit (OU) structure to mimic corporate departments (e.g., HR, Engineering) and provisioned standard user accounts.

Screenshot: The Active Directory Users and Computers (ADUC) console displaying your domain tree, custom OUs, and a newly created test user.

Phase 3: Tier 1 Help Desk Operations

Scenario: Resolving a simulated user lockout request utilizing standard IT operating procedures.

Execution: Located the affected user account within the ADUC console. Executed a secure password reset utilizing a complex temporary credential, and mandated a forced password change upon the user's next login to maintain security compliance.

Screenshot: The ADUC password reset dialog box showing the temporary password entered and the "User must change password at next logon" checkbox selected.
