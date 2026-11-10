---
title: Does GitLaw work with Claude or ChatGPT?
slug: does-gitlaw-work-with-claude-or-chatgpt
category: frequently-asked-questions-faqs
excerpt: "Yes. Connect GitLaw to Claude, ChatGPT or any MCP-compatible AI assistant and ask it to find, read, draft and redline your contracts, with GitLaw's legal AI doing the legal work."
---

Yes. GitLaw has an MCP server, so Claude, ChatGPT and other AI assistants can keep your contracts in GitLaw and work on them without you leaving the chat. GitLaw stores every contract in one place, keeps every version and records changes as tracked changes. You sign in to GitLaw once and click **Allow**; you don't need an API key. It works on every GitLaw plan, free included.

### What your assistant can do

| Ask your assistant to…               | What happens in GitLaw                                                                      |
| ------------------------------------ | ------------------------------------------------------------------------------------------- |
| **Bring in your existing contracts** | Imports a .docx (up to 10 MB) and stores it with your other contracts, searchable           |
| **Find or read a contract**          | Searches your documents by title and summary, and reads the full text                       |
| **Review a contract you were sent**  | Edits are applied directly, or as tracked changes you accept or reject in GitLaw            |
| **Check if a clause is standard**    | GitLaw answers using its jurisdiction playbooks (US, UK, India) and your organisation's own |
| **Draft a new contract**             | GitLaw's legal AI drafts it from a template or from scratch, for your jurisdiction          |
| **Export to Word**                   | Hands you back a Word file of any contract                                                  |

Your assistant gives you a link to open each document in GitLaw.

### How to connect

**Claude (web and desktop)**

1. In Claude, open **Settings → Connectors** and click **Add custom connector**.
2. Name it **GitLaw** and paste `https://be-public-api.git.law/mcp`.
3. A GitLaw window opens: sign in and click **Allow**.
4. In a chat, turn GitLaw on from the tools menu and ask about your contracts.

On Claude Team and Enterprise plans, an owner may need to add the connector for the organisation first.

**ChatGPT**

1. In ChatGPT, open **Settings → Apps & Connectors → Advanced** and turn on **Developer mode**.
2. Back in **Apps & Connectors**, click **Create**.
3. Name it **GitLaw**, paste `https://be-public-api.git.law/mcp` and choose **OAuth**.
4. Sign in to GitLaw and click **Allow**.

Custom connectors need a paid ChatGPT plan.

**Claude Code**

Run `claude mcp add --transport http gitlaw https://be-public-api.git.law/mcp`, then type `/mcp` in Claude Code, pick **gitlaw** and choose **Authenticate**.

**Cursor, VS Code and other apps**

Any app that supports remote MCP servers with sign-in (OAuth) works with `https://be-public-api.git.law/mcp`.

### GitLaw AI or your assistant's own?

Both work together. Your assistant reads, summarises and answers follow-ups in seconds, on your Claude or ChatGPT plan. GitLaw AI drafts, redlines and checks clauses against legal playbooks, and uses your GitLaw AI credits. Say "ask GitLaw" to get GitLaw's legal answer instead of your assistant's.

---

**Related articles**

- [What can an AI assistant connected to GitLaw access?](/knowledge-base/what-can-connected-ai-apps-access)
- [How is GitLaw different from ChatGPT?](/knowledge-base/how-is-gitlaw-different-from-chatgpt)
- [AI credits and top-ups](/knowledge-base/ai-credits-and-top-ups)
