# Azure Cloud Security Implementation Project

## Objective
The objective of this project is to transition SWBTL LLC’s IT infrastructure to a secure Azure cloud environment, addressing the current security challenges, ensuring regulatory compliance, and enhancing overall security posture. 

## Skills Learned
- Azure IaaS implementation
- Role-Based Access Control (RBAC) configuration
- Azure Key Vault management
- Data encryption techniques
- Backup and recovery configuration
- Compliance management in cloud environments

## Tools Used
- Microsoft Azure Portal
- Azure Active Directory (AAD)
- Azure Key Vault
- Azure Security Center
- Azure Backup and Recovery Services

## Executive Summary
SWBTL LLC has faced growing security challenges due to outdated infrastructure and the departure of a key IT consultant. These issues have led to improper access controls, inadequate backup verification, and a lack of security scanning for over two years. This project proposes a secure Azure IaaS cloud solution, designed to address these challenges, ensure compliance with FISMA and PCI DSS standards, and improve the company’s overall security posture.

## Proposed Course of Action
### Service Model Identification
The **Infrastructure as a Service (IaaS)** model is chosen to provide SWBTL LLC with control over operating systems, storage, and deployed applications while leveraging Azure’s infrastructure.

### Regulatory Compliance
The project ensures compliance with:
- **FISMA**: Monitoring and managing the security of government information systems.
- **PCI DSS**: Encrypting card transaction data in transit and at rest.

### Security Benefits and Challenges
**Benefits:**
- Enhanced security with tools like Azure AD, Azure Firewall, and Azure Monitor.
- Scalability to support SWBTL LLC’s growth.
- Comprehensive compliance support with Azure’s built-in tools.

**Challenges:**
- Addressing skill gaps in cloud security knowledge.
- Managing data sovereignty and privacy across different jurisdictions.
- Ensuring a seamless transition without service disruption.

## Implementation Steps

### 1. Role-Based Access Control (RBAC) Configuration
RBAC settings were configured to align with the principle of least privilege:
- **IT Resource Group**: Assigned the "Contributor" role.
- **Marketing Resource Group**: Assigned the "Contributor" role.
- **Accounting Resource Group**: Assigned the "Contributor" role.

**Screenshot of RBAC Configuration:**
![RBAC Configuration Screenshot](https://github.com/user-attachments/assets/36acb32d-2921-43a0-b4ad-4ffc4223810a)


### 2. Azure Key Vault Implementation
Best practices were applied for managing encryption keys:
- Segregation of Key Vaults by department.
- Enforcement of strict access policies.

**Screenshot of Azure Key Vault Setup:**
![Azure Key Vault Configuration Screenshot](https://github.com/user-attachments/assets/39500df5-fb61-4ab3-82c7-70d8cf543273)


### 3. File Backup Configuration
To meet business requirements, file backups were configured with:
- Daily backups scheduled at 7 p.m. Eastern Time.
- Retention of recovery snapshots for 3 days and daily backups for 45 days.

**Screenshot of Backup Configuration:**
![Backup Configuration Screenshot](https://github.com/user-attachments/assets/8b995676-64f8-4da2-9e31-fe10b7facc2b)

## Division of Responsibilities
In the IaaS model:
- **Azure**: Responsible for infrastructure security, host security, and managed services security.
- **SWBTL LLC**: Responsible for data security, application security, network security, and access management.

**Shared Responsibilities:**
Compliance adherence between Azure’s infrastructure and SWBTL LLC’s service configurations.

## Threats and Mitigation Strategies
### 1. Data Breaches and Leaks
**Mitigation:** Encrypt data in transit and at rest using Azure Key Vault, implement strict access controls, and utilize Azure Security Center for continuous monitoring.

### 2. Account Hijacking
**Mitigation:** Implement Multi-Factor Authentication (MFA), enforce regular password changes, and monitor user activities through Azure tools.

### 3. Distributed Denial of Service (DDoS) Attacks
**Mitigation:** Utilize Azure’s DDoS Protection services, implement load balancing, and have an incident response plan in place.

## Conclusion
This project ensures a secure transition of SWBTL LLC’s IT infrastructure to the Azure cloud environment, addressing current security challenges, ensuring regulatory compliance, and improving the company's overall security posture.

**References:**
- Microsoft Azure Documentation
- Center for Internet Security Guidelines


