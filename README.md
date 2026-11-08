# Awesome-User-Identity-Access-Administration

# Awesome User Identity & Access Administration

> A curated list of top User Identity and Access Administration platforms — both SaaS/Hosted commercial solutions and open-source alternatives for managing user identities, roles, permissions, and access governance.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [Okta](#okta)
  - [Microsoft Entra ID](#microsoft-entra-id)
  - [Ping Identity](#ping-identity)
  - [JumpCloud](#jumpcloud)
  - [OneLogin](#onelogin)
  - [Auth0](#auth0)
  - [CyberArk](#cyberark)
  - [SailPoint](#sailpoint)
  - [Google Workspace Admin](#google-workspace-admin)
- [Open-Source Software](#-open-source-software)
  - [Keycloak](#keycloak)
  - [Casdoor](#casdoor)
  - [Hanzo IAM](#hanzo-iam)
  - [Ory](#ory)
  - [Zitadel](#zitadel)
  - [Authentik](#authentik)
  - [WSO2 Identity Server](#wso2-identity-server)
  - [Apache Syncope](#apache-syncope)
  - [Evolveum midPoint](#evolveum-midpoint)
  - [Nubus](#nubus)
  - [Thand Agent](#thand-agent)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted User Identity and Access Administration platforms. These are not open-source but are included as reference points for feature comparison.

### Okta
**Type:** Enterprise identity and access management  
Okta is the most widely adopted vendor-neutral identity platform, offering SSO, MFA, lifecycle management, and user administration across thousands of integrations. Strengths include neutrality across productivity suites and a mature provisioning engine. Features are sold as separate products, so total cost rises significantly beyond base SSO.

### Microsoft Entra ID
**Type:** Identity platform within Microsoft 365  
Entra ID is the default choice for Microsoft-centric organizations, providing user administration, authentication, Conditional Access, and integration with the broader Microsoft security stack. Basic SSO to third-party apps is included with Microsoft 365 at no extra charge.

### Ping Identity
**Type:** Enterprise federation and identity orchestration  
Ping Identity (including PingFederate, PingOne, and ForgeRock) is built for complex estates with multiple directories, on-premises and cloud apps, legacy protocols, and strict compliance requirements. Strengths include federation depth and deployment flexibility. Heavier implementation effort and quote-based pricing.

### JumpCloud
**Type:** Cloud directory with device management  
JumpCloud combines cloud directory, SSO, MFA, LDAP/RADIUS, and cross-OS device management in a single console. It is a common replacement for on-premises Active Directory in small and mid-sized companies.

### OneLogin
**Type:** IAM with directory integration  
OneLogin (part of One Identity) offers SSO, MFA, directory integration, and user provisioning with a straightforward admin experience. Simpler than the largest suites, with a smaller integration ecosystem than Okta or Entra ID.

### Auth0
**Type:** Developer-focused identity platform  
Auth0 is widely used for application authentication and user administration, with strong SDKs, extensibility, and support for social login, enterprise SSO, and RBAC. Pricing can escalate with identity provider connections and advanced features.

### CyberArk
**Type:** Privileged access management (PAM)  
CyberArk focuses on privileged user administration, credential vaulting, session isolation, and least-privilege enforcement for administrative accounts. A critical component of user access administration for high-risk accounts, often integrated alongside Okta or Entra ID.

### SailPoint
**Type:** Enterprise identity security and governance  
SailPoint's platform covers identity governance, access certifications, role management, and policy enforcement across enterprise applications. It ensures that access is granted, reviewed, and revoked according to policy.

### Google Workspace Admin
**Type:** Directory administration for Google-first organizations  
Google Workspace Admin provides user lifecycle management, admin role assignment, and directory controls through the Admin console and Directory API. Suited for organizations standardized on Google's productivity suite.

---

## 🟩 Open-Source Software

Self-hosted, community-driven User Identity and Access Administration platforms. All listed projects offer source code you can deploy on your own infrastructure.

### Keycloak
**Stack:** Java | **License:** Apache-2.0  
The most widely deployed open-source identity server, supporting OIDC, SAML, social login, identity brokering, and MFA. Keycloak is the most mature self-hosted option, with a large community and extensive documentation. It supports user federation, role-based access control, and fine-grained authorization [citation:7].  
**Best for:** Organizations wanting a proven, battle-tested identity foundation with broad protocol support.

### Casdoor
**Stack:** Go / React | **License:** Apache-2.0  
An open-source IAM and SSO platform with a web admin console. Supports OAuth 2.0, OIDC, SAML, CAS, LDAP, and RADIUS. Ships with more than 70 OAuth providers built in. Features include WebAuthn/passkeys, TOTP, MFA, organizations with per-tenant branding, and authorization built on Casbin (ACL, RBAC, ABAC). Deploys as one Go binary with a choice of databases [citation:7].  
**Best for:** Teams wanting a single-binary, feature-rich IAM with broad provider support and Apache-2.0 licensing throughout.

### Hanzo IAM
**Stack:** Go | **License:** Apache-2.0  
An AI-first IAM and MCP gateway/auth server with web UI. Supports OAuth 2.1, OIDC, SAML, CAS, LDAP, SCIM, WebAuthn, TOTP, MFA, and 40+ social login providers. Features RBAC, multi-tenancy, API-first design, and SCIM provisioning for automated user lifecycle management. Deploys via Docker [citation:3].  
**Best for:** Teams wanting a modern, Go-based IAM with AI/MCP integration and broad protocol support.

### Ory
**Stack:** Go | **License:** Apache-2.0  
A modular ecosystem of cloud-native identity servers. Components include Ory Kratos (identity and authentication), Ory Hydra (OAuth2/OIDC), Ory Keto (permissions), and Ory Polis (enterprise SSO). Each service works standalone, so you can adopt a single component or combine them into a full IAM stack.  
**Best for:** Teams wanting a modular, composable IAM stack they can adopt incrementally and fully control.

### Zitadel
**Stack:** Go | **License:** AGPL-3.0  
A cloud-native identity platform with a focus on multi-tenancy and self-service. Provides OIDC, SAML, MFA, passwordless, and user management with a modern API-first design. Comparable to Keycloak and Auth0, with a growing community [citation:7].  
**Best for:** Teams wanting a cloud-native, multi-tenant identity platform with modern APIs.

### Authentik
**Stack:** Python (Django) / Go | **License:** MIT (core)  
An open-source identity provider with a flexible flow-based model for login logic. Supports OIDC, SAML, LDAP, and proxy authentication. The core is MIT-licensed, with some features reserved for the paid Enterprise edition. Has the most flexible sign-in flow engine among open-source options [citation:7].  
**Best for:** Teams wanting highly customizable login flows and proxy-based app protection.

### WSO2 Identity Server
**Stack:** Java | **License:** Apache-2.0  
A Digital Public Good-recognized open-source IAM solution supporting OAuth2, OIDC, SAML, SCIM 2.0, and FIDO2. Features include adaptive MFA, RBAC, SSO, identity federation, social login, and user management. Used in 93 countries across finance, public administration, healthcare, and education [citation:12].  
**Best for:** Organizations wanting a comprehensive, standards-based IAM platform with a proven track record in regulated sectors.

### Apache Syncope
**Stack:** Java | **License:** Apache-2.0  
An open-source IAM and IGA platform for managing digital identities, provisioning, authentication, and access control. Supports user/group/role management, automated provisioning workflows, RBAC, delegated administration, LDAP/AD/database connectors, SAML 2.0, OIDC, and SCIM. Includes audit logging and compliance reporting.  
**Best for:** Organizations seeking a standards-based, Apache-governed IGA platform with strong connector support.

### Evolveum midPoint
**Stack:** Java | **License:** Open Source (subscription model)  
A comprehensive open-source Identity Governance and Administration (IGA) platform with automated provisioning/deprovisioning, policy-based approvals, segregation of duties controls, access certification campaigns, and role mining. Subscription-based with no license fees — pay only for support.  
**Best for:** Organizations needing full IGA with lifecycle automation and governance controls without per-identity licensing costs.

### Nubus
**Stack:** (Check repository) | **License:** AGPL-3.0-or-later  
A modular open-source IAM solution for centralized management of user identities, roles, permissions, and application access via a central web portal. Integrated SSO, self-service password changes, and user lifecycle management. Supports Kubernetes, on-premises, and hybrid deployment. Used by ZenDiS GmbH, Orange S.A., and several German state education ministries [citation:8].  
**Best for:** European organizations prioritizing digital sovereignty and open standards, with commercial support options.

### Thand Agent
**Stack:** Go | **License:** BSL 1.1  
A distributed open-source agent for privileged access management (PAM) and just-in-time (JIT) access to cloud infrastructure, SaaS applications, and local systems. Eliminates standing access by granting temporary permissions on request, with complete audit trails and automatic revocation. Uses Serverless Workflows and Temporal for deterministic execution [citation:4].  
**Best for:** Security teams wanting to eliminate standing privileges and implement JIT access with a self-hostable agent.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Self-Hosted | JIT/PAM | Best For |
|----------|---------|-------|-------------|---------|----------|
| **Okta** | Proprietary | Cloud | ❌ | ❌ | Enterprise workforce + CIAM |
| **Microsoft Entra ID** | Proprietary | Cloud | ❌ | ❌ | Microsoft 365 organizations |
| **Ping Identity** | Proprietary | Cloud/on-prem | (Enterprise) | ❌ | Complex federation |
| **JumpCloud** | Proprietary | Cloud | ❌ | ❌ | SMB cloud directory |
| **OneLogin** | Proprietary | Cloud | ❌ | ❌ | Simpler IAM |
| **Auth0** | Proprietary | Cloud | ❌ | ❌ | Developer application auth |
| **CyberArk** | Proprietary | Cloud/on-prem | (Enterprise) | ✅ PAM | Privileged access |
| **SailPoint** | Proprietary | Cloud | ❌ | ❌ | Identity governance |
| **Keycloak** | Apache-2.0 | Java | ✅ | ❌ | Proven OSS foundation |
| **Casdoor** | Apache-2.0 | Go/React | ✅ | ❌ | Single-binary + 70+ providers |
| **Hanzo IAM** | Apache-2.0 | Go | ✅ | ❌ | AI-first IAM + MCP |
| **Ory** | Apache-2.0 | Go | ✅ | ❌ | Modular composable IAM |
| **Zitadel** | AGPL-3.0 | Go | ✅ | ❌ | Cloud-native multi-tenancy |
| **Authentik** | MIT (core) | Python/Go | ✅ | ❌ | Flexible flow-based login |
| **WSO2 IS** | Apache-2.0 | Java | ✅ | ❌ | Standards-based IAM |
| **Apache Syncope** | Apache-2.0 | Java | ✅ | ❌ | Standards-based IGA |
| **midPoint** | Open Source | Java | ✅ | ❌ | Full governance without license fees |
| **Nubus** | AGPL-3.0 | (Check) | ✅ | ❌ | European sovereignty |
| **Thand Agent** | BSL 1.1 | Go | ✅ | ✅ JIT | Zero standing privileges |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source User Identity or Access Administration platform that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note the license if source-available but not OSI-approved, as with Thand Agent's BSL).

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
