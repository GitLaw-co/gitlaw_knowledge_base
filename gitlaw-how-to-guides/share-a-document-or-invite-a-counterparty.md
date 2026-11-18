---
title: Share a document or invite a counterparty
slug: share-a-document-or-invite-a-counterparty
category: gitlaw-how-to-guides
excerpt: Learn how to invite collaborators by email, create a shareable link, share documents with external counterparties, and revoke access on GitLaw.
---

All documents on GitLaw are **private by default**. This guide walks you through the different ways to share a document - whether with a colleague, an external counterparty, or anyone with a link.

For a full breakdown of what each role can do, see [File sharing permissions in personal and organisation accounts](/knowledge-base/file-sharing-permissions-in-personal-and-organisation-accounts).

---

### Roles at a glance

| Role       | Can edit | Can see earlier versions | Can share | Can manage participants | Can delete |
| ---------- | -------- | ------------------------ | --------- | ----------------------- | ---------- |
| **Owner**  | Yes      | Yes                      | Yes       | Yes (full control)      | Yes        |
| **Editor** | Yes      | Yes                      | Yes       | Yes (with limits)       | No         |
| **Viewer** | No       | No                       | No        | No                      | No         |

Editors can open the document's full version history, including every earlier draft. Viewers see only the current version. If earlier drafts contain anything you would not send to this person, share with **Viewer**.

Editors can invite new participants and promote others to Editor, but cannot remove Owners or grant the Owner role.

---

### Invite someone by email

1. Open the document you want to share.
2. Click **Share** at the top right of the document.
3. Type the person's email address in **Add people via email** and select it.

   ![The Share panel with the Add people via email field](https://git.law/kb-images/share-a-document-or-invite-a-counterparty/share-panel.png "ring: 5 15.5 90 14")

4. Select a role next to their name - **Editor** or **Viewer**. You can edit the optional message.
5. Click **Send**.

   ![The invite step with the role picker set to Editor and the Send button](https://git.law/kb-images/share-a-document-or-invite-a-counterparty/share-invite.png "ring: 72.5 42.5 23 8.5; ring: 5 84 90 10")

The recipient will receive an email with a link to access the document. They do not need to be a member of your organisation - GitLaw supports sharing with anyone.

---

### Create a shareable link

Instead of inviting people individually, you can generate a link to share.

1. Click **Share** on the document.
2. Under **General access**, choose who can open it:
   - **Only people you invite** - the link only works for people who are already collaborators or have a pending invitation.
   - **Anyone with the link** - anyone who has the URL can open the document, including people who are not signed in.
   - **Organization** - anyone in your organisation can view it.
   - **Public** - anyone can find and view it in the GitLaw community.

   ![The General access menu with Organization, Public, Anyone with the link and Only people you invite](https://git.law/kb-images/share-a-document-or-invite-a-counterparty/share-access.png "ring: 5.5 65 92 14")

3. Click **Copy link** at the bottom of the Share panel and send it.

Anyone opening the document through the link gets **view** access. To give someone edit access, invite them by email and choose **Editor**.

A document can have one active shared link at a time. Updating the settings on an existing link reuses the same URL - you do not need to redistribute it.

---

### Share with a counterparty for negotiation

Sharing with an external counterparty (for example, the other side in a contract negotiation) follows the same steps as inviting anyone else. A few things to keep in mind:

- Share with **Viewer** access so counterparties can review the document without making direct changes and without seeing your earlier drafts. Viewers see only the current version.
- A Viewer can create their own copy of the document, make edits to that copy, and submit it back to you as a **change request** for your review.
- Counterparties have no visibility into your organisation, its members, or any other documents - they only see what you share with them.

For more on the negotiation workflow, see [Negotiate and redline a contract](/knowledge-base/negotiate-and-redline-a-contract).

---

### Revoke access

**To remove an individual:**

1. Click **Share** on the document.
2. Find the person in the participants list.
3. Remove them or change their role.

**To revoke a shared link:**

1. Click **Share** on the document.
2. Set **General access** back to **Only people you invite**.

Once revoked, the link stops working immediately. If you create a new link for the same document later, the same link ID is reactivated - it does not generate a new URL.

---

### Who can see my document?

See [Who can see my documents](/knowledge-base/who-can-see-my-documents) for a full explanation of visibility, organisation access settings, and public sharing options.
