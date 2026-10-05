# Awesome-Local-Administrator-Password-Management

## Top Local Administrator Password Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on LAPS-style Rotation, Local Admin Password Storage, Just-in-Time Elevation & Endpoint Privilege Control*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Local Administrator Password Management**. These solutions automatically rotate, securely store, and control access to local administrator (or root) passwords on Windows, macOS, and other endpoints—reducing the risk of shared or static privileged credentials.



**Examples** include Microsoft Local Administrator Password Solution (LAPS), CyberArk Endpoint Privilege Manager, BeyondTrust Privilege Management, Delinea Privilege Manager, ManageEngine PAM360, Netwrix Password Secure, Thycotic Secret Server, Admin By Request, AutoElevate, and Securden Password Vault (the category leaders).



**Open-source emphasis**: Full-featured commercial PAM and LAPS alternatives dominate this space. Useful open-source and community tools exist—**Lithnet Access Manager**, **macOSLAPS**, serverless LAPS scripts, and general secrets managers that can be adapted. This section expands those while remaining realistic about commercial strength.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Microsoft Local Administrator Password Solution (LAPS)](https://learn.microsoft.com/windows-server/identity/laps/laps-overview)**  

  Microsoft’s built-in solution (now part of Windows) that automatically rotates and stores unique local administrator passwords in Active Directory or Microsoft Entra ID.



- **[CyberArk Endpoint Privilege Manager](https://www.cyberark.com/products/endpoint-privilege-manager/)**  

  Enterprise endpoint privilege management that removes standing local admin rights and provides controlled application elevation alongside credential protection.



- **[BeyondTrust Privilege Management](https://www.beyondtrust.com/privilege-management)**  

  Endpoint and privilege management platform focused on removing local admin rights, controlling elevation, and securing privileged credentials across endpoints.



- **[Delinea Privilege Manager](https://delinea.com/products/privilege-manager)**  

  Privilege elevation and least-privilege solution that helps eliminate standing local administrator rights while allowing approved applications to run elevated.



- **[ManageEngine PAM360](https://www.manageengine.com/privileged-access-management/)**  

  Privileged access management suite that includes password vaulting, rotation, and session management for local and domain privileged accounts.



- **[Netwrix Password Secure](https://www.netwrix.com/)**  

  Password and privileged account management offering focused on secure storage, rotation, and controlled access to sensitive credentials.



- **[Thycotic Secret Server (Delinea)](https://delinea.com/products/secret-server)**  

  Established privileged account password vault and management platform widely used for storing and rotating local and service account credentials.



- **[Admin By Request](https://www.adminbyrequest.com/)**  

  Just-in-time privilege elevation solution that allows users to request temporary admin rights with approval workflows and full auditing.



- **[AutoElevate](https://autoelevate.com/)**  

  Endpoint privilege management focused on removing local admin rights and providing policy-based application elevation for Windows environments.



- **[Securden Password Vault](https://www.securden.com/)**  

  Privileged password management and vaulting solution that supports secure storage, rotation, and access control for local administrator and other privileged accounts.



## Open-Source GitHub Projects

- **[Lithnet Access Manager](https://github.com/lithnet/access-manager)**  

  Open-source (free Standard edition) web-based tool for securely retrieving Microsoft LAPS passwords, BitLocker recovery keys, and granting just-in-time admin access.



- **[macOSLAPS](https://github.com/joshua-d-miller/macoslaps)**  

  Open-source tool that rotates local administrator passwords on macOS in a manner similar to Microsoft LAPS, storing the new password in a directory or secure location.



- **[SLAPS – Serverless Local Administrator Password Solution](https://github.com/jseerden/SLAPS)**  

  Community PowerShell-based approach for rotating local admin passwords and storing them in Azure Key Vault using a serverless model.



- **[Microsoft LAPS (legacy & community tooling)](https://www.microsoft.com/)**  

  While the modern Windows LAPS is built into the OS, community scripts and management tools continue to extend and automate LAPS workflows.



- **[General open-source secrets managers adapted for LAPS use cases](https://github.com/hashicorp/vault)**  

  Tools such as Vault, OpenBao, Infisical, or Bitwarden that can store and control access to rotated local administrator passwords when integrated with custom rotation scripts.



- **[PowerShell and automation scripts for local admin rotation](https://github.com/)**  

  Community repositories containing scripts that generate random local admin passwords, update accounts, and push values to Active Directory or a secrets store.



- **[Documentation and LAPS / Lithnet deployment guides](https://github.com/lithnet/access-manager)**  

  Resources for deploying web portals for LAPS password retrieval and just-in-time access in Active Directory environments.



- **[Just-in-time elevation experiments and open PAM prototypes](https://github.com/)**  

  Emerging community projects exploring open approaches to temporary privilege elevation and local admin control.



- **[Active Directory and Entra ID integration helpers](https://github.com/)**  

  Scripts and tools that help manage LAPS attributes, permissions, and reporting in directory environments.



- **[Cross-platform local privilege management experiments](https://github.com/)**  

  Early-stage open efforts targeting consistent local admin password handling across Windows, macOS, and Linux.



### Additional Strong Open-Source Options

- Using **Lithnet Access Manager** as a modern web front-end for Microsoft LAPS.

- Deploying **macOSLAPS** for consistent local admin rotation on Apple endpoints.

- Building custom rotation pipelines with PowerShell + Azure Key Vault or an open secrets manager.

- Accepting that full endpoint privilege management (application control, policy-based elevation, broad OS support, and enterprise support) remains the domain of commercial platforms (CyberArk, BeyondTrust, Delinea, Admin By Request, AutoElevate, etc.).

- Focusing open-source efforts on password retrieval portals, rotation scripts, and integration with existing directory and secrets infrastructure.



**Frameworks for building custom systems**: Enable Windows LAPS or macOSLAPS → store passwords in AD/Entra or a secrets vault → expose controlled access via Lithnet Access Manager or custom portal → add just-in-time elevation where possible. Suitable for organizations already invested in Microsoft ecosystems. Larger or multi-OS environments typically adopt commercial privilege management platforms.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- Local administrator password management is security-critical. Incorrect configuration can lock out administrators or expose privileged credentials. Open-source tools require careful testing and operational expertise. This list is not security architecture advice.



---

**Made for Windows/macOS administrators, identity teams, and security engineers.**

Let's keep local privileged credentials rotated, controlled, and as open as practical.
