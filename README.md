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
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **HashiCorp Vault (HCP Vault Dedicated)**
  **Managed secrets management** with dynamic credentials and encryption-as-a-service. **Pricing**: **HCP Vault Dedicated Essentials from ~$1.58/cluster/hour** (~$1,152/month for a small cluster) plus **$72.92/client/month** for each authenticated identity; **Standard from ~$1.85/hour** adds performance replication, Sentinel policies, and secrets sync . **Free tier**: Vault Community Edition is free (self-hosted); HCP offers a **$500 trial credit** . **Best for**: organizations wanting Vault's dynamic secrets and PKI capabilities without operating the control plane—**trade-off**: per-client pricing makes costs unpredictable at scale (every pod, container, and user counts) .

- **AWS Secrets Manager**
  **Managed secrets with native rotation**. **Pricing**: **$0.40 per secret per month** plus **$0.05 per 10,000 API calls** (US pricing; China region shows CNY 2.752/secret and CNY 0.344/10k calls) . **Free tier**: **30-day free trial** from first secret stored; new AWS accounts get up to **$200 in credits** . **Best for**: AWS-centric organizations wanting native RDS/Aurora/Redshift rotation and IAM integration—**trade-off**: rotation only works for supported integration partners; third-party API keys cannot be auto-rotated without a Lambda .

- **CyberArk**
  **Privileged access management** with secrets management and identity security. **Pricing**: Quote-only; enterprise contracts. **Free tier**: None. **Best for**: enterprises needing the deepest privileged access controls and compliance coverage—**trade-off**: enterprise-only; complex deployment. **Note**: CyberArk reported **$1.44B ARR in 2025** (up 23% YoY) and announced a definitive agreement to be acquired by **Palo Alto Networks**, expected to close in Q3 of PANW's fiscal 2026 .

- **Doppler**
  **Developer-friendly secrets management** with per-seat pricing. **Pricing**: **Developer free for 3 users**, then **$8/user/month**; **Team $21/user/month** (14-day free trial); **Enterprise custom**. **AI agents and non-human identities ride free** . **Free tier**: Yes, 3 users. **Best for**: small teams wanting minutes-to-setup secrets management with CI/CD and AI agent integrations—**trade-off**: no dynamic credentials, no HSM support, and per-user pricing grows fast on large teams .

- **Azure Key Vault**
  **Managed secrets, keys, and certificates** within Azure. **Pricing**: Consumption-based; quote-only for full scope. **Free tier**: Limited trial. **Best for**: Microsoft-centric organizations wanting native Azure integration.

- **Google Secret Manager**
  **Managed secrets within Google Cloud**. **Pricing**: **$0.06 per active secret version per month** plus **$0.03 per 10,000 access operations**; **free tier includes 6 active versions and 10,000 access operations per month** . **Free tier**: Yes, 6 versions/10k ops. **Best for**: GCP organizations wanting native secrets management with a genuine free tier—**trade-off**: rotation notifications cost $0.05 each; no dynamic credentials .

- **1Password**
  **Password manager with Developer Tools** for secrets automation. **Pricing**: **Business $7.99/user/month**; **Starter $19.95/5 users/month**; **Enterprise custom**. Developer Tools (API keys, certificates, infrastructure secrets) are a **separate product line** . **Free tier**: No free tier for API access. **Best for**: teams already on 1Password wanting to extend into developer secrets—**trade-off**: Developer Tools separate; no dynamic credentials or rotation engine.

- **Okta**
  **Identity platform** with secrets and credential management via Workflows and Access Gateway. **Pricing**: Quote-only; per-user and per-module models. **Free tier**: Developer edition available. **Best for**: organizations wanting identity and secrets under one governance plane—**trade-off**: secrets management is not Okta's primary focus; complex licensing.

- **Auth0**
  **Identity platform for applications** with credential management for API access. **Pricing**: Free tier for small projects; paid plans scale by MAU. **Free tier**: Yes, limited. **Best for**: developers wanting API authentication and token management without building auth from scratch—**trade-off**: customer identity focus; not a secrets vault.

- **Postman**
  **API platform** with auth management for collections and environments. **Pricing**: Free tier; paid per user. **Free tier**: Yes, limited. **Best for**: teams wanting to manage API auth during development and testing—**not** a production secrets management platform.

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
