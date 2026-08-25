---
title: Accept or reject tracked changes
slug: accept-or-reject-tracked-changes
category: gitlaw-how-to-guides
excerpt: 'Learn how to turn Track Changes on, review proposed insertions and deletions inline, and accept or reject tracked changes individually or all at once - including changes from collaborators, the AI Agent, and imported Word documents.'
---

GitLaw uses **Track Changes** - the same revision marks you'd see in Microsoft Word - as the single way to review any proposed edit, whether it comes from you, a collaborator, the AI Agent, or an imported DOCX file. Every insertion, deletion, or formatting change appears inline; nothing is hidden in a separate diff view.

### Turning Track Changes on and off

When Track Changes is on, every edit you make is recorded as a tracked change rather than applied directly to the document.

1. **Open the document** in the GitLaw Editor.
2. **Toggle Track Changes on** using the control in the editor toolbar. When enabled, the control is highlighted and subsequent edits appear as coloured insertions or strikethrough deletions attributed to your name.
3. **Toggle it off** to return to direct editing. Changes you already made with Track Changes on remain as revision marks until accepted or rejected.

The AI Agent follows the same toggle. When Track Changes is on, Agent edits also appear as tracked changes attributed to you - your counterparty sees your name, not the AI's.

### Reviewing tracked changes

Insertions appear as coloured text and deletions appear as strikethrough, each labelled with the author's name and the date of the change. All pending changes are shown inline, so you can see exactly what's been proposed before you accept or reject anything.

### Accepting or rejecting individual changes

1. **Click on a tracked change** in the document. An action popover appears.
2. Choose **Accept** to apply the change (insertions stay, deletions are removed) or **Reject** to discard it (insertions are removed, deletions are restored).

Each accept or reject creates a new version in history, so nothing is lost. You can [view and restore version history](/knowledge-base/view-and-restore-version-history) at any time.

### Accepting or rejecting all changes at once

To resolve several changes at once, use the change list in chat when the Agent has proposed edits, or the review panel of an incoming change request - both offer **Accept all** and **Reject all**. In the document itself, changes are accepted or rejected one at a time.

### Changes from Word documents

When you import a DOCX file that already contains tracked changes, GitLaw preserves those revision marks with their original author names. Imported authors are shown with an **External** badge so you can tell them apart from GitLaw collaborators. Accepting or rejecting these marks works identically to native changes.

When you export to DOCX, tracked changes round-trip correctly and open with redlines in Word.

### Related articles

- [Negotiate and redline a contract](/knowledge-base/negotiate-and-redline-a-contract)
- [Review a document using Agent](/knowledge-base/review-a-document-using-agent)
- [View and restore version history](/knowledge-base/view-and-restore-version-history)
- [Add comments to a document](/knowledge-base/add-comments-to-a-document)
