# Quick Start Guide

Implement AIETHOS in your organization in 4 steps.

**Total time**: approximately 2 hours for a solo operator. Slightly more for a team.

---

## Step 0 — Solo operator? Start here.

If you work alone, your entire AIETHOS implementation is:

- **AI Leader**: you
- **AI Map**: one tab in a Google Sheet or Notion page
- **AI Check**: three questions on a sticky note on your monitor:
  - No customer or confidential data entered?
  - Marked as AI-generated if needed?
  - Facts verified before publishing?

Complete steps 1–4 once. It takes about two hours. You are done.

---

## Step 1 — Appoint an AI Leader

Name one person to own AI ethics and responsible use across your organization.

**Who**: the owner, CEO, COO, CTO, or another person with real authority and a working understanding of your AI tools. Deep technical skills are not required.

**Responsibilities**:
- Create and maintain the AI Map
- Receive and act on AI Notes
- Communicate with AI tool vendors
- Run or manage the regular review cycle
- Consult legal counsel on AI compliance

**Done when**: the AI Leader is named, announced to the team, and has access to all AI tools in use.

---

## Step 2 — Create an AI Map

List every AI tool your organization uses in a spreadsheet.

**Template**: `templates/ai_map_template.csv`

**Columns to fill**:

| Column | What to enter |
|--------|--------------|
| Tool | Name of the tool |
| Provider | Company behind the tool |
| Risk Category (EU AI Act) | EU AI Act category — ask the vendor or check with legal |
| Purpose / Use | What you use it for |
| Data Entered | What kind of data you put into it |
| Users | Who has access |
| Automation? | Yes if it runs without manual trigger each time |
| External Access? | Yes if it calls external APIs or services |
| Used From / To | Dates |
| Vendor Contact | Support URL or email |
| Vendor Compliance | Confirmed / Not yet / N/A |
| Notes | Anything relevant — limitations, special rules, kill switch if agent |

**Risk categories** (EU AI Act, 2026):
- **Minimal risk** — most productivity tools, chatbots, content generators
- **Limited risk** — tools interacting with people (must disclose AI use)
- **High risk** — tools used in hiring, credit, health, law enforcement (require extra scrutiny)
- **Prohibited** — never use (social scoring, real-time biometric surveillance in public, subliminal manipulation)

**Done when**: all tools are listed, risk categories assigned, and AI Map is accessible to the whole team.

---

## Step 3 — Implement AI Check and AI Note

**AI Check**: Use before publishing content or using AI output in important decisions. Template: `templates/ai_check.md`

**AI Note**: Provide to all employees for reporting issues. Template: `templates/ai_note.md`

**Done when**: templates are accessible and the team knows when to use them.

---

## Step 4 — Establish Review Cycle and Contact with Legal Counsel

**Review cycle**:

**For teams**: 10-minute AI agenda in regular status meeting.

**For small teams**: async — AI Leader scans AI Notes and AI Map every month.

**Legal counsel**: Ensure the AI Leader has access to legal support for AI compliance. This is the only regulatory requirement in AIETHOS.

**Done when**: review cadence is set and legal contact is established.

---

## AIETHOS Light — Minimum for Very Small Organizations

If your organization has very limited resources, implement these 5 minimum priorities:

1. Appoint an AI Leader
2. List all AI tools used (AI Map)
3. Create a list of prohibited data for AI input (include in AI Check)
4. Establish a policy for labeling AI-generated content
5. Determine which decisions always require human approval
