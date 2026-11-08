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



- **HashiCorp Vault (Community Edition)**

  **Open-source secrets management** (MPL 2.0) — **the most mature open-source secrets engine**, free and self-hosted . **Features**: **KV secrets storage**; **dynamic secrets** for databases, cloud providers, and SSH; **transit encryption-as-a-service**; **PKI certificate management**; **identity-based access** with a wide range of auth methods (LDAP, OIDC, Kubernetes, AppRole, and more); **audit devices** for every request. **Tech stack**: Go. **Deploy**: Self-hosted (binary, Docker, Kubernetes). **Trade-off**: **Community Edition lacks enterprise features**—no namespaces, disaster recovery, performance replication, Sentinel policies, or HSM support; no SLA and community-only support . **Best for**: teams wanting a proven, self-hosted secrets engine with dynamic credentials and PKI—willing to accept the operational burden and missing enterprise features.



- **Infisical**

  **Open-source secrets management platform** (open source) — **the most modern open-source Vault alternative**, with a developer-friendly UI and platform approach. **Features**: **Secrets management** across environments and projects; **secret scanning**; **PKI**; **SSH access**; **dynamic secrets**; **AI agent integration**; developer-first CLI and SDKs. **Tech stack**: Node.js, TypeScript, PostgreSQL. **Deploy**: Self-hosted (Docker) or Infisical Cloud. **Trade-off**: **Newer than Vault**—smaller ecosystem and less battle-tested at enterprise scale; some features gated to paid tiers. **Best for**: teams wanting a modern, UI-driven secrets platform they can self-host—especially those migrating from Vault or Doppler.



- **OpenBao**

  **Open-source fork of HashiCorp Vault** (MPL 2.0) — **the community-governed continuation of Vault** after HashiCorp's license change to BUSL. **Features**: **API-compatible with Vault**—drop-in replacement for existing Vault deployments; **community-driven roadmap** under the OpenSSF (Open Source Security Foundation); retains Vault's secrets engines, auth methods, and audit capabilities. **Tech stack**: Go. **Deploy**: Self-hosted (binary, Docker, Kubernetes). **Trade-off**: **Fork maturity**—newer governance and roadmap; evaluate enterprise feature parity before migrating production Vault. **Best for**: organizations that want Vault's capabilities under a truly open-source, community-governed license—especially those concerned about BUSL restrictions.



- **Keygate**

  **Open-source software license management platform** (open source) — **the most purpose-built open-source license enforcement platform**, positioned as a self-hosted Keygen alternative. **Features**: **Every licensing model**—subscriptions, perpetual, trials, and floating licenses; **per-device or per-user activation limits** with atomic enforcement; **license keys hashed with SHA-256**; **signed tokens for offline verification**; **seats and entitlements**; **API Providers** for atomic quota enforcement; **Stripe integration**. **Tech stack**: Go. **Deploy**: Self-hosted. **Trade-off**: **v0.1.18**—newer project with limited validation; license enforcement, not a full secrets vault. **Best for**: SaaS and software vendors selling licensed products needing activation limits and entitlement enforcement—not general-purpose API credential storage.



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
