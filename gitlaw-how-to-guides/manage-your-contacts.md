---
title: Manage your contacts
slug: manage-your-contacts
category: gitlaw-how-to-guides
excerpt: 'Keep counterparty details in one place: create Person and Company contacts, link them to each other, and let GitLaw Agent populate them automatically from uploaded documents.'
---

Contacts is GitLaw's address book for counterparties. Once a contact exists, the Agent can look it up while drafting or reviewing, and you can link reminders directly to it. There are two contact types - **Person** and **Company** - and you can link people to companies to build a full picture of each counterparty.

### Create a contact

**From Memory**

1. Open **Memory** in the left sidebar and select the **Contacts** tab.

   ![The Contacts tab with the Add new contact button](https://git.law/kb-images/manage-your-contacts/contacts-list.png "ring: 88 20 11.5 9.5")

2. Click **Add new contact** and choose **Person** or **Company** under **Contact type**.

   ![The Add contact form with the Contact type menu](https://git.law/kb-images/manage-your-contacts/contact-form.png "narrow; ring: 4.5 13 91 7.5")

3. Fill in the required field (full name for a person, company name for a company) and any optional fields - emails, phones, job title, address, linked company and relationship.
4. Click **Add contact**.

   ![Relationship quick picks and the Add contact button](https://git.law/kb-images/manage-your-contacts/contact-form-bottom.png "ring: 51 74 44 17")

---

### Contact types and key fields

| Type        | Required field | Optional fields                                           |
| ----------- | -------------- | --------------------------------------------------------- |
| **Person**  | Full name      | Emails, phones, job title, address, linked company, relationship |
| **Company** | Company name   | Company address, relationship                             |

The **relationship** field is free text with quick picks (Client or customer, Vendor or supplier, Investor or lender, Employee or contractor, Advisor or consultant, Others) that help you categorise contacts at a glance.

---

### Link a person to a company

A Person contact can be linked to a Company contact as a point of contact. Open the person's record, find the **Linked company** field, and search for an existing Company contact to attach. You can unlink them at any time without deleting either record.

---

### Who sees a contact in an organisation

In an organisation, each contact has a **Who sees it** setting: **Everyone in the organization** (the default) or **Only me**. A contact only you see carries an **Only you** badge. Whoever added a contact can change this setting later. A person everyone sees cannot belong to a company only you see, so share the company first.

Whoever added a shared contact can edit or delete it, and so can the organisation's owners and admins. Only you can edit a contact you keep as **Only me**.

---

### Search and manage contacts

The contacts list is paginated and supports free-text search across name fields. Use the search bar at the top of the list to find a contact by name. You can edit or delete a contact from its detail view.

---

### Contacts created automatically from uploaded documents

When you [import a Word or PDF contract](/knowledge-base/import-a-word-or-pdf-contract), GitLaw extracts the named parties from the document. Each unique party is automatically promoted to a Contact and labelled with the document it came from - for example **Found in Acme MSA**. Contacts you add yourself are labelled **Added by you**. In an organisation, parties found in a file only you can open become **Only me** contacts. Review and edit these auto-created contacts on the **Memory → Contacts** tab - the originating document stays linked regardless of any edits you make to the contact.

---

### GitLaw Agent and contacts

The Agent can search for contacts and create or update them during a conversation - for example, if you mention a counterparty by name that doesn't have a record yet, it saves one - or reuses the existing record when the name or an email already matches. The Agent saves without asking first, so review its changes on the **Memory → Contacts** tab.

---

### Best practices

- Create Company contacts first, then link Person contacts to them - this keeps your counterparty structure clean and makes Agent lookups more accurate.
- Use the relationship label consistently so you can filter and find contacts quickly.
- After [sharing a document or inviting a counterparty](/knowledge-base/share-a-document-or-invite-a-counterparty), add them as a contact to build a full history over time.
