---
title: Attach a file to chat
slug: attach-a-file-to-chat
category: gitlaw-how-to-guides
excerpt: 'Attach a DOCX or PDF to GitLaw chat and the Agent will use it as a reference, edit it directly, or create a copy from it - depending on what you ask.'
---

You can attach an existing Word or PDF file to a GitLaw chat session. Before making any changes, the Agent reads your prompt to understand your intent and acts accordingly - so the outcome depends on how you phrase your request.

### **How to attach a file**

1. **Open a chat session:** Start a new chat or open an existing one.

2. **Attach your file:** Click the attachment button in the chat input and select a DOCX, PDF, MD or HTML file from your device. The file is added to your GitLaw files once you send the message.

3. **State your intent clearly:** Type your instruction in the same message (or immediately after). The Agent uses your wording to decide what to do with the file - see the table below.

### **What happens depending on your intent**

| Intent                  | Example prompt                                                   | What the Agent does                                                                                                                                                    |
| ----------------------- | ---------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Reference (context)** | "Here's our company policy - draft an NDA based on it"           | Reads the file as background context; creates a new, independent document. The original is untouched and no copy is made.                                              |
| **Edit**                | "Fix the typo in clause 3" or "Update the payment terms"         | Edits the file directly. DOCX and PDF files convert to GitLaw's editor format on the first edit; the original is preserved as version 1 in the file's version history. |
| **Template**            | "Fill this MSA for Client X" or "Create a new SOW based on this" | Creates a copy of your file with a link back to the source. The Agent edits the copy; the original stays untouched and remains reusable for future deals.              |

### **Tips for getting the outcome you want**

- **Context:** Mention what you want drafted, not what you want done _to_ the file. Phrasing like "based on this" or "using this as reference" signals context intent.

- **Edit:** Refer directly to content inside the file - clauses, sections, specific wording. The Agent will treat it as a document to modify in place.

- **Template:** Use phrases like "fill this for \[client\]", "create a new \[document type\] from this", or "use as a template". This triggers a copy so your master template is never overwritten.

### **Best practices**

1. **Check the file opened in the editor:** After the Agent acts, confirm it has opened the right file - the original or the new copy - before reviewing changes.

2. **Use version history:** For edited files, open the version history panel on the right to compare against the original if needed.

3. **Keep templates clean:** If you regularly reuse a contract template, always attach it with template-style phrasing so the original is never consumed.

---

Related guides: [Import a Word or PDF contract](/knowledge-base/import-a-word-or-pdf-contract) · [Review a document using Agent](/knowledge-base/review-a-document-using-agent) · [Create a draft document using Agent](/knowledge-base/create-a-draft-document-using-agent)
