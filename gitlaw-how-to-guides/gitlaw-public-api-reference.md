---
title: GitLaw Public API Reference
slug: gitlaw-public-api-reference
category: gitlaw-how-to-guides
excerpt: Build custom integrations with the GitLaw Public API - trigger contract generation and document analysis from any system over HTTP.
---

Build custom integrations with the GitLaw Public API. Connect GitLaw to any system - your internal tools, Make, n8n, Pipedream, or anything else that can make HTTP requests.

**Prefer no-code?** Use our [Zapier integration](/knowledge-base/automate-contracts-with-zapier) instead.

## Overview

The GitLaw Public API lets external services trigger contract generation and document analysis. Send a request, and the API processes it and returns the result directly in the response.

**What you can do:**

- Generate contracts and legal documents via AI
- Analyze existing documents by referencing a file already in GitLaw
- Upload new files for analysis by including base64-encoded content
- Continue existing chat conversations or start new ones

## Authentication

All API requests require an API key passed via the `X-API-Key` header:

`X-API-Key: YOUR_API_KEY   `

Generate API keys in your GitLaw account settings. The full key is shown **only once** at creation - store it securely.

## API Endpoint

### `POST /api/v1/chat/ask`

Send a message to generate or analyze a contract.

### Request Body

`{    "message": "Create an NDA between Acme Corp and Beta Inc",    "outputFileFormat": "docx",    "fileId": "file-123",    "fileContent": "base64...",    "fileName": "doc.docx",    "chatId": "550e8400-e29b-41d4-a716-446655440000"   }   `

### Parameters

| Parameter          | Required | Description                                                                     |
| ------------------ | -------- | ------------------------------------------------------------------------------- |
| `message`          | Yes      | Your request or instruction for the AI                                          |
| `outputFileFormat` | Yes      | Format of the returned document - `pdf` or `docx`                               |
| `chatId`           | No       | Chat ID to continue an existing conversation. If omitted, a new chat is created |
| `fileId`           | No       | ID of an existing file in GitLaw to use as context                              |
| `fileContent`      | No       | Base64-encoded file content to upload as a new document                         |
| `fileName`         | No       | Filename for the uploaded file (required when using `fileContent`)              |

### File Handling Rules

- You can provide `fileId`, `fileContent` + `fileName`, or neither - but **not both** `fileId` and `fileContent`
- If both `fileId` and `fileContent` are provided, the request is rejected with a `400 Bad Request` error
- If `fileContent` is provided, `fileName` must also be included (and vice versa)
- Use `fileId` for files already in GitLaw
- Use `fileContent` + `fileName` to upload a new file with your request

## Response

The API processes the request and returns the result directly.

### Success Response

`{    "chatId": "550e8400-e29b-41d4-a716-446655440000",    "answer": "I've created an NDA between Acme Corp and Beta Inc...",    "fileId": "file_789",    "fileContent": "base64...",    "fileName": "nda.docx"   }   `

| Field         | Description                                                            |
| ------------- | ---------------------------------------------------------------------- |
| `chatId`      | The chat where the conversation took place (existing or newly created) |
| `answer`      | The AI's response text                                                 |
| `fileId`      | ID of the file used or created (if applicable)                         |
| `fileContent` | Base64-encoded document content (if a document was generated)          |
| `fileName`    | Filename of the returned document                                      |

## Example: Create a Contract

### Request

`curl -X POST https://api.git.law/api/v1/chat/ask \    -H "X-API-Key: YOUR_API_KEY" \    -H "Content-Type: application/json" \    -d '{      "outputFileFormat": "docx",      "message": "Create an NDA between Acme Corp and Beta Inc"    }'   `

### Response

`{    "chatId": "550e8400-e29b-41d4-a716-446655440000",    "answer": "I've created an NDA between Acme Corp and Beta Inc...",    "fileId": "file_789",    "fileContent": "UEsDBBQAAAAI...",    "fileName": "nda.docx"   }   `

