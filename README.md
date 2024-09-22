# Describe Azure, Identity, Access, and Security 

## Introduction

In this module, you'll be introduced to Azure identity, access, and security services and tools. The key areas covered include directory services, authentication methods, access control, Zero Trust, defense in depth, and Microsoft Defender for Cloud.

### Learning Objectives

- Describe directory services in Azure, including Entra ID and Microsoft Entra Domain Services.
- Explain authentication methods in Azure, including single sign-on (SSO), multifactor authentication (MFA), and passwordless.
- Discuss external identities and guest access in Azure.
- Describe Microsoft Entra Conditional Access.
- Explain Azure Role Based Access Control (RBAC).
- Understand the concept of Zero Trust.
- Describe the purpose of the defense in depth method.
- Explain the purpose of Microsoft Defender for Cloud.

---

## Describe Azure Directory Services

### Microsoft Entra ID
- **Microsoft Entra ID** is a directory service that enables access to Microsoft cloud apps and services. It can also sync with on-premises Active Directory, providing a unified identity management experience.
- **Key Services**:
  - **Authentication**: Supports self-service password reset, MFA, smart lockout.
  - **Single Sign-On (SSO)**: Allows users to access multiple applications with one set of credentials.
  - **Application Management**: Manage cloud and on-premises apps with features like Application Proxy and SaaS apps.
  - **Device Management**: Register and manage devices through tools like Microsoft Intune.

### Microsoft Entra Domain Services
- Provides domain services like domain join, group policy, LDAP, and Kerberos/NTLM authentication.
- Managed by Azure, so no need to manage domain controllers (DCs) manually.
- Allows integration of legacy applications with modern Azure cloud environments.

---

## Azure Authentication Methods

### Single Sign-On (SSO)
- SSO allows a user to sign in once and access multiple resources across different applications.

### Multifactor Authentication (MFA)
- Adds an extra layer of security by requiring a second form of authentication like a phone call, text message, or app notification.

### Passwordless Authentication
- **Windows Hello for Business**: Uses biometrics or PIN to authenticate users.
- **Microsoft Authenticator App**: Allows authentication without passwords by matching a number on your device.
- **FIDO2 Security Keys**: A hardware-based passwordless solution that uses a USB key for authentication.

---

## Azure External Identities

- **External Identity**: Refers to an identity that is not part of your organization, such as partners or customers.
- **B2B Collaboration**: Enables external users to access your Microsoft apps or custom-developed apps.
- **Azure Active Directory Business to Consumer (B2C)**: Manage customer access to apps while maintaining their credentials.

---


## Azure Conditional Access

- **Conditional Access** is used to enforce access based on signals like location, device, and user behavior.
- Can require MFA or limit access based on the user's context.

---


## Azure Role-Based Access Control (RBAC)

- **RBAC** is used to manage access to Azure resources by assigning roles to users, groups, or services.
- Scope levels include:
  - **Management Group**
  - **Subscription**
  - **Resource Group**
  - **Resource**

---

## Zero Trust Model

- **Zero Trust** is a security model that assumes a breach has already occurred.
- Three main principles:
  1. **Verify Explicitly**: Always authenticate based on data points.
  2. **Use Least Privilege**: Grant only the access necessary.
  3. **Assume Breach**: Always be prepared for a breach.

---


## Defense in Depth

- **Defense in Depth** is a strategy that uses multiple layers of security to protect data and slow down attackers.
  - **Physical Security**: Safeguard hardware in data centers.
  - **Identity and Access**: Control who can access infrastructure and data.
  - **Perimeter**: Protect against network-based attacks.
  - **Network**: Limit communication between resources.
  - **Compute**: Secure virtual machines and endpoints.
  - **Application**: Ensure applications are secure and free from vulnerabilities.
  - **Data**: Control access to sensitive data.

---


## Microsoft Defender for Cloud

- **Defender for Cloud** is a tool for security posture management and threat protection.
- Provides continuous security assessments, tracks vulnerabilities, and detects threats.
- Integrates with Azure services and extends protection to hybrid and multi-cloud environments.

### Key Features:
  - **Azure-Native Protections**: Detect threats across Azure services (App Service, SQL, Storage).
  - **Hybrid and Multi-Cloud Protection**: Extended protection via Azure Arc.
  - **Security Alerts**: Provides detailed remediation steps.
  - **Advanced Threat Protection**: Secures VMs, SQL databases, containers, and web apps.

---


## Knowledge Check

1. **Which Microsoft Entra tool varies credentials needed to log in based on signals, such as location?**
   - **Answer**: Conditional Access

2. **Which security model assumes worst-case security scenarios?**
   - **Answer**: Zero Trust

3. **If a user is assigned multiple roles in RBAC, what are their permissions?**
   - **Answer**: All permissions from all assigned roles.

---


## Summary

In this module, we covered key Azure identity, access, and security services including:
- **Directory services**: Entra ID and Entra Domain Services.
- **Authentication methods**: SSO, MFA, passwordless.
- **Access control**: External identities, Conditional Access, RBAC.
- **Security models**: Zero Trust and Defense in Depth.
- **Microsoft Defender for Cloud**: Security management and threat protection.

---

# Additional Resources

- [Microsoft Certified: Security, Compliance, and Identity Fundamentals](https://learn.microsoft.com/en-us/learn/certifications/security-compliance-and-identity-fundamentals/)
