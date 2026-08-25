---
title: Use playbooks and negotiation posture
slug: use-playbooks-and-negotiation-posture
category: gitlaw-how-to-guides
excerpt: Steer GitLaw Agent's redlining and negotiation suggestions by setting up a playbook of your standard positions and telling the Agent in chat what negotiation posture to take, which controls how assertive its edits are.
---

Playbooks and negotiation posture work together to make GitLaw Agent's suggestions match your actual negotiating strategy - not just generic best practice.

- **Playbook** - a saved set of your preferred clauses, fallback positions, and non-negotiables that the Agent checks every contract against.
- **Negotiation posture** - how hard you want the Agent to push when it proposes redlines or counter-proposals, which you set just by telling it in chat.

---

### What is a playbook?

A playbook captures your organisation's standard positions for a given contract type (for example, an NDA playbook or a SaaS MSA playbook). When you review an incoming document, the Agent compares each clause against your playbook and flags deviations - clauses that are missing, weaker than your standard, or that your playbook marks as non-negotiable.

The Agent uses the playbook to:

- Identify where the counterparty's draft deviates from your preferred language.
- Propose redlines that bring the contract back in line with your positions.
- Suggest alternative wording drawn from your standard clauses rather than generic templates.
- Highlight any clause the counterparty has changed that touches a non-negotiable item.

Playbooks are private to your organisation. The counterparty's agent works only from their own playbook - your positions, tactics, and internal notes are never shared. See [Negotiate and redline a contract](/knowledge-base/negotiate-and-redline-a-contract) for how data isolation works across parties.

---

### Setting the negotiation posture

There's no posture slider to configure. Instead, you tell the Agent in chat how you want to negotiate - how hard to push, where to compromise, and what matters most - and it shapes its redlines and counter-proposals accordingly. For example:

- "Take a collaborative approach - look for compromise wording both sides will accept."
- "Be assertive on liability and IP, but flexible on everything else."
- "Hold a firm line and propose minimal concessions."

You can change tack at any point in the conversation. Adjusting your instructions does not change which clauses the Agent flags - it changes how the Agent words its proposed redlines and what kind of counter-proposals it suggests. Ask it to push back harder and it will challenge most counterparty changes; ask it to find middle ground and it will look for compromise language both sides are likely to accept.

---

### How playbooks and posture work together during a negotiation

1. **Drafting (your document)** - the Agent checks your draft against your playbook before you send it, flagging anything that falls short of your standard positions.

2. **Receiving a counterparty draft** - the Agent analyses the incoming document, identifies deviations from your playbook, and proposes redlines. The aggressiveness of those redlines is shaped by your chosen posture.

3. **Responding to counterparty edits** - when the counterparty returns a marked-up version, the Agent summarises what changed, assesses risk, and suggests responses. Again, the posture controls whether the Agent recommends accepting a compromise or holding the line.

4. **Final checks** - once both sides converge, the Agent can assist with cross-references, signature blocks, and exhibit attachments before the document goes to execution.

For step-by-step guidance on running a full negotiation cycle, see [Negotiate and redline a contract](/knowledge-base/negotiate-and-redline-a-contract). For general document review without a negotiation workflow, see [Review a document using Agent](/knowledge-base/review-a-document-using-agent).

---

### Best practices

- **Let GitLaw build the playbook, then tune it.** GitLaw auto-creates playbooks from the documents you upload, and you can edit them by hand whenever you like. You don't need to spell out industry-standard positions - the Agent already applies those - so focus your playbook on the unique deviations you want from the market standard.
- **Mark true non-negotiables explicitly.** The Agent will flag these regardless of posture, keeping your must-haves visible throughout the negotiation.
- **Tell the Agent how assertive to be.** Ask it to push harder for high-stakes deals, or to favour compromise when preserving the relationship matters more than squeezing every term.
- **Always review AI-generated redlines before sending.** The Agent proposes edits as tracked changes; you accept or reject each one. Nothing leaves your document without your approval.
