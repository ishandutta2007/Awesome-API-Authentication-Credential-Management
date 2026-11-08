<div align="center">

<img src="./assets/banner.svg" alt="Awesome API Authentication &amp; Credential Management Banner" width="100%" />

# Awesome API Authentication & Credential Management 🔐

**A curated index of top-tier Secrets Management SaaS platforms, Self-Hosted Vaults, Dynamic Credential Brokers, and Open-Source Security Engines.**

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a>
  <a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-API-Authentication-Credential-Management/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-API-Authentication-Credential-Management?style=social" alt="Stars" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-API-Authentication-Credential-Management/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-API-Authentication-Credential-Management?style=social" alt="Forks" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-API-Authentication-Credential-Management/issues"><img src="https://img.shields.io/github/issues/ishandutta2007/Awesome-API-Authentication-Credential-Management?color=green" alt="Issues" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-API-Authentication-Credential-Management/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License" /></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

*Defend against secrets sprawl, govern non-human machine identities, automate OAuth & API tokens, and secure agentic AI workflows.* 🚀

**Last updated: November 2026**

</div>

---

## 📌 Table of Contents

- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS / Hosted Platforms](#️-saas--hosted-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
- [🤝 How to Contribute](#-how-to-contribute)
- [💖 Support](#-support)
- [📈 Star History](#-star-history)
- [⚠️ Disclaimer](#️-disclaimer)

---

## 🌐 Sector Overview & Market Dynamics

The global **secrets management solutions market** was valued at **USD 2.43 billion in 2025** and is projected to reach **USD 7.86 billion by 2034** at a compound annual growth rate (**CAGR of 14.1%**). Driven by the exponential growth of microservices, cloud infrastructure, and autonomous agentic AI workloads, **API keys and machine tokens** represent the fastest-growing secret type expanding at **17.88% CAGR**.

The market structure is **moderately fragmented yet bifurcated**:
1. **Hyperscaler Baseline Services** (AWS Secrets Manager, Azure Key Vault, Google Secret Manager) dominate platform-native cloud storage and compute-adjacent encryption.
2. **Specialized Multi-Cloud & Enterprise PAM Platforms** (CyberArk, HashiCorp Vault / IBM, Doppler, 1Password) capture complex multi-environment sprawl, just-in-time dynamic secrets, and zero-trust machine-to-machine identity governance.

---

## ☁️ SaaS / Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing | Free Tier / Trial Limits | Key Focus & Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **Microsoft Azure Key Vault** | ~$3.1T Market Cap (Microsoft) | $0.03 per 10,000 operations (keys/secrets/cert operations) | 30-day trial with $200 free Azure credits; free storage (pay only per operation) | Native Azure secrets, keys, and HSM certificate storage. |
| **Google Secret Manager** | ~$2.1T Market Cap (Alphabet) | $0.06 per active secret version/mo + $0.03 per 10,000 operations | Free forever: 6 active secret versions and 10,000 access operations per month | Native GCP secret storage, replication, and audit logging. |
| **AWS Secrets Manager** | ~$2.0T Market Cap (Amazon) | $0.40 per secret per month + $0.05 per 10,000 API calls | 30-day free trial from 1st stored secret; new accounts get up to $200 credits | Managed secrets with native automatic rotation for RDS, Aurora, and Redshift. |
| **CyberArk (Privilege Cloud)** | ~$1.44B ARR / $18.5B Market Cap (Acq. pending PANW) | From ~$125/user/month (~$1,500/user/year list, typically 25-user minimum) | No public self-service free tier; guided 30-day PoC evaluation upon request | Enterprise privileged access management (PAM), dynamic credential brokerage, and compliance. |
| **Okta** | ~$2.6B ARR / ~$15B Market Cap | From $6/user/mo (Starter) to $17/user/mo (Essentials); APIAM add-on ~$2/user/mo (Enterprise custom) | Integrator Free Plan limited to 10 active users; 30-day enterprise trial | Workforce and customer identity governance with API Access Management and OAuth tokens. |
| **Auth0** (by Okta) | Part of Okta (~$2.6B ARR) / $6.5B Acq. Val | B2C from $35/mo (500 MAU); B2B from $150/mo (500 MAU) | Free forever: up to 25,000 MAUs, unlimited social connections, and 1 enterprise connection | Developer-first CIAM/B2B identity platform with token minting and API authorization. |
| **HashiCorp Vault (HCP Vault Dedicated)** | $350M+ ARR / $6.4B Acq. (by IBM) | HCP Vault Essentials from ~$1.58/cluster/hour (~$1,152/mo) + $72.92/client/mo; Standard from ~$1.85/hr | Self-hosted Community Edition is 100% free; HCP Dedicated provides $500 trial credits | Managed Vault clusters with dynamic secrets, PKI engine, and transit encryption. |
| **1Password** | $408M+ ARR / $6.8B Valuation | Business at $7.99/user/month; Starter Pack at $19.95/month (up to 5 users) | 14-day free trial on Business & Teams plans (no credit card required) | Credential management extending to developer CLI, SSH agent, and service accounts. |
| **Postman** | $313M+ ARR / $3.6B–$5.6B Valuation | Basic/Team from $19/user/month (billed annually); Solo paid plans from $14/mo | Free forever: 1 user (solo developer) with unlimited collection runs and mock calls | API collaboration platform managing environment secrets, tokens, and mock auth. |
| **Doppler** | ~$10M–$20M ARR / ~$80M Valuation | Developer tier free (up to 3 seats); Team tier at $8/user/month or $21/user/month | Free forever: up to 3 seats with unlimited projects, environments, and secrets sync | Developer-first secrets sync and orchestration across local envs, CI/CD, and AI agents. |

---

## 💻 Open-Source GitHub Projects

- **HashiCorp Vault** [![GitHub stars](https://img.shields.io/github/stars/hashicorp/vault?style=social&color=white)](https://github.com/hashicorp/vault/stargazers)
  - 📖 **Description**: The most mature open-source secrets engine (MPL 2.0 / BSL), free and self-hosted. Provides KV storage, dynamic secrets for databases and clouds, transit encryption-as-a-service, and PKI certificate authority.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: Binary, Docker, Kubernetes

- **Infisical** [![GitHub stars](https://img.shields.io/github/stars/Infisical/infisical?style=social&color=white)](https://github.com/Infisical/infisical/stargazers)
  - 📖 **Description**: Modern end-to-end secrets management platform (MIT / Business Source) with an intuitive web dashboard, secret scanning, dynamic secrets, Kubernetes operator, SDKs, and AI agent credential security.
  - 🛠️ **Tech Stack**: Node.js, TypeScript, PostgreSQL | 🚀 **Deploy**: Self-hosted (Docker) or Infisical Cloud

- **SOPS (Secrets OPerationS)** [![GitHub stars](https://img.shields.io/github/stars/getsops/sops?style=social&color=white)](https://github.com/getsops/sops/stargazers)
  - 📖 **Description**: Simple, flexible editor for encrypted files (YAML, JSON, ENV, INI, binary) supporting AWS KMS, GCP KMS, Azure Key Vault, HashiCorp Vault, and age/PGP keys for GitOps workflows.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: CLI tool, CI/CD integration

- **Teleport** [![GitHub stars](https://img.shields.io/github/stars/gravitational/teleport?style=social&color=white)](https://github.com/gravitational/teleport/stargazers)
  - 📖 **Description**: Identity-native infrastructure access management providing zero-trust credential issuance, short-lived certificates, and session recording for SSH, Kubernetes, databases, and internal web applications.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: Self-hosted cluster, Teleport Cloud

- **Bitwarden Server** [![GitHub stars](https://img.shields.io/github/stars/bitwarden/server?style=social&color=white)](https://github.com/bitwarden/server/stargazers)
  - 📖 **Description**: Open-source backend infrastructure for Bitwarden Password Manager and Bitwarden Secrets Manager, offering programmatic secret retrieval, CLI access, and developer SDKs.
  - 🛠️ **Tech Stack**: C#, .NET, Docker | 🚀 **Deploy**: Self-hosted (Docker Compose)

- **Git-crypt** [![GitHub stars](https://img.shields.io/github/stars/AGWA/git-crypt?style=social&color=white)](https://github.com/AGWA/git-crypt/stargazers)
  - 📖 **Description**: Transparent encryption of sensitive files in Git repositories. Keeps repository contents readable while automatically encrypting selected files when committed and decrypting when checked out.
  - 🛠️ **Tech Stack**: C++ | 🚀 **Deploy**: CLI tool, Git filter

- **OpenBao** [![GitHub stars](https://img.shields.io/github/stars/openbao/openbao?style=social&color=white)](https://github.com/openbao/openbao/stargazers)
  - 📖 **Description**: Community-governed, truly open-source fork of HashiCorp Vault maintained under the OpenSSF (Linux Foundation) to ensure continuous open-source API-compatible secrets management under MPL-2.0.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: Binary, Docker, Kubernetes

- **External Secrets Operator** [![GitHub stars](https://img.shields.io/github/stars/external-secrets/external-secrets?style=social&color=white)](https://github.com/external-secrets/external-secrets/stargazers)
  - 📖 **Description**: Kubernetes operator that synchronizes credentials from external APIs and vaults (AWS Secrets Manager, HashiCorp Vault, Azure Key Vault, GCP Secret Manager, Infisical) directly into Kubernetes native Secrets.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: Kubernetes Operator (Helm)

- **Square Keywhiz** [![GitHub stars](https://img.shields.io/github/stars/square/keywhiz?style=social&color=white)](https://github.com/square/keywhiz/stargazers)
  - 📖 **Description**: Systems architecture designed by Square for distributing and managing secrets, certificates, and keys securely to servers and microservices with mutual TLS (mTLS).
  - 🛠️ **Tech Stack**: Java | 🚀 **Deploy**: Self-hosted service

- **Lyft Confidant** [![GitHub stars](https://img.shields.io/github/stars/lyft/confidant?style=social&color=white)](https://github.com/lyft/confidant/stargazers)
  - 📖 **Description**: Secrets management service developed by Lyft that uses AWS KMS and DynamoDB for end-to-end encrypted storage, user-friendly UI, and IAM-based authentication.
  - 🛠️ **Tech Stack**: Python, AngularJS, AWS KMS | 🚀 **Deploy**: Self-hosted AWS deployment

- **Pinterest Knox** [![GitHub stars](https://img.shields.io/github/stars/pinterest/knox?style=social&color=white)](https://github.com/pinterest/knox/stargazers)
  - 📖 **Description**: High-performance secret management service built by Pinterest for storing, rotating, and distributing cryptographic keys and access tokens with strict audit trails.
  - 🛠️ **Tech Stack**: Go | 🚀 **Deploy**: Self-hosted service

- **AthenZ** [![GitHub stars](https://img.shields.io/github/stars/AthenZ/athenz?style=social&color=white)](https://github.com/AthenZ/athenz/stargazers)
  - 📖 **Description**: Fine-grained role-based access control (RBAC) and dynamic X.509 certificate provisioning system for machine identities, service-to-service authentication, and short-lived tokens in dynamic cloud environments.
  - 🛠️ **Tech Stack**: Java, Go | 🚀 **Deploy**: Self-hosted (Docker, Kubernetes)

- **CyberArk Conjur** [![GitHub stars](https://img.shields.io/github/stars/cyberark/conjur?style=social&color=white)](https://github.com/cyberark/conjur/stargazers)
  - 📖 **Description**: Security platform specifically designed for DevOps and cloud-native application environments to authenticate, authorize, and control machine identities and secrets.
  - 🛠️ **Tech Stack**: Ruby, Go | 🚀 **Deploy**: Docker, Kubernetes

- **Keygate** [![GitHub stars](https://img.shields.io/github/stars/tabloy/keygate?style=social&color=white)](https://github.com/tabloy/keygate/stargazers)
  - 📖 **Description**: Open-source license and API credential enforcement platform supporting subscriptions, floating licenses, offline tokens, atomic quota enforcement, and Stripe integration.
  - 🛠️ **Tech Stack**: Go, SQLite/PostgreSQL | 🚀 **Deploy**: Single binary, Docker

---

## 🤝 How to Contribute

Contributions are welcome! Help maintain this list as the premier open-source guide for API authentication and credential management:

1. 🍴 Fork this repository.
2. 🌿 Create a feature branch: `git checkout -b add-new-secrets-tool`.
3. 📝 Add or update entries in `README.md` adhering to factual metrics, pricing, and category distinctions.
4. 🚀 Push changes and open a Pull Request with a clear description of the project.

⭐ **Star this repository** if you find it helpful for your infrastructure or security architecture!

---

## 💖 Support

If you find this repository valuable for your engineering projects, platform design, or security audits, please consider supporting the project:

- ⭐ **Star this repo** on GitHub to amplify visibility.
- 🍴 **Fork and contribute** new tools, benchmarks, and updates.
- 📢 **Share with colleagues** on Twitter, LinkedIn, and developer communities.
- ☕ **Buy me a coffee**: Support ongoing curation and maintenance via the [GitHub Sponsors Dashboard](https://github.com/sponsors/ishandutta2007).

---

## 📈 Star History

[![Star History Chart](https://www.star-history.com/svg?repos=ishandutta2007/Awesome-API-Authentication-Credential-Management&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Awesome-API-Authentication-Credential-Management&type=date&legend=top-left)

---

## ⚠️ Disclaimer

- 🛡️ This is a **community-curated directory** intended for informational and architectural guidance—not an endorsement.
- 🔐 Credential management platforms handling secrets and API keys must comply with relevant data protection regulations (GDPR, SOC 2, HIPAA, ISO 27001) and enforce rigorous encryption, role-based access control, and auditing. **A secrets vault is only as secure as its configuration.**
- 🧩 **Managed secrets service vs. Self-hosted vault vs. Identity provider vs. Licensing engine**:
  - **AWS Secrets Manager, Azure Key Vault, Google Secret Manager**: Managed hyperscaler services with zero infrastructure overhead.
  - **HashiCorp Vault, OpenBao, Infisical**: Self-hosted multi-cloud engines offering granular control, dynamic credentials, and zero vendor lock-in.
  - **Okta, Auth0**: Identity platforms specializing in authentication protocols (OAuth 2.0, OIDC, SAML, JWT) rather than raw arbitrary secret storage.
  - **Keygate**: Specialized software licensing platform enforcing activation quotas, not general-purpose API key vaults.
- 🏢 **Corporate Transitions**: Note that CyberArk is under acquisition by Palo Alto Networks, and HashiCorp is under IBM; verify organizational roadmap alignment when designing long-term enterprise systems.

---

<div align="center">

**Built with precision for security engineers, DevOps professionals, and platform teams worldwide.** 🌍

</div>
