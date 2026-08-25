---
title: Import a Word or PDF contract
slug: import-a-word-or-pdf-contract
category: gitlaw-how-to-guides
excerpt: Bring your existing contracts into GitLaw in bulk - GitLaw preserves track changes and comments, extracts parties and key dates automatically, and keeps your original files intact until you choose to edit them.
---

If your contracts live in a folder of Word documents or PDFs, you can bring them into GitLaw all at once. GitLaw stores the originals exactly as they are, extracts the key details automatically, and only converts a file to its editable format when you actually open it to make changes.

#### Accepted formats

GitLaw accepts **DOCX** and **PDF** files from your device. You can also use **Add from Google Drive**, which additionally accepts native Google Docs, TXT, MD and HTML - up to 20 files per batch. DOCX files with tracked changes and comments are supported: revision marks and comments (including author and timestamp) are preserved on import.

---

### How to import your contracts

##### Step 1: Open the upload panel

In the main menu, click **Files**, then select **Upload files**. You can also upload during onboarding - GitLaw offers this step after you complete your profile, and you can skip it and come back at any time.

##### Step 2: Select your files

Choose one or more DOCX or PDF files from your device, or use **Add from Google Drive** (up to 20 files per batch). Processing is limited by your monthly allowance. If a batch would exceed your remaining allowance, GitLaw processes files in order and holds the rest with a clear message.

##### Step 3: Watch extraction run

After upload completes, GitLaw routes you to **Files → Overview**, which fills in progressively as each file finishes. For each file, GitLaw automatically extracts:

| Field                               | Notes                                                                                                                                        |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **Parties**                         | Primary parties become Contacts; other named parties (signatories, witnesses, advisors) stay on the file detail and can be promoted manually |
| **Status**                          | Inferred as Draft, In review, Pending signature, Signed or Expired                                                                           |
| **Category**                        | Matched against the GitLaw category list (NDA, SaaS Agreement, Employment Contract, etc.)                                                    |
| **Execution date / Effective date** | Captured as distinct fields when both are present                                                                                            |
| **Expiry / renewal date**           | Auto-creates a Reminder with a 30-day lead time                                                                                              |
| **Governing law and courts**        | Captured when stated                                                                                                                         |

Extraction runs on the original file - no conversion is needed for GitLaw to read the content.

##### Step 4: Review extracted details

Click any file to open its detail view. You will see the extracted fields as chips at the top and a summary below. Fields that could not be extracted with confidence are flagged for your attention. You can edit any field inline.

---

### What gets preserved

|                                                      | Preserved on import                                                                           |
| ---------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Track changes (inserts, deletes, replacements)       | Yes - imported as revision marks; counterparty edits are attributed to a placeholder identity |
| Comments (author, timestamp, thread, anchored range) | Yes                                                                                           |
| Headings, tables, lists, numbering                   | Yes where feasible; lossy cases surface a warning on the file detail                          |
| Original file format                                 | Yes - your DOCX or PDF is stored as version 1 and remains accessible via version history      |

The original file is **not** converted until you open it to edit. At that point the conversion happens once, and the original is preserved as v1 in version history. If any content cannot round-trip cleanly, a warning appears on the file detail.

---

### After import

- **Contacts** - each primary party becomes a Contact on the **Files → Contacts** tab, deduplicated by name. You can click a Contact to see every file, reminder, and chat related to them.
- **Reminders** - renewal and expiry dates create Reminders with a default 30-day lead time. Look for the "inferred" tag on auto-created Reminders; confirm or edit them to remove it.
- **Chat** - you can attach any imported file to a chat session and ask the agent to review, redraft, or compare it. See [Attach a file to chat](/knowledge-base/attach-a-file-to-chat).
- **Export** - once a file is in GitLaw's editor you can export it as DOCX or PDF. Comments are included in DOCX exports only. See [Export your document](/knowledge-base/export-your-document).

---

### Merging files manually

If GitLaw does not automatically detect that two files are versions of the same contract (for example, because the filenames are very different), you can merge them via chat. Open a chat, attach both files, and tell the agent - for example, _"This is the same contract as the Acme MSA from last month."_ The agent will propose the merge for your confirmation.

---

### Related guides

- [How to add a new file to GitLaw](/knowledge-base/how-to-add-a-new-file-to-gitlaw)
- [Review a document using the agent](/knowledge-base/review-a-document-using-agent)
- [Attach a file to chat](/knowledge-base/attach-a-file-to-chat)
- [Export your document](/knowledge-base/export-your-document)
