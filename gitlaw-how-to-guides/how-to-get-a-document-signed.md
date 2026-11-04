---
title: How to get a document signed
slug: how-to-get-a-document-signed
category: gitlaw-how-to-guides
excerpt: 'Send a finished document for e-signature directly from GitLaw: add signers, place signature fields, and receive a tamper-sealed PDF - all for free.'
---

GitLaw includes free built-in e-signatures, so you can send a finalised document for signing without leaving the platform or paying extra.

### Steps

1. **Start signing:** open the document, click **Share** at the top right, then **eSign** at the bottom of the panel. You can also choose **Start eSign** from the **…** menu next to the document title. Or ask the Agent: "Send this for signature".

   ![The Share panel with the eSign button](https://git.law/kb-images/how-to-get-a-document-signed/share-panel.png "ring: 55.5 86 15.5 8")

2. **Add yourself if you sign too:** GitLaw asks for your signature details. Click **Add** to sign the document yourself, or **Skip**.

3. **Add recipients:** click **Add recipient** and enter each person's name, email and role (for example **Needs to sign**). If the document contains signature blocks placed in the GitLaw editor, GitLaw detects the parties for you. Click **Add fields** when everyone is listed.

   ![Step 1, Add recipients, with one recipient and the Add fields button](https://git.law/kb-images/how-to-get-a-document-signed/sign-recipients.png "narrow; ring: 5.5 28 88 15")

4. **Place signature fields:** click **Auto-place fields** to let GitLaw place them, or open **Place fields manually**. You can move any field before sending.

5. **Send:** click **Send**. Each signer receives an email from `sign@git.law` containing the document name, their role, and a button to sign in their browser. No GitLaw account is required to sign.

   ![Step 2, Add signature fields, with Auto-place fields and the Send button](https://git.law/kb-images/how-to-get-a-document-signed/sign-fields.png "narrow; ring: 5.5 46.5 88 15; ring: 51 83 43.5 11.5")

6. **Track status:** The document moves through three states - **Draft → Awaiting Signatures → Fully Signed**. You can see who has signed and who has not from the document view, and send a reminder to anyone outstanding using **Send reminder**.

7. **Receive the signed PDF:** Once every party has signed, GitLaw generates a final, tamper-sealed PDF and attaches it to the document. All participants receive a copy by email. The document is then locked against further edits.

### Audit trail

Every signing event produces a secure audit file stored alongside the signed PDF. It captures:

| Data point                   | Purpose                            |
| ---------------------------- | ---------------------------------- |
| Timestamp of each signature  | Legal audit trail                  |
| Signer IP address            | Identity evidence                  |
| Device / browser fingerprint | Dispute resolution                 |
| Email address used           | Authentication match               |
| Full transaction log         | Sent → Viewed → Signed → Completed |

This meets industry standards (equivalent to DocuSign / HelloSign audit certificates) and is legally enforceable under the **ESIGN Act / UETA** (US), **Electronic Communications Act 2000** (UK), and **eIDAS Regulation** (EU).

### Notes

- **Collaboration history is excluded.** The version sent for signature contains only the finalised document - chat, comments, and drafting history are not shared with signers.
- **Free, always.** E-signature is included in GitLaw at no extra cost and is not metered.
- **Signing from the Agent.** If you prefer, simply tell the Agent to send the document for signature. It will detect the parties and guide you through the same flow.

### Related articles

- [Export your document](/knowledge-base/export-your-document)
- [Review a document using Agent](/knowledge-base/review-a-document-using-agent)
- [File sharing and permissions](/knowledge-base/file-sharing-permissions-in-personal-and-organisation-accounts)
