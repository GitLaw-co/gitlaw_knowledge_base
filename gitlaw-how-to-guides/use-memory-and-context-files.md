---
title: Use Memory and context files
slug: use-memory-and-context-files
category: gitlaw-how-to-guides
excerpt: GitLaw remembers key facts about your business, contracts, and counterparties so every chat feels less like starting from scratch.
---

Every time you start a chat in GitLaw, the Agent loads what it already knows about you - your company details, how you like contracts written, and notes on the counterparties you deal with. This collection of knowledge is called your **Memory**, and the individual notes it contains are called **Context Files**.

### What GitLaw remembers

Memory is organised into distinct layers:

- **Profile** - your legal name, trading name, jurisdiction, industry, and registered address. Set during [account setup](/knowledge-base/set-up-your-gitlaw-account) and editable in Settings.
- **Playbook** - drafting defaults, both cross-category and contract-specific: your preferred liability position, standard payment terms, governing law, and rules such as "for NDAs, always use a mutual structure."
- **Contact notes** - per-counterparty intelligence: negotiation history, red lines, fallback positions accepted, communication style. One note per contact, built up over time.

File summaries are not context files - they appear on the file detail page alongside the extracted structured fields.

The Agent loads whichever layers are relevant to the work in hand. If you open a chat about an NDA with Acme Ltd, it loads your Profile, your general and NDA-specific playbook, and your Acme contact note - not every note you have.

### How Memory is updated

GitLaw builds your Memory from several sources:

- **Chat** - as you talk to the Agent, it picks up preferences, corrections, and decisions. If you say "actually we switched to Net 45" mid-chat, that can update the relevant entry.
- **File upload** - when you upload an existing contract, GitLaw extracts parties, dates, governing law, category, and status, then generates a file summary and (where relevant) a counterparty note.
- **You, directly** - you can read and edit any Context File yourself at any time.

Facts the Agent learns are written to Memory and are always visible and reversible - you can open any entry and edit it.

### Viewing and editing your Context Files

Your context files are collected under **Memory** in the sidebar, in the **Context** section. From there you can:

- Filter by scope (Profile, Memory, Playbook, Contact)
- Click any entry to read the full note
- Edit the body inline and save your changes

Contact-specific notes are also accessible from a contact's detail view. File summaries appear on the file detail page alongside the extracted structured fields.

### Where Memory shows up in chat

The Agent cites memory at the point it uses it. If it applies your standard liability cap, it will say so - _"Using your preferred liability cap of £100k here"_ - rather than announcing a save during the conversation. This makes it easy to spot when a remembered preference is being applied, and to correct it if circumstances have changed.

### Good habits

- **Check your Profile is complete.** A full profile - especially [jurisdiction](/knowledge-base/set-your-jurisdiction) and industry - means the Agent's first draft is already closer to what you need. See [Set up your GitLaw account](/knowledge-base/set-up-your-gitlaw-account).
- **Upload your existing contracts.** The more contracts GitLaw has seen, the more accurate your playbooks and counterparty notes become.
- **Add contact notes for frequent counterparties.** A few lines on a counterparty's red lines saves you re-explaining them every time. Find contacts under **Files → Contacts** - see [Manage your contacts](/knowledge-base/manage-your-contacts).
