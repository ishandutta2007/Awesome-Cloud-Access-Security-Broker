# Awesome-Cloud-Access-Security-Broker

## Top Cloud Access Security Broker (CASB) Platforms Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Shadow IT Discovery, Data Loss Prevention, SaaS Posture Management & Threat Protection*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Access Security Brokers (CASB)**. These tools help security teams gain visibility into cloud application usage, enforce data security policies across SaaS and IaaS, discover shadow IT, and protect sensitive data as it moves between users, devices, and cloud services.



**Examples** include Netskope, Microsoft Defender for Cloud Apps, Skyhigh Security, Lookout CASB, Bitglass, Forcepoint ONE, Palo Alto Prisma SaaS, Zscaler CASB, Broadcom CloudSOC, and Cisco Cloudlock (the category leaders).



**Open-source emphasis**: CASB is one of the **most commercially consolidated categories** in cybersecurity. **No production-ready open-source CASB platform exists** that matches the full scope of commercial offerings. The open-source landscape consists of **research projects**, **partial implementations**, and **building blocks** rather than complete solutions. The most notable open-source effort is **ReliableSecurity/cloud-security-broker** (a CASB system with DLP, MFA, and monitoring for Yandex Cloud, SberCloud, and Mail.ru, with AWS/Azure in development) , and **Tanitay/Cloud-Access-Security-Broker-Project** (a learning project exploring CASB concepts with AWS and GCP) . This section documents these foundations honestly, including the significant gap between research projects and enterprise-grade CASB capabilities.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Netskope](https://www.netskope.com/)**

  The leading CASB platform, now part of Netskope One SSE. Provides both **inline** and **API-based** modes, with deep integration into Next-Gen Secure Web Gateway. Features generative AI-powered app risk classification, visibility into **80,000+ SaaS applications and IaaS services**, Cloud Confidence Index (CCI) risk scoring across 50+ categories, and unified DLP across all cloud traffic . The inline architecture provides real-time enforcement, not retrospective API-only control. Offers incident management workflows, UEBA, and advanced threat protection with sandboxing .



- **[Microsoft Defender for Cloud Apps](https://learn.microsoft.com/en-us/defender-cloud-apps/)**

  Full-featured CASB integrated into Microsoft Defender XDR. Provides fundamental CASB capabilities (shadow IT discovery, information protection, compliance), plus **SaaS Security Posture Management (SSPM)** with recommendations from CIS benchmarks, **App-to-App protection** for OAuth apps, and **AI agent protection** for Copilot Studio agents . Integrates with Microsoft Purview for DLP and sensitivity labels. SSPM data feeds into Microsoft Secure Score .



- **[Skyhigh Security](https://www.skyhighsecurity.com/)**

  Enterprise CASB with **Cloud Registry** (world's largest cloud service registry with 261-point risk assessment), **Autonomous Remediation** (coaches users and auto-resolves incidents), and **In-App Coaching** (real-time guidance within native apps) . Supports OneDrive with near real-time scanning (10-15 seconds) via API or inline reverse proxy, with quarantine/tombstone capabilities . Multi-source control covers upload, cloud-created, shared, cloud-to-cloud, and download .



- **[Lookout CASB](https://www.lookout.com/)**

  Secure Cloud Access CASB within Lookout's Cloud Security Platform. Provides real-time policy enforcement for public/external shares, content inspection with DLP, and automated removal of unauthorized collaborators . Features Cloud Sandbox for zero-day malware, UEBA-based risk scoring, and native DRM policies (data masking, watermarking, time-bound encryption) . Also provides CSPM, SSPM, and DSPM capabilities .



- **[Bitglass](https://www.bitglass.com/)**

  Agentless CASB with **multi-mode** deployment (API, inline proxy, on-device SWG). Uniquely combines CASB, SWG, and ZTNA in a single platform . Features SmartEdge SWG that decrypts traffic on-device to minimize latency, and zero-day threat protection powered by Cylance . Agentless architecture enables BYOD security without device agents .



- **[Forcepoint ONE CASB](https://www.forcepoint.com/)**

  Unified CASB with inline and API inspection, agentless application access, and built-in DLP enforcement. Named a Leader in Gartner Magic Quadrant for CASB for three consecutive years . Provides **190+ pre-defined data security policies**, unlimited scalability on AWS with 99.99% uptime, and shadow IT reporting/blocking .



- **[Palo Alto Prisma SaaS](https://www.paloaltonetworks.com/)**

  CASB integrated into Prisma Access (Strata Cloud Manager). Provides SaaS Security Inline, SaaS Security API, SSPM, and Enterprise DLP. Offers **CASB-X** license with all components. Dashboard views for Discovered Apps, Data Security, Posture Security, and Behavior Threats .



- **[Zscaler CASB](https://www.zscaler.com/)**

  Multi-mode CASB within Zscaler's SSE platform. Provides inline security for data in transit (TLS/SSL inspection, shadow IT detection, DLP) and out-of-band API scanning for data at rest. Cloud Sandbox processes 200 billion transactions daily, identifying 150 million threats .



- **[Broadcom CloudSOC](https://techdocs.broadcom.com/)**

  Symantec's CASB and Cloud DLP platform. Components include **Gatelets** (inline inspection of managed cloud services) and **Securlets** (API connectors to cloud services). Cloud Detection Service (CDS) provides DLP detectors and policies .



- **[Cisco Cloudlock](https://www.cisco.com/)**

  Cloud-native CASB using APIs to manage cloud app ecosystem risks. Features user security (ML-based anomaly detection, impossible travel), data security (continuous DLP monitoring), and app security (Apps Firewall with Community Trust Rating). **FedRAMP ATO** certified .



## Open-Source GitHub Projects



- **[ReliableSecurity/cloud-security-broker](https://github.com/ReliableSecurity/cloud-security-broker)**

  **The most complete open-source CASB implementation available.** A production-ready Cloud Security Broker with **DLP, MFA, and enterprise security features** . **Cloud providers supported**: Yandex Cloud (full support: Compute, Storage, IAM, Audit Trails), SberCloud (basic: Compute, Storage, Security), Mail.ru Cloud (basic: Compute, Storage). **AWS, Azure, and GCP are in development or planned** . **Features**: Access control policies for cloud resources, DLP engine with scanning and automatic encryption of confidential files, monitoring with anomaly detection rules (e.g., mass data download alerts), API integration with credential management and resource synchronization, dashboards (general, activity monitoring, DLP, policy management), and metrics tracking (total requests, blocked requests, threats detected, DLP scans) . **Open source**. **Limitations**: Primarily focused on Russian cloud providers; Western cloud support is incomplete; no inline proxy or SSPM capabilities.



- **[Tanitay/Cloud-Access-Security-Broker-Project](https://github.com/Tanitay/Cloud-Access-Security-Broker-Project)**

  **A learning/research project exploring CASB concepts.** Tests features including data protection, threat detection, and access control using **AWS and Google Cloud** . Designed to enhance cloud security through real-world implementation and testing. **1 star, 1 commit**. **Educational project** — not production-ready, but provides a foundation for understanding CASB architecture with AWS/GCP.



### Additional Building Blocks (Not Complete CASB Solutions)



- **DLP Engines**: **pleno-dlp** (multi-format secret and PII scanning, SARIF output), **Nightfall sensitive-data-scanner** (PII/API key discovery via APIs).

- **Shadow IT Discovery**: **Cloudflare CASB** (Free tier supports up to 2 integrations; Enterprise tier for full findings detail) . Commercial but has a free tier for evaluation.

- **SSPM Foundations**: **Prowler** (open-source cloud security posture management for AWS, Azure, GCP), **ScoutSuite** (multi-cloud security auditing).

- **API Security**: **OWASP ZAP** (for API security testing), **42Crunch** (API security audit).



**Frameworks for building custom systems**: Combine **ReliableSecurity/cloud-security-broker** as the core CASB engine (for Yandex/Sber/Mail.ru cloud environments), **pleno-dlp** for DLP scanning capabilities, and **Prowler** or **ScoutSuite** for SSPM foundations. **Critical gap**: No open-source solution provides the inline proxy, real-time enforcement, API connectors for major SaaS apps (M365, Google Workspace, Salesforce), or the scale of commercial CASB platforms. Building a production CASB requires significant custom development across cloud API integrations, inline traffic inspection, and policy engines.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- CASB platforms handle sensitive cloud data and user activity; ensure compliance with data protection regulations and cloud provider terms of service.

- **Open-source reality**: **No production-ready open-source CASB platform exists** that matches commercial offerings. **ReliableSecurity/cloud-security-broker** is the most complete implementation but is primarily focused on Russian cloud providers (Yandex Cloud, SberCloud, Mail.ru) with AWS/Azure/GCP support incomplete or in development . **Tanitay/Cloud-Access-Security-Broker-Project** is educational . Commercial platforms (Netskope, Microsoft Defender for Cloud Apps, Skyhigh, Lookout, Bitglass, Forcepoint, Palo Alto, Zscaler, Broadcom CloudSOC, Cisco Cloudlock) provide inline proxy, API connectors for major SaaS apps, SSPM, and enterprise-scale enforcement that open-source alternatives cannot match without massive investment. For organizations seeking a free entry point, **Cloudflare CASB** offers a free tier with limited integrations .



---



**Made for cloud security architects, SOC analysts, data protection officers, and SaaS security teams.**

Let's make cloud access security more open, transparent, and enforceable.
