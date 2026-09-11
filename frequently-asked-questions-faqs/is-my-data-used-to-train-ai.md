---
title: Is my data used to train AI models?
slug: is-my-data-used-to-train-ai
category: frequently-asked-questions-faqs
excerpt: "No: GitLaw's AI providers do not train on your contract data, and your document content is never shared with third parties for model training."
---

No. Your contracts and document content are not used to train AI models - by GitLaw or by the AI providers that power GitLaw's features.

## How AI processing works

When you use GitLaw's AI features (document review, drafting, clause analysis), your document content is sent to third-party AI providers - currently Anthropic, OpenAI, and Google - to carry out the specific task you requested. Once the response is returned, your data is discarded. It does not become part of any training dataset.

A few specifics worth knowing:

- **No model training.** GitLaw's AI providers contractually do not use your inputs to train their models. Your contract data is processed for your request only.
- **Zero data retention (Anthropic).** GitLaw's primary AI provider, Anthropic, operates under a zero data retention agreement - your data is not stored by Anthropic after processing is complete.
- **Data minimisation.** Only the data needed for the specific task you trigger is sent to an AI provider.
- **AI features are optional.** You can use GitLaw's editor, collaboration, and version control features without ever triggering AI processing.

## What about conversation logs?

Your AI conversation chain is sent to LangSmith (a monitoring tool by LangChain) so GitLaw can debug issues and improve response quality. LangSmith does not use your data for model training. Within GitLaw, access to the production LangSmith instance is restricted to a small number of team members who need it for their role. Conversation data in LangSmith is retained for 14 days and then automatically deleted.

## What GitLaw may use de-identified data for

GitLaw may use de-identified or aggregated data - for example, statistical patterns such as clause frequency - to improve GitLaw's features over time for the benefit of all users. Your document content is never exposed to other users or shared with third parties for training purposes.

## AI subprocessors

The third-party providers that process data on GitLaw's behalf are listed in the [GitLaw Subprocessors](/knowledge-base/gitlaw-subprocessors) article. GitLaw gives at least 30 days' notice before adding new subprocessors.

## Further reading

- [How GitLaw Protects Your Data and Personal Information](/knowledge-base/how-gitlaw-protects-your-data-and-personal-information) - full overview of encryption, access controls, and AI processing
- [Where We Store Data](/knowledge-base/where-we-store-data) - data storage locations and infrastructure
- [GitLaw Subprocessors](/knowledge-base/gitlaw-subprocessors) - authorised third-party processors
- [Privacy Policy](https://git.law/privacy-policy) - how GitLaw handles Personal Data

Questions? Contact us at privacy@git.law or reach our Data Protection Officer at dpo@git.law.
