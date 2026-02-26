# AIETHOS Framework Overview

**Version**: 1.1.0
**Last updated**: February 2026

---

## Credo — 12 Principles

1. Technology should serve people — not the opposite.
2. Every intelligent system must protect human dignity, rights, and safety.
3. Creating benefits must go hand in hand with preventing harm.
4. Artificial intelligence systems should support people, not replace them.
5. Transparency of AI operation is a prerequisite for its acceptance.
6. Solutions should be designed with everyone in mind — without exceptions or exclusions.
7. The use of data must be based on informed, voluntary consent.
8. We respect ethical boundaries, even when crossing them is technically possible.
9. Ethics is never an add-on — it is built into the core of every solution.
10. Responsibility for the effects of AI begins at the design stage.
11. Those responsible for AI actions are its creators and operators — never the machine itself.
12. The long-term development of AI requires ethical vigilance.

---

## Three Core Documents

AIETHOS is built around three documents only. No others are required to implement the framework.

| Document | What it is |
|----------|-----------|
| **AI Map** | A spreadsheet listing every AI tool in use: purpose, data, users, vendor contact, risk category |
| **AI Check** | A checklist run before publishing content or approving AI-assisted decisions |
| **AI Note** | A lightweight issue report for logging problems, questions, or observations |

---

## The 7 Pillars

### A — Accountability

**Principle**: Programs and machines are not responsible. Accountability is always assigned to humans.

One person is the **AI Leader**. They own AI ethics across the organization, maintain the AI Map, respond to AI Notes, and communicate with tool vendors. In a small company, this is typically the owner or a senior manager. No dedicated role is needed — just a named person with real authority.

**AI Leader responsibilities**:
- Maintain and update the AI Map
- Receive and act on AI Notes (categorize as low/high risk)
- Communicate with AI tool vendors on behalf of the organization
- Run or coordinate the regular review cycle
- Consult with legal counsel on AI compliance

---

### I — Inclusivity

**Principle**: AI use must not exclude or discriminate against any individual or social group.

Check AI-generated content for bias before publishing or sending to customers. Pay special attention to stereotypes related to gender, age, background, disability, and socioeconomic status. Ensure equal access to AI tools across all relevant roles.

**Prompt hygiene**: The bias in AI output often originates in the prompt, not the model. Before submitting a prompt, ask: Does this prompt contain built-in assumptions? Does it ask for neutral, inclusive language?

Document 3–5 core principles for bias-free prompting and include them in your AI tool guides.

---

### E — Explainability

**Principle**: We understand what our AI tools can and cannot do, we can clearly explain the results, and we understand the limits of that explanation.

Create a short instruction for each AI tool: typical uses, known limitations, common errors, and risk category. Apply the common sense rule — if output sounds too good or too unusual, verify it before using it. For any output informing an important decision: note what factors the AI considered, what it could not consider, and where human judgment was applied. Determine which content types always require human review.

For agents and automations: document what actions they can and cannot perform.

**Scope clarification**: AIETHOS addresses *functional explainability* —the deployer's ability to understand, verify, and communicate AI outputs.*Technical XAI* (SHAP, LIME, model internals) is the responsibility of model providers.
This aligns with: OECD AI Principles 1.3 ("transparency and explainability"), NIST AI RMF (explainability as a trustworthiness characteristic), EU AI Act Art. 13 (outputs sufficiently transparent to enable interpretation), and GDPR Art. 13–15/22 (meaningful information about the logic of automated processing).

---

### T — Transparency

**Principle**: Be clear with your team and customers about when and how AI tools are used.

Mark AI-generated materials as standard practice. Add a note to your website FAQ. Draft 2–3 simple disclosure templates for customer communications and reports. Keep the AI Map as your single source of truth and update it when new tools are introduced.

---

### H — Human-Centricity

**Principle**: AI supports people and never replaces them. No AI system overrides basic human rights.

Define clearly which decisions require human sign-off. Hard rule: any choice that directly affects a person requires human review. Delegate repetitive work to AI; keep judgment, empathy, and ethical calls for humans. Collect team feedback through AI Notes and reflect it in AI Map updates.

---

### O — Oversight

**Principle**: Regularly verify that AI tools are used in accordance with policy and deliver expected benefit.

**Quality monitoring**: Collect examples of good and bad AI usage outcomes within the company. Track employee issues reported using AI Notes.

**Review options**:

**Option 1 — Team meetings**: Add a 10-minute AI agenda item to regular status meetings. Discuss AI Notes, AI Map changes, compliance updates.

**Option 2 — Async for small teams**: The AI Leader spends 5 minutes every two weeks scanning open AI Notes and checking for new tools in AI Map. No meeting required.

The AI Leader maintains contact with legal counsel and monitors regulatory updates.

---

### S — Safety and Security

**Principle**: Protect sensitive data from exposure to external AI tools and prevent misuse.

Maintain a short list of data categories that must never be entered into AI tools. Include this list in the AI Check (pillar S). Apply the rule: if in doubt, do not enter. Use AI Notes to report security issues and establish a fast escalation path for serious incidents.

**Categories that must never be entered**:
- Customer personal data (name, national ID, address)
- Medical data
- Financial data (card numbers, bank accounts)
- Trade secrets (proprietary processes, pricing, unpublished strategy)
- Plain access credentials (passwords, API keys, tokens — always encrypted)
- Information covered by NDA or confidentiality agreements

**Safe to use**:
- Publicly available information (articles, documentation, Wikipedia)
- Your own drafts without sensitive details
- Anonymized or synthetic data (Customer A, City X, Order 00001)
- General research and writing prompts

---

## Success Metrics

Track these simple metrics to measure improvement:

1. Number of unresolved AI Notes — lower is better
2. Percentage of published content incorrectly flagged as AI-generated — lower is better
3. Number of customer comments about AI-generated content — lower is better
4. Number of complaints about AI-based support — lower is better
5. Number of legal interventions related to AI use — lower is better

---

## How the Three Documents Bind the Pillars

| Pillar | AI Map | AI Check | AI Note |
|--------|--------|----------|---------|
| A — Accountability | Tool ownership, AI Leader | Approved tool confirmed | Issue ownership |
| I — Inclusivity | | Bias and prompt check | Bias incidents |
| E — Explainability | Tool limitations noted | Facts verified | Unexplained outputs |
| T — Transparency | Single source of truth | AI label confirmed | Disclosure issues |
| H — Human-Centricity | | Human approval confirmed | Decision override concerns |
| O — Oversight | Reviewed regularly | | Backlog reviewed async |
| S — Safety | Data types per tool | Prohibited data check | Security incidents |

---

## Extensions (No New Documents Required)

### Agents and Automations

If your organization uses automations or agents that act on external systems (email, CRM, payments), extend the existing documents as follows:

- **AI Map**: Add columns `Automation?` (Yes/No) and `External Access?` (Yes/No). In Notes: document kill switch location, log location, and outbound data filter.
- **AI Check**: Add three questions in pillars O and S — kill switch confirmed, logs active, outbound data filtered.

No new roles, documents, or meetings are required.

### Larger Organizations

For organizations with more than 10 people, separate policies, signed data lists, vendor review procedures, and onboarding checklists may be appropriate.

---

## AIETHOS Light — Minimum for Very Small Organizations

If your organization has very limited resources, implement these 5 minimum priorities:

1. Appoint an AI Leader
2. List all AI tools used (AI Map)
3. Create a list of prohibited data for AI input
4. Establish a policy for labeling AI-generated content
5. Determine which decisions always require human approval
