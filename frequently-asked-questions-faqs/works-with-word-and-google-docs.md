---
title: Does GitLaw work with Microsoft Word and Google Docs?
slug: works-with-word-and-google-docs
category: frequently-asked-questions-faqs
excerpt: Yes - GitLaw round-trips Word (.docx) documents, preserving tracked changes and comments both ways, and imports from Google Docs. Here's exactly how it works.
---

Yes. GitLaw fits into the way you already work. You can bring a Microsoft Word
or Google Docs file into GitLaw, review and edit it with AI, and send it back out
as a Word document - with your **tracked changes and comments fully intact in both
directions**. Nobody on the other side needs a GitLaw account, and nothing about
your existing Word or email workflow has to change.

## The short version

- **Import** a `.docx` or Google Doc - GitLaw reads the whole document, including
  any existing **tracked changes and comments**.
- **Work** on it in GitLaw: redline with AI, accept or reject changes, and add your
  own edits and comments.
- **Export** back to Word - your edits come out as native Word **track changes**, and
  your comments come out as native Word **comments**, so the other side sees them
  exactly as if you'd marked up the document by hand.

This is true round-tripping: a document can go Word → GitLaw → Word (and back again)
without losing the markup that matters in a negotiation.

## Importing from Word

When you upload a `.docx` file, GitLaw doesn't just read the final text - it
understands the document's structure and its review layer:

- **Tracked changes** - insertions, deletions, and replacements are all read in, so
  you can see and act on the counterparty's redlines.
- **Comments** - each comment keeps its **author, timestamp, and the exact text it's
  anchored to**. Reply threads are not yet preserved on import: a thread arrives as a
  single comment.
- **Formatting** - headings, lists, tables, and numbering are preserved wherever
  possible.

## Working on the document in GitLaw

Once it's in, the document behaves like any GitLaw contract:

Tracked changes only appear if you have **track changes turned on**. With it on:

- Ask the AI to **review and redline** it, and every suggested edit appears as a
  tracked change you can **accept or reject** one by one.
- Your own edits are recorded as tracked changes too.
- Leave **comments** and reply in threads, just like in Word.

With track changes turned off, edits are applied directly to the document instead of
being marked up.

## Exporting back to Word

When you're ready to send it out, export to `.docx`:

- **Track changes map both ways.** Insertions, deletions, and replacements you (or
  the AI) made in GitLaw become real Word track changes - the recipient can accept
  or reject them in Word.
- **Comments map both ways.** Your GitLaw comments export as native Word comments,
  with the author preserved.

That means you can run the AI review inside GitLaw and hand the counterparty a
clean Word file that opens with familiar redlines and margin comments - no GitLaw
login required on their end.

## Exporting to PDF

Need a PDF instead? You can download the document as a PDF.

## What about Google Docs?

You can bring a Google Doc into GitLaw directly. Choose **Add from Google Drive** -
available in chat, in e-sign and in Files - and pick the file. GitLaw converts native
Google Docs itself; no manual download is needed. Drive import also accepts DOCX, PDF,
TXT, MD and HTML, up to 20 files at a time.

## Is everything tracked?

Yes - every change is captured in the document's **revision history**, so you always
have a record of what changed and when.

---

**In short:** GitLaw plugs into Word and Google Docs rather than replacing them. Bring
the document in, let the AI do the heavy lifting on review and redlining, and send it
back out in the format the other side expects - with your track changes and comments
carried through every step.
