# Awesome-Customer-Knowledge-Base-Help-Center

# Awesome-Customer-Knowledge-Base-Help-Center
**Top Customer Knowledge Base Help Center (Opensource) 🌟 Star if you like it! 🌟**

**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on Self-Service Portals, AI-Powered Search, Article Analytics & Self-Hosted Documentation Hubs*
**Last updated: November 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Customer Knowledge Base & Help Center** software. These tools enable support teams to publish help articles, reduce ticket volume through self-service, and surface answers with AI search—from fully managed platforms with enterprise governance and analytics to self-hosted knowledge platforms that give organizations complete ownership of their documentation and customer data.

**Examples** include Zendesk Guide, Document360, Helpjuice, Guru, Slab, Bloomfire, Freshdesk Knowledge Base, GitBook, Archbee, and HubSpot Knowledge Base (the category leaders in commercial space).

**Open-source emphasis**: This section is expanded with every relevant project for self-hosted knowledge bases, help centers, and open documentation infrastructure. **Critical note**: The open-source landscape has matured—**Red Arch Knowledge Manager (KM2)** is the most ambitious platform with RAG chat, knowledge graphs, and field-level RBAC , while **Synthadoc** offers a local-first LLM compilation approach . No open-source project matches Zendesk Guide's support-ecosystem integration or Document360's analytics depth out of the box, but for core knowledge base functionality, the open-source options are production-capable.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Zendesk Guide](https://www.zendesk.com/)**
  **Knowledge base within Zendesk Suite** with AI search and article analytics. **Pricing**: **Suite Team $55/agent/month** (annual) is the first tier that includes Knowledge Base; **Suite Professional $115/agent/month** adds AI reporting; no free plan after **14-day trial** . **Free tier**: No—trial only. **Best for**: Zendesk support customers wanting KB integrated with ticketing—**trade-off**: requires Suite Team tier ($55/agent/month); article limit 40,000.

- **[Document360](https://document360.com/)**
  **Knowledge base platform** with AI features and analytics. **Pricing**: Pricing data conflicts across sources—Outmano reports **custom/quote-only with 14-day trial and no free plan** , while Toolradar reports a **free plan** (2 team accounts, 50 articles) and **Standard from $149/month** . **Free tier**: Conflicting reports—verify directly with vendor. **Best for**: teams wanting dedicated KB software with analytics—**trade-off**: pricing opacity and conflicting public data.

- **[Helpjuice](https://www.helpjuice.com/)**
  **Knowledge base platform** for customer and internal docs. **Pricing**: **Customized Knowledge Base $249/month** (30 users, 12GB, no AI); **AI-Powered $449/month** (100 users, 24GB, SSO, AI Suite); **Unlimited $799/month** (unlimited users, 38GB, AI, SSO) . **Free tier**: **No free tier**; **14-day free trial** with full access, no credit card required . **Best for**: teams wanting a dedicated KB with tiered AI options—**trade-off**: premium pricing; read-only users count as paid seats .

- **[Guru](https://www.getguru.com/)**
  **AI knowledge management** with verified cards and contextual delivery. **Pricing**: **Free for up to 3 users** (unlimited light users); **Starter 5 users €5/user/month**; **Builder €10/user/month** (advanced permissions, analytics, duplicate detection); **Expert €20/user/month** (AI suggestions, ticket linking) . **Free tier**: Yes, 3 users. **Best for**: teams wanting verified knowledge cards in Slack/Teams—**trade-off**: per-user pricing scales with team size.

- **[Slab](https://slab.com/)**
  **Knowledge base with unified search** across connected tools. **Pricing**: **Free plan** with **1 workspace, 2,000 monthly credits, 1 GB storage, 100,000 API requests/month**; all plans support **unlimited users** . **Free tier**: Yes, unlimited users with limits on credits/storage/API. **Best for**: teams wanting a wiki with search across Slack, Drive, and other sources—**trade-off**: credit-based AI consumption on all plans.

- **[Bloomfire](https://bloomfire.com/)**
  **Knowledge sharing platform** with AI search. **Pricing**: **Quote-only**; **no free plan**; only a guided "Test Drive" demo . **Free tier**: None. **Best for**: mid-market and enterprise teams wanting a knowledge program with AI search—**trade-off**: multi-year contracts; no self-serve evaluation.

- **[Freshdesk Knowledge Base](https://www.freshworks.com/freshdesk/)**
  **Knowledge base within Freshdesk** support suite. **Pricing**: **Free program for 1-2 agents for 6 months** includes ticketing, knowledge base, and reports—no credit card required . **Free tier**: Yes, 1-2 agents for 6 months. **Best for**: small support teams wanting free KB with ticketing—**trade-off**: limited free period; scales to paid after 6 months.

- **[GitBook](https://www.gitbook.com/)**
  **Documentation platform** with Git sync and AI features. **Pricing**: **Free trial of Ultimate plan features**—starts when you publish a site or invite members; no payment method required to start . **Free tier**: Trial only; free plan exists after trial downgrade. **Best for**: product documentation with developer workflows—**trade-off**: trial converts to paid for advanced features.

- **[Archbee](https://www.archbee.com/)**
  **Documentation platform** for product and API docs. **Pricing**: **Growing from $80/month** (10GB + 2GB/team member); **Scaling from $350/month** (20GB + 10GB/member); **Enterprise quote-only**. **No free tier**—"A free offering is not available at the moment" . **Free tier**: None; **14-day trial** no credit card required. **Best for**: teams wanting API docs with portals—**trade-off**: no free tier; readers never charged as seats.

- **[HubSpot Knowledge Base](https://www.hubspot.com/)**
  **Knowledge base within HubSpot Service Hub**. **Pricing**: Included with Service Hub Professional ($100/seat/month) and Enterprise. **Free tier**: Limited. **Best for**: HubSpot users wanting KB integrated with CRM and tickets.

## Open-Source GitHub Projects

- **[Red Arch Knowledge Manager (KM2)](https://github.com/redarchlabs/red-arch-km)**
  **Open-source, role-based knowledge management platform** (Apache-2.0) — **the most feature-complete open-source knowledge platform** found in this research, combining an enterprise document brain with a no-code application layer . **Features**: **Knowledge brain with RAG and passage-level citations**—chat answers cite the exact passage; vector search (Qdrant) and knowledge graph (Neo4j); **permission-aware search**—results filtered by caller's permissions before return . **No-code app layer**—custom entities, forms, views, dashboards, reports, BPMN-style workflows; bundled LMS, HRMS, and ticketing designs are configurations of these primitives . **Governed AI agents**—org chart with model tiering, authority engine, approvals, schedules . **Enterprise controls**—Clerk OIDC auth, org API keys with scopes, HMAC-signed webhooks, release-based change management with diff/preview/rollback, cross-org site-admin console . **Isolation by default**—PostgreSQL Row-Level Security, per-entity write policies, per-field read policies (`server_only`, `workflow_only`) . **Tech stack**: FastAPI (Python), Next.js (React), PostgreSQL 18 (RLS), Qdrant, Neo4j, Redis, MinIO . **Deploy**: Self-hosted (Docker Compose via `make dev-infra` and `make dev`) . **Trade-off**: **Complex deployment**—requires Clerk (cloud OIDC), multiple databases, and operational maturity. Go rewrite in progress but Python services authoritative . **Best for**: organizations wanting an enterprise-grade self-hosted knowledge platform with governed AI, field-level security, and no-code app building—not just a help center.

- **[Synthadoc](https://github.com/axoviq-ai/synthadoc)**
  **Open-source LLM knowledge compilation engine** (license per repo) — **the most innovative local-first approach** to knowledge bases, turning raw documents into structured Markdown wikis . **Features**: **Compiles documents into a self-contained wiki**—a folder of Markdown pages maintained and cross-referenced automatically; **Obsidian plugin** for browsing; CLI ingest and query commands; **local-first**—server binds to `127.0.0.1:7070` (localhost-only); supports switching LLM providers via config; **human-readable alternative to traditional RAG** . **Tech stack**: Python (pip install), Docker optional . **Deploy**: Local (`pip install synthadoc`; `synthadoc serve`) or Docker . **Trade-off**: **Single-user local tool**—not a multi-tenant help center; no web UI for customers; no permissions or SSO. **Best for**: individuals and small teams wanting a local, transparent, LLM-compiled wiki they fully own—not a customer-facing help center.

### Additional Strong Open-Source Options

- **Docmost** — Open-source collaborative wiki (AGPL-3.0 core). Real-time editing, spaces, native diagrams, built-in auth. **Note**: Team wiki, not a customer help center—no public portal or article analytics. **Best for**: internal team documentation.
- **BookStack** — Simple self-hosted wiki (MIT). Shelves → Books → Chapters → Pages hierarchy; WYSIWYG editor; built-in auth. **Note**: Internal wiki, not customer-facing help center. **Best for**: non-technical teams wanting structured internal docs.
- **Outline** — Polished team wiki (BSL 1.1). Notion-like editor; requires external SSO. **Note**: Internal wiki; source-available not OSI open source. **Best for**: teams with existing SSO wanting a modern internal wiki.

**Frameworks for building custom systems**: **Red Arch KM2** is the closest open-source analog to a full knowledge platform, with RAG, permissions, and no-code apps. **Synthadoc** serves local-first compilation. **Docmost, BookStack, and Outline** provide internal wiki foundations. **None provide a customer-facing help center with public portal, article analytics, and support-ticket integration**—those require commercial platforms or significant custom development.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Knowledge base platforms handling customer data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls for internal and external documentation.
- **The "customer-facing help center" vs. "internal wiki" vs. "knowledge platform" distinction is critical.** **Zendesk Guide, Document360, Helpjuice, Freshdesk KB, and HubSpot KB** are **customer-facing help centers**—they publish public articles and integrate with support tickets . **Guru and Slab** are **internal knowledge tools**—they surface answers to employees, not customers . **Red Arch KM2** is a **knowledge platform**—it combines internal knowledge with no-code apps and governed AI, but is not a turnkey customer help center . **Docmost, BookStack, and Outline** are **internal wikis**—not customer-facing. **Synthadoc** is a **local compilation tool**—not a multi-user platform . **Choose based on whether you need public self-service, internal team knowledge, or a governed platform.**
- **Pricing data for Document360 conflicts across sources.** One source reports custom/quote-only with no free plan ; another reports a free plan (2 accounts, 50 articles) and Standard at $149/month . **Verify directly with the vendor before committing.**
- **Helpjuice has no free tier and charges read-only users as paid seats.** Plans start at $249/month for 30 users, with AI requiring $449/month . **The 14-day trial requires no credit card** .
- **Zendesk Guide requires Suite Team at $55/agent/month**—the lower Support Team tier ($19/agent/month) does not include Knowledge Base . **Budget accordingly for a 10-agent team: $550/month minimum** .
- **Guru's free tier covers only 3 users**—unlimited light users can view but not edit . **For teams larger than 3, paid plans start at €5/user/month** .
- **Archbee has no free tier**—"A free offering is not available at the moment" . **Trial is 14 days with no credit card** .
- **Red Arch KM2 is the most capable open-source knowledge platform**, but it is **complex to deploy**—requiring Clerk (cloud OIDC), PostgreSQL, Qdrant, Neo4j, Redis, and MinIO . **For organizations wanting governed AI knowledge with field-level security, it is the most ambitious option.**
- **Synthadoc is not a help center.** It compiles documents into a local wiki for individual browsing—no public portal, no multi-user permissions . **For internal knowledge compilation, it is useful; for customer self-service, look elsewhere.**
- Self-hosted open-source solutions require proper infrastructure, security hardening, and ongoing maintenance. **Knowledge bases may contain internal procedures and customer-facing content**—ensure your deployment meets your organization's privacy and access control requirements before publishing.

---

**Made for support teams, documentation leads, and organizations building transparent knowledge base solutions.**
Let's make Customer Knowledge Base & Help Center more open, data-driven, and self-service-friendly.
