# Awesome-API-Authentication-Credential-Management

# Awesome-API-Authentication-Credential-Management

**Top API Authentication Credential Management (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Secrets Sprawl, Dynamic Credentials, AI Agent Identity & Self-Hosted Vaults*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **API Authentication & Credential Management**. These tools enable organizations to store, rotate, inject, and audit the secrets that applications and AI agents use to authenticate—API keys, OAuth tokens, database passwords, and certificates—without exposing plaintext in code, logs, or agent contexts.



The global **secrets management solutions market** was valued at **USD 2.43 billion in 2025** and is projected to reach **USD 7.86 billion by 2034** at a **14.1% CAGR** . **API keys and tokens** are the fastest-growing secret type at a **17.88% CAGR** , driven by the explosion of machine identities and agentic AI workloads .



**Examples** include HashiCorp Vault, AWS Secrets Manager, Azure Key Vault, Google Secret Manager, CyberArk, Doppler, 1Password, Okta, Auth0, and Postman (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted secrets management, dynamic credentials, and open credential infrastructure. **Critical note**: The open-source landscape is anchored by **HashiCorp Vault Community Edition**—free and self-hosted, covering KV storage, dynamic secrets, transit encryption, and a wide range of auth methods—but it lacks enterprise features like namespaces, disaster recovery, performance replication, and HSM support . No open-source project matches CyberArk's privileged access depth or AWS Secrets Manager's managed rotation integrations, but for core secret storage and dynamic credential generation, Vault Community is production-capable.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## Sector Overview & Market Dynamics

The global secrets management market is estimated at **$2.43 billion in 2025** and is projected to reach **$7.86 billion by 2034 at a 14.1% CAGR**, driven by a 17.88% surge in non-human API keys and machine identities. The sector is **moderately fragmented yet increasingly bifurcated**: hyperscalers (AWS, Azure, GCP) command native baseline storage, while enterprise privileged access and multi-cloud dynamic secrets management are concentrating around market leaders like CyberArk, HashiCorp/IBM, and specialized developer platforms.



## SaaS/Hosted Platforms

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



## Open-Source GitHub Projects

- **HashiCorp Vault** [![GitHub stars](https://img.shields.io/github/stars/hashicorp/vault?style=social&color=white)](https://github.com/hashicorp/vault/stargazers)
  - **Description**: The most mature open-source secrets engine (MPL 2.0 / BSL), free and self-hosted. Provides KV storage, dynamic secrets for databases and clouds, transit encryption-as-a-service, and PKI certificate authority.
  - **Tech Stack**: Go | **Deploy**: Binary, Docker, Kubernetes

- **Infisical** [![GitHub stars](https://img.shields.io/github/stars/Infisical/infisical?style=social&color=white)](https://github.com/Infisical/infisical/stargazers)
  - **Description**: Modern end-to-end secrets management platform (MIT / Business Source) with an intuitive web dashboard, secret scanning, dynamic secrets, Kubernetes operator, SDKs, and AI agent credential security.
  - **Tech Stack**: Node.js, TypeScript, PostgreSQL | **Deploy**: Self-hosted (Docker) or Infisical Cloud

- **SOPS (Secrets OPerationS)** [![GitHub stars](https://img.shields.io/github/stars/getsops/sops?style=social&color=white)](https://github.com/getsops/sops/stargazers)
  - **Description**: Simple, flexible editor for encrypted files (YAML, JSON, ENV, INI, binary) supporting AWS KMS, GCP KMS, Azure Key Vault, HashiCorp Vault, and age/PGP keys for GitOps workflows.
  - **Tech Stack**: Go | **Deploy**: CLI tool, CI/CD integration

- **Teleport** [![GitHub stars](https://img.shields.io/github/stars/gravitational/teleport?style=social&color=white)](https://github.com/gravitational/teleport/stargazers)
  - **Description**: Identity-native infrastructure access management providing zero-trust credential issuance, short-lived certificates, and session recording for SSH, Kubernetes, databases, and internal web applications.
  - **Tech Stack**: Go | **Deploy**: Self-hosted cluster, Teleport Cloud

- **Bitwarden Server** [![GitHub stars](https://img.shields.io/github/stars/bitwarden/server?style=social&color=white)](https://github.com/bitwarden/server/stargazers)
  - **Description**: Open-source backend infrastructure for Bitwarden Password Manager and Bitwarden Secrets Manager, offering programmatic secret retrieval, CLI access, and developer SDKs.
  - **Tech Stack**: C#, .NET, Docker | **Deploy**: Self-hosted (Docker Compose)

- **Git-crypt** [![GitHub stars](https://img.shields.io/github/stars/AGWA/git-crypt?style=social&color=white)](https://github.com/AGWA/git-crypt/stargazers)
  - **Description**: Transparent encryption of sensitive files in Git repositories. Keeps repository contents readable while automatically encrypting selected files when committed and decrypting when checked out.
  - **Tech Stack**: C++ | **Deploy**: CLI tool, Git filter

- **OpenBao** [![GitHub stars](https://img.shields.io/github/stars/openbao/openbao?style=social&color=white)](https://github.com/openbao/openbao/stargazers)
  - **Description**: Community-governed, truly open-source fork of HashiCorp Vault maintained under the OpenSSF (Linux Foundation) to ensure continuous open-source API-compatible secrets management under MPL-2.0.
  - **Tech Stack**: Go | **Deploy**: Binary, Docker, Kubernetes

- **External Secrets Operator** [![GitHub stars](https://img.shields.io/github/stars/external-secrets/external-secrets?style=social&color=white)](https://github.com/external-secrets/external-secrets/stargazers)
  - **Description**: Kubernetes operator that synchronizes credentials from external APIs and vaults (AWS Secrets Manager, HashiCorp Vault, Azure Key Vault, GCP Secret Manager, Infisical) directly into Kubernetes native Secrets.
  - **Tech Stack**: Go | **Deploy**: Kubernetes Operator (Helm)

- **Square Keywhiz** [![GitHub stars](https://img.shields.io/github/stars/square/keywhiz?style=social&color=white)](https://github.com/square/keywhiz/stargazers)
  - **Description**: Systems architecture designed by Square for distributing and managing secrets, certificates, and keys securely to servers and microservices with mutual TLS (mTLS).
  - **Tech Stack**: Java | **Deploy**: Self-hosted service

- **Lyft Confidant** [![GitHub stars](https://img.shields.io/github/stars/lyft/confidant?style=social&color=white)](https://github.com/lyft/confidant/stargazers)
  - **Description**: Secrets management service developed by Lyft that uses AWS KMS and DynamoDB for end-to-end encrypted storage, user-friendly UI, and IAM-based authentication.
  - **Tech Stack**: Python, AngularJS, AWS KMS | **Deploy**: Self-hosted AWS deployment

- **Pinterest Knox** [![GitHub stars](https://img.shields.io/github/stars/pinterest/knox?style=social&color=white)](https://github.com/pinterest/knox/stargazers)
  - **Description**: High-performance secret management service built by Pinterest for storing, rotating, and distributing cryptographic keys and access tokens with strict audit trails.
  - **Tech Stack**: Go | **Deploy**: Self-hosted service

- **AthenZ** [![GitHub stars](https://img.shields.io/github/stars/AthenZ/athenz?style=social&color=white)](https://github.com/AthenZ/athenz/stargazers)
  - **Description**: Fine-grained role-based access control (RBAC) and dynamic X.509 certificate provisioning system for machine identities, service-to-service authentication, and short-lived tokens in dynamic cloud environments.
  - **Tech Stack**: Java, Go | **Deploy**: Self-hosted (Docker, Kubernetes)

- **CyberArk Conjur** [![GitHub stars](https://img.shields.io/github/stars/cyberark/conjur?style=social&color=white)](https://github.com/cyberark/conjur/stargazers)
  - **Description**: Security platform specifically designed for DevOps and cloud-native application environments to authenticate, authorize, and control machine identities and secrets.
  - **Tech Stack**: Ruby, Go | **Deploy**: Docker, Kubernetes

- **Keygate** [![GitHub stars](https://img.shields.io/github/stars/tabloy/keygate?style=social&color=white)](https://github.com/tabloy/keygate/stargazers)
  - **Description**: Open-source license and API credential enforcement platform supporting subscriptions, floating licenses, offline tokens, atomic quota enforcement, and Stripe integration.
  - **Tech Stack**: Go, SQLite/PostgreSQL | **Deploy**: Single binary, Docker



### Additional Strong Open-Source Options



- **No mature open-source equivalent to AWS Secrets Manager's managed rotation or CyberArk's privileged access depth exists.** Vault Community and OpenBao cover core secrets management; Infisical covers modern UI and platform features. For managed rotation of cloud-native credentials, commercial cloud services remain necessary.



**Frameworks for building custom systems**: Choose **HashiCorp Vault Community** for the most battle-tested secrets engine, **OpenBao** for a community-governed fork with API compatibility, and **Infisical** for a modern UI-driven platform. **None match AWS Secrets Manager's native rotation integrations or CyberArk's privileged access controls.**



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Credential management platforms handling secrets and API keys must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate encryption, access controls, and audit logging. **A secrets management platform is only as secure as its configuration**—misconfigured vaults are a primary breach vector.

- **The "managed secrets service" vs. "self-hosted vault" vs. "identity platform" vs. "license enforcement" distinction is critical.** **AWS Secrets Manager, Azure Key Vault, and Google Secret Manager** are **managed secrets services**—they provide storage and (for supported integrations) rotation without infrastructure . **HashiCorp Vault, OpenBao, and Infisical** are **self-hosted vaults/platforms**—they provide the engine, but you own operations . **Okta and Auth0** are **identity platforms**—they manage authentication and tokens, not arbitrary secrets. **Keygate** is **license enforcement**—it manages product license keys, not API credentials. **Choose based on whether you need managed convenience, self-hosted control, identity governance, or license activation.**

- **HashiCorp Vault's Community Edition is genuinely free but missing key enterprise features.** No namespaces, disaster recovery, performance replication, Sentinel policies, or HSM support—and no SLA . **For production at scale, HCP Vault Dedicated or Enterprise is required.**

- **AWS Secrets Manager's $0.40/secret/month is only worth it if you use managed rotation.** For third-party API keys from non-partner companies, you pay for a feature you cannot use—Parameter Store's SecureString may be sufficient at $0 for storage . **Choose per-secret, not per-organization.**

- **Doppler's per-seat pricing is developer-friendly but grows fast.** **$21/user/month on Team** for a 20-person team is **$5,040/year**—and it lacks dynamic credentials and HSM support . **For teams wanting dynamic secrets, Vault Community is the free alternative.**

- **Google Secret Manager's free tier is genuinely usable**—6 active versions and 10,000 access operations per month . **For small GCP projects, it may cost nothing.**

- **CyberArk is being acquired by Palo Alto Networks**, expected to close in Q3 of PANW's fiscal 2026 . **Evaluate roadmap continuity before committing.**

- Self-hosted open-source solutions require proper infrastructure (Go for Vault/OpenBao/Keygate, Node.js for Infisical), security hardening, and ongoing maintenance. **Secrets management platforms are high-value targets**—ensure your deployment meets your organization's security and compliance requirements before storing production credentials.



---



**Made for security engineers, platform teams, and organizations building transparent credential management solutions.**

Let's make API Authentication & Credential Management more open, data-driven, and secret-safe.
