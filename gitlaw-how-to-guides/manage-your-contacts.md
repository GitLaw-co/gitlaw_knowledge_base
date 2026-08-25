---
title: Manage your contacts
slug: manage-your-contacts
category: gitlaw-how-to-guides
excerpt: 'Keep counterparty details in one place: create Person and Company contacts, link them to each other, and let GitLaw Agent populate them automatically from uploaded documents.'
---

Contacts is GitLaw's address book for counterparties. Once a contact exists, the Agent can look it up while drafting or reviewing, and you can link reminders directly to it. There are two contact types - **Person** and **Company** - and you can link people to companies to build a full picture of each counterparty.

### Create a contact

**From Files**

1. Open **Files** and select the **Contacts** tab.
2. Select **New contact** and choose **Person** or **Company**.
3. Fill in the required field (full name for a person, company name for a company) and any optional fields - email, phone, address, and relationship.
4. Save.

---

### Contact types and key fields

| Type        | Required field | Optional fields                                           |
| ----------- | -------------- | --------------------------------------------------------- |
| **Person**  | Full name      | Email, phone, company name, company address, relationship |
| **Company** | Company name   | Company address, relationship                             |

The **relationship** field is a single-select label (Client / Customer, Vendor / Supplier, Investor / Lender, Employee / Contractor, Advisor / Consultant, or Other) that helps you categorise contacts at a glance.

---

### Link a person to a company

A Person contact can be linked to a Company contact as a point of contact. Open the person's record, find the **Company** field, and search for an existing Company contact to attach. You can unlink them at any time without deleting either record.

---

### Search and manage contacts

The contacts list is paginated and supports free-text search across name fields. Use the search bar at the top of the list to find a contact by name. You can edit or delete any contact from its detail view.

---

### Contacts created automatically from uploaded documents

When you [import a Word or PDF contract](/knowledge-base/import-a-word-or-pdf-contract), GitLaw extracts the named parties from the document. Each unique party is automatically promoted to a Contact and labelled with the document it came from - for example **Found in Acme MSA**. Contacts you add yourself are labelled **Added by you**. Review and edit these auto-created contacts on the **Files → Contacts** tab - the originating document stays linked regardless of any edits you make to the contact.

---

### GitLaw Agent and contacts

The Agent can search for contacts and create or update them during a conversation - for example, if you mention a counterparty by name that doesn't have a record yet, it will offer to create one before proceeding. Any Agent-driven change requires your confirmation before it is saved.

---

### Best practices

- Create Company contacts first, then link Person contacts to them - this keeps your counterparty structure clean and makes Agent lookups more accurate.
- Use the relationship label consistently so you can filter and find contacts quickly.
- After [sharing a document or inviting a counterparty](/knowledge-base/share-a-document-or-invite-a-counterparty), add them as a contact to build a full history over time.
