# Hands-on 1: From regulation to requirements (70 min)

You run the full workflow yourself: navigate, plan, prompt, verify and iterate. You work on the chain **regulation → policy → requirements → data definitions**, using FBB's data governance policy.

Work alone or in pairs. We pause briefly after each step.

Files you need:
- `sources/bcbs239.pdf` and `sources/ecb-rdarr-guide-2024.pdf`
- `case/03-fbb-data-governance-policy.md`
- `templates/co-star-prompt.md` and `templates/gap-analysis-table.md`

---

## Step 1: Navigate the pile (10 min)

When you face a lot of text, ask for a **map**, not a summary.

1. Ask Copilot which sections of BCBS 239 and the ECB guide deal with:
   - data ownership
   - reconciliation of risk data
   - reporting frequency and timeliness

   Ask for principle numbers and ECB sections and points.
2. Ask: *"Where should a human reviewer look first, and why?"*
3. **Spot-check two references.** Open the PDF and find them yourself. Do they exist, and do they say what the map says?

Note here what you found:

>

## Step 2: Plan with AI (10 min)

1. Ask Copilot to propose a plan for a gap analysis of FBB's policy against BCBS 239 and the ECB guide.
2. **Change the plan.** Remove what doesn't serve the board's question, add what's missing, and reorder it. You set the direction.

Your final plan, in three to five steps:

1.
2.
3.

## Step 3: Prompt beyond the basics (20 min)

1. **One-line prompt.** Start a new session and type:
   *"Compare the FBB policy with BCBS 239."*
   Save the output as `reviews/hands-on-1-one-line.md`.
2. **Structured prompt.** Start a new session. Write a structured prompt using `templates/co-star-prompt.md`. You can start from the example in that file, but make it your own. Ask for the output table from `templates/gap-analysis-table.md`.
   Save the output as `reviews/hands-on-1-structured.md`.
3. **Compare** the two outputs side by side. What is different? Which one could you defend in front of a client?

## Step 4: Verify (15 min)

1. Pick **three rows** from your structured output.
2. For each row, open the source and the policy:
   - Does the quoted passage exist?
   - Does it say what the row claims?
   - Is the policy clause quoted correctly?
3. Find **at least one row where the AI is wrong**, and name the failure pattern (see `templates/four-review-questions.md`).

| Row | Correct? | If wrong: failure pattern |
| --- | --- | --- |
| | | |
| | | |
| | | |

## Step 5: Iterate (15 min)

1. Tell Copilot what it got wrong, and why.
2. Change your prompt so it doesn't happen again, and run it once more.
3. Optional: run the same prompt with a second model from the model picker and compare.
4. Pick three requirements from your table and turn them into draft data definitions in `templates/gap-analysis-table.md`: data element, owner, frequency and reconciliation rule.

What did you change in your prompt, and what difference did it make?

>