## Example: Analyze an Existing Document

### Request

`curl -X POST https://api.git.law/api/v1/chat/ask \    -H "X-API-Key: YOUR_API_KEY" \    -H "Content-Type: application/json" \    -d '{      "outputFileFormat": "docx",      "message": "Review this contract and identify any problematic clauses",      "fileId": "file_existing_789"    }'   `

### Response

`{    "chatId": "chat_123",    "answer": "I've reviewed the contract. Here are the key issues I identified:\n\n1. The liability clause in Section 4.2 is unusually broad...",    "fileId": "file_existing_789"   }   `

## Example: Upload and Analyze a New File

### Request

`curl -X POST https://api.git.law/api/v1/chat/ask \    -H "X-API-Key: YOUR_API_KEY" \    -H "Content-Type: application/json" \    -d '{      "outputFileFormat": "docx",      "message": "Summarize this contract",      "fileContent": "UEsDBBQAAAAI...",      "fileName": "vendor-agreement.docx"    }'   `

### Response

`{    "chatId": "550e8400-e29b-41d4-a716-446655440000",    "answer": "Here is a summary of the vendor agreement...",    "fileId": "file_new_456",    "fileContent": "UEsDBBQAAAAI...",    "fileName": "nda.docx"   }   `

## Example: Continue a Conversation

### Request

`curl -X POST https://api.git.law/api/v1/chat/ask \    -H "X-API-Key: YOUR_API_KEY" \    -H "Content-Type: application/json" \    -d '{      "outputFileFormat": "docx",      "chatId": "550e8400-e29b-41d4-a716-446655440000",      "message": "Now add a non-compete clause to the NDA"    }'   `

### Response

`{    "chatId": "550e8400-e29b-41d4-a716-446655440000",    "answer": "I've added a non-compete clause to the NDA...",    "fileId": "file_789",    "fileContent": "UEsDBBQAAAAI...",    "fileName": "nda.docx"   }   `

## Error Handling

### Common Errors

| Error                                            | Cause                                        | Solution                                      |
| ------------------------------------------------ | -------------------------------------------- | --------------------------------------------- |
| `400` - Missing `message`                        | Required field not provided                  | Include a `message` in the request body       |
| `400` - Both `fileId` and `fileContent` provided | These fields are mutually exclusive          | Use one or the other, not both                |
| `400` - `fileContent` without `fileName`         | `fileName` is required when uploading a file | Include `fileName` alongside `fileContent`    |
| `401` - Unauthorized                             | Invalid or expired API key                   | Check your API key is correct and not expired |
| `404` - Invalid `fileId`                         | File doesn't exist or isn't accessible       | Verify the file ID and your permissions       |
| `403` - Forbidden                                | The key may not act on this resource         | Check the key's account and permissions       |
| `413` - Payload Too Large                        | Decoded file over 1 MB (~1.4 MB base64)      | Send a smaller file                           |
| `422` - Conversion failed                        | The document could not be converted          | Check the file is a valid DOCX or PDF         |
| `429` - Rate limited                             | Too many requests                            | Wait before retrying                          |
| `500` - Server error                             | Unexpected failure on our side               | Retry, then contact support if it persists    |

## Best Practices

1.  **Store your API key securely** - It is shown only once at creation and cannot be recovered
2.  **Use `chatId` to continue conversations** - This preserves context from previous messages, producing better results
3.  **Prefer `fileId` for existing files** - Avoid re-uploading files that are already in GitLaw
4.  **Handle errors gracefully** - Check HTTP status codes and parse error responses
5.  **Respect rate limits** - Back off when you receive a `429` response

## Questions?

If you encounter issues:

1.  Verify your API key is valid and not expired
2.  Ensure all required parameters are provided
3.  Check that `fileId` and `fileContent` are not used together
4.  Contact GitLaw support if problems persist
