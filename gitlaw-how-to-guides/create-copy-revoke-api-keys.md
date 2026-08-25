---
title: Create, copy and delete GitLaw API keys
slug: create-copy-revoke-api-keys
category: gitlaw-how-to-guides
excerpt: API keys let external systems authenticate with the GitLaw Public API. Learn how to create a key, copy it (it's shown only once), delete it, and keep it secure.
---

GitLaw API keys authenticate requests to the [GitLaw Public API](/knowledge-base/gitlaw-public-api-reference). If you want to trigger contract generation or document analysis from your own tools - or from automation platforms like Make, n8n, or Pipedream - you'll need an API key.

GitLaw provides a management interface to **create, copy, and delete** keys.

## What API keys are for

An API key is a secret credential that identifies your account when you call the GitLaw Public API. Every API request includes the key (via the `X-API-Key` header), and GitLaw uses it to authenticate and authorise the request. Anyone holding the key can make requests as you, so treat it like a password.

## Create a key

1. Open your GitLaw account settings and go to the API keys section.
2. Choose to create a new key.
3. GitLaw generates the key and displays it.

## Copy the key (shown only once)

When a key is created, GitLaw shows the full secret **only once**, at creation time. Use the copy action to copy it immediately and store it somewhere secure - a secrets manager or your integration's environment configuration.

If you navigate away without copying it, you won't be able to see the full key again. In that case, create a new key and delete the old one.

## Delete a key

If a key is no longer needed, has been exposed, or you want to rotate credentials, delete it from the same API keys section. Deletion is permanent and cannot be undone. Once deleted, the key stops working immediately and any system still using it receives a `401 Unauthorized` response. To keep an integration running, create a new key and update your integration before deleting the old one.

**Limits:** up to 30 keys per account; key names up to 50 characters; each key can be set to expire after 7, 30 or 90 days, or never.

## Security best practice

- **Store keys securely** - never commit them to source control or paste them into shared documents or chats.
- **Treat a key like a password** - anyone with it can act as you against the API.
- **Rotate regularly** - periodically create a new key and delete the old one.
- **Delete on exposure** - if a key may have leaked, delete it straight away and issue a replacement.
- **Use one key per integration** where practical, so you can delete a single integration's key without affecting others.

For the full list of endpoints, request and response formats, and example requests, see the [GitLaw Public API Reference](/knowledge-base/gitlaw-public-api-reference). If you'd rather not write code, the [Zapier integration](/knowledge-base/automate-contracts-with-zapier) offers a no-code alternative.

## Quick reference

| Question                      | Answer                                                               |
| ----------------------------- | -------------------------------------------------------------------- |
| What is an API key for?       | Authenticating requests to the GitLaw Public API.                    |
| When can I copy the full key? | Only once, at creation - copy and store it then.                     |
| What if I lose it?            | Create a new key and delete the old one.                             |
| What does deleting do?        | Removes the key permanently; requests using it return `401`.         |
| How should I store it?        | Securely, like a password - never in source control or shared chats. |

---

Related articles: [GitLaw Public API Reference](/knowledge-base/gitlaw-public-api-reference) · [Automate contracts with Zapier](/knowledge-base/automate-contracts-with-zapier)
