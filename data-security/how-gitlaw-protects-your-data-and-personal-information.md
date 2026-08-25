---
title: How GitLaw Protects Your Data and Personal Information
slug: how-gitlaw-protects-your-data-and-personal-information
category: data-security
excerpt: Your contracts contain sensitive information - names, email addresses, financial terms, and business details. This guide explains exactly how GitLaw stores, processes, and protects that data.
---

Your contracts contain sensitive information - names, email addresses, financial terms, and business details. This guide explains exactly how GitLaw stores, processes, and protects that data.

# Overview

#### What does this cover?

This article explains how GitLaw handles personally identifiable information (PII) and sensitive business data found in your contracts and documents. It covers encryption, data storage, access controls, AI processing, and your rights over your data.

#### Key takeaways

- All data is encrypted at rest and in transit
- Primary data storage is in the US and EU (Belgium)
- Your private documents are never visible to other users or competitors
- AI features use third-party providers (Anthropic, OpenAI and Google) that do not train on your data
- You can access, export, and delete your data at any time
- GitLaw is GDPR-compliant and SOC 2 Type 2 certified

# How Your Data Is Protected

#### Encryption

All data is encrypted using industry-standard methods:

- **At rest:** AES-256 encryption protects stored documents and data
- **In transit:** TLS 1.2+ encryption secures data moving between your browser and our servers

This means your contract content - including counterparty names, emails, rates, and payment terms - is encrypted both when stored and when transmitted.

#### Where is my data stored?

We only use trusted cloud infrastructure that complies with ISO 27001, SOC 2, CCPA, and GDPR requirements. Our primary data infrastructure runs on Google Cloud servers located in **the US and EU (Belgium)**.

We also use:

- **PostgreSQL** for structured data storage
- **Elasticsearch** for search functionality

For a full list of where data is stored and processed, see our [Where We Store Data](https://www.git.law/knowledge-base/where-we-store-data) article.

#### Access controls for your documents

- **Private by default** - all documents are private unless you explicitly share them
- **Organization owners can access their organization data** - including files owned by others within their organization.
- **Role-based access control (RBAC)** so only authorized users with specific permissions can access or edit documents

#### How we operate at GitLaw

GitLaw uses multiple layers to prevent unauthorized access:

- **Multi-factor authentication (MFA)** for account login. We use Sprinto to continuously monitor compliance across the organization.
- **Regular security audits** and vulnerability assessments.
- **Principle of Least Privilege** so team members are granted only the minimum level of access necessary to perform their job functions.

# AI Features and Your Data

#### Does AI process my contract data?

When you use GitLaw's AI features (document review, drafting, clause analysis), your document content is sent to third-party AI providers for processing (OpenAI, Anthropic and Google). Our AI providers do not use your data to train their models – your data is processed and discarded. We may use de-identified or aggregated data to improve GitLaw's features over time (e.g. statistical patterns like clause frequency for the benefit of all GitLaw users), but your document content is never exposed to other users or shared with third parties for training.

Important things to know:

- **Data minimization:** We send only the data needed for the specific AI task you've requested.
- **No model training:** Our AI providers do not use your inputs to train their models. Your contract data is processed and discarded - it does not become part of any AI training dataset.
- **Zero data retention:** Our primary AI provider (Anthropic) operates under a zero data retention agreement - your contract data is not stored by the AI provider after processing is complete.
- **Conversation logging**: Your AI conversation chain is sent to LangSmith, a monitoring and observability tool by LangChain, which we use to debug, monitor, and improve the quality of AI responses. LangSmith does not use your data for model training. At GitLaw we carefully limit who inside GitLaw has access to our production LangSmith instance.
- **Optional:** AI features are optional. You can use GitLaw's editor, collaboration, and version control features without ever triggering AI processing.

# Privacy Between Parties

#### Can the other side of my contract see my notes or strategy?

No. GitLaw enforces **strict data isolation** between parties:

- Each party's data, notes, and AI interactions are completely separate
- Negotiation tactics, internal notes, and playbook details are never shared between parties
- Only the document itself (and any marked-up versions you choose to share) passes between parties

#### Can competitors see my contract terms?

No. Private documents on GitLaw are private. Other users cannot see, search, or access your documents unless you explicitly share them.

#### What access to data do GitLaw staff have?

We limit internal access to your data to what's needed to run and improve the service:

- A small number of team members can review data processed by our AI features in LangSmith to monitor quality, debug issues, and improve reliability. This data is retained for 14 days and then automatically deleted.
- Only team members who need this access for their role have it.
- We do not access your documents for sales, marketing, or any purpose unrelated to running the service.
- We may access your data if you ask us to (e.g., for a support request), for security purposes (e.g., scanning for malware), or where required by law.

We will notify you if we ever need to access your private content outside of normal service operations, unless prohibited by law.

# Compliance and Certifications

- **GDPR** - Compliant. EU data residency, data minimization, user rights.
- **SOC 2 Type 2** - Certified.
- **Data Protection Agreement** - Available for enterprise customers.

You can view our full security posture, policies (34+), and controls at our [**Trust Center**](https://gitlaw.trust.site/).

# Frequently Asked Questions

#### Does GitLaw sell my data?

No. We do not sell your personal data or contract content to third parties.

#### Who are GitLaw's subprocessors?

We use a limited number of subprocessors, including providers for cloud infrastructure, content delivery, and authentication. A full list is available in our [Subprocessors](https://www.git.law/knowledge-base/gitlaw-subprocessors) article. We provide 30 days' notice before adding new subprocessors.

#### Is my chat history with the AI assistant private?

Yes. Your conversations with GitLaw's AI assistant are private between you and the AI. They are not visible to other users, counterparties, or the public.

#### How does GitLaw handle data breaches?

We have an incident management policy in place. In the event of a data breach affecting your personal data, we will notify you and the relevant authorities as required by GDPR and applicable law.

# Further Reading

- [GitLaw Trust Center](https://gitlaw.trust.site/) - Security posture, policies, and compliance status
- [Privacy Policy](https://git.law/privacy-policy)
- [Terms of Use](https://git.law/terms-of-service)
- [Where We Store Data](https://www.git.law/knowledge-base/where-we-store-data) - Data storage locations and infrastructure
- [GitLaw Subprocessors](https://www.git.law/knowledge-base/gitlaw-subprocessors) - Third-party data processors
- [Security](https://www.git.law/knowledge-base/security) - Security controls overview

# Need Help?

If you have questions about how your data is handled, contact us:

- **Privacy questions:** privacy@git.law
- **Data Protection Officer:** dpo@git.law
- **General support:** Through the GitLaw support portal

_GitLaw is a technology platform that provides legal document tools and AI-assisted document generation. GitLaw is not a law firm and does not provide legal advice._
