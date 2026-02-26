# AI Check

A checklist to verify AI-generated content before publishing or using it in important decisions.
Also used before deploying a new agent or automation to production.

This is a sequence of pointed questions — not a form to fill mechanically.
Most checks take under 5 minutes.

**When to use**:
- Before publishing AI-generated content
- Before making business decisions based on AI analyses
- Before approving AI-created or AI-based documents
- Before sending AI-generated communications to customers
- Before deploying a new agent or automation to production

---

## A — Accountability

Did we use a tool that is listed and approved in our AI Map?

- [ ] Yes — the tool is in AI Map
- [ ] No — **stop**: add tool to AI Map and get AI Leader approval first

---

## I — Inclusivity

**Prompt hygiene** — check the prompt you used, not just the output:

- [ ] The prompt was neutral — no built-in assumptions about gender, age, race, background, or ability
- [ ] The prompt asked for sources or verification where facts are involved

**Output bias check**:

- [ ] Content is free from stereotypes (gender, age, race, disability, background)
- [ ] Content does not exclude or disadvantage any group
- [ ] Customer-facing content uses inclusive language

If bias found: revise the prompt or regenerate before continuing.

---

## E — Explainability

- [ ] All key facts and figures have been verified against a reliable source
- [ ] Information is current and accurate as of today
- [ ] Checked why did the AI provide this answer and what are its sources.
- [ ] The AI reasoning is clear and makes sense (if it sounds too perfect or unusual, verify independently)

Common sense rule: if something looks too good or too strange, it needs additional checking.

---

## T — Transparency

Does this content need to be disclosed as AI-generated or AI-assisted?

Mark as AI-generated if:
- [ ] It will be published externally
- [ ] It will be sent to a customer or partner
- [ ] It is used in an official document, report, or pitch
- [ ] A customer interaction was handled by an automated agent

Disclosure options:
- Content footer: *"Created with AI assistance, reviewed by [Name]."*
- Customer message: *"This response was generated with AI assistance."*
- Website FAQ: *"We use AI tools for [purpose]. All customer-facing content is human-reviewed."*

---

## H — Human-Centricity

- [ ] The output informs a decision — it does not make the decision autonomously
- [ ] If this directly affects a person (hiring, health, finance, legal): a human has reviewed and approved it

For agents and automations:
- [ ] Any action involving money, account changes, contracts, or bulk communications was explicitly approved by a human before execution

---

## O — Oversight

- [ ] A human reviewed and approved the final output
- [ ] The output meets our quality standards

For agents and automations (fill only if Automation? = Yes in AI Map):
- [ ] Kill switch confirmed — location: _______________
- [ ] Logs or audit trail active — location: _______________

---

## S — Safety and Security

**Data entered into the AI tool — confirm none of the following was included**:

- [ ] Customer personal data (name, national ID, address, phone, personal email)
- [ ] Medical data
- [ ] Financial data (card numbers, bank accounts, financial statements)
- [ ] Trade secrets (proprietary processes, pricing, unpublished strategy)
- [ ] Plain access credentials (passwords, API keys, tokens, private keys)
- [ ] Information covered by NDA or confidentiality agreement

If any box is checked: **stop** — remove the data and regenerate. Submit an AI Note to the AI Leader.

**Safe to use**:
- Publicly available information (articles, documentation, Wikipedia)
- Your own drafts without sensitive details
- General research and writing prompts
- Anonymized or synthetic data (Customer A, City X, Order 00001)
- Access credentials (passwords, API keys, tokens, private keys) only with encryption.

For agents with External Access? = Yes (fill only if applicable):
- [ ] Outbound data filtered — no prohibited data is sent to external APIs or services