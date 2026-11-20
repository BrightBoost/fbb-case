# Case brief: Fake Bright Bank (FBB)

> Fake Bright Bank is a fictional bank created for this training. Its policy, people and figures are invented. The regulation it is assessed against is real.

## The client

Fake Bright Bank N.V. (FBB) is a mid-sized Dutch bank with its head office in Amersfoort. It is a significant institution under direct ECB supervision.

| | |
| --- | --- |
| Total assets | about EUR 68 billion |
| Staff | about 3,900 FTE |
| Core business | Retail mortgages and savings (NL), SME and mid-corporate lending, a small treasury desk |
| Subsidiaries | FBB Lease B.V. (equipment leasing, NL) and Bright Bank Deutschland GmbH (online savings and SME lending, Germany, about 12% of group deposits) |
| Liquidity position | See `04-fbb-lcr-disclosure.csv` (four quarters, EU LIQ1 layout) |

## Why now

- The ECB's 2025 on-site inspection found weaknesses in FBB's risk data aggregation and risk reporting: unclear ownership of liquidity data, heavy manual aggregation and slow internal risk reporting.
- The Joint Supervisory Team has asked FBB to show how it will meet the ECB *Guide on effective risk data aggregation and risk reporting* (May 2024), read together with BCBS 239.
- FBB must submit a remediation plan in Q1 2027. Before approving the plan and its budget, the board wants an independent impact assessment.

## The board's question

> **"Does our risk data aggregation and liquidity reporting meet supervisory expectations, and what has to change?"**

- Audience: the Management Board, with the Supervisory Board's risk committee attending.
- Meeting: 15 December 2026.
- Format: at most 5 slides, plus an appendix if needed.
- Decision requested: approve the remediation priorities and a budget envelope.

## What we learned in the intake interviews

- FBB's data governance policy for risk data is RDG-01, version 2.3. See `03-fbb-data-governance-policy.md`.
- The monthly group risk report is delivered **26 working days** after month-end.
- **37 end-user computing tools** (mostly spreadsheets) sit in the credit and liquidity risk reporting chain. Only part of them is inventoried.
- Bright Bank Deutschland delivers its risk data to the group in separate spreadsheets.
- Data owners have been appointed for credit risk data. Owners for liquidity and market risk data have not been appointed yet.
- The CFO indicated a budget envelope of **up to EUR 15 million over two years** for the remediation programme.
- The Chief Data Officer (CDO) role was created in 2026. The CDO and the CRO both claim to chair the data quality committee.

## Stakeholders

| Role | Interest |
| --- | --- |
| CRO | Sponsor of this assessment, owns the relationship with the JST |
| CFO | Budget, alignment with finance data and COREP/FINREP reporting |
| CDO | New role, wants a group-wide data governance mandate |
| Head of Treasury | Runs liquidity management and the LCR calculation |
| Head of IT | Owns the systems and the data platform roadmap |

## The engagement

- Team: one manager, one senior consultant, two junior consultants.
- Duration: three weeks.
- Tools: the client's laptops and approved tools. The statement of work states that AI is used for research and drafting, and that the team discloses this in its deliverables.

## Files in this repository

| File | What it is |
| --- | --- |
| `case/01-case-brief.md` | This brief |
| `case/02-sources.md` | The regulation to work with, and where to find it |
| `case/03-fbb-data-governance-policy.md` | FBB's internal policy RDG-01 v2.3 |
| `case/04-fbb-lcr-disclosure.csv` | FBB's LCR disclosure, four quarters, EUR million |
| `case/04-fbb-lcr-disclosure-notes.md` | How to read the disclosure |
| `case/05-fbb-board-deck-draft.pptx` | The draft board deck a junior made with AI |
| `case/05-fbb-board-deck-draft.md` | The same deck as text, so an agent can read it |
