# The CO-STAR prompt pattern, plus source rules

CO-STAR is a checklist for structured prompts: **C**ontext, **O**bjective, **S**tyle, **T**one, **A**udience, **R**esponse format. For regulatory work, add **source rules**.

## Template

```text
# CONTEXT
<Who you are, who the client is, what situation you're in, and which files to use.>

# OBJECTIVE
<Exactly what should come out. One task per prompt.>

# STYLE
<For example: concise, analytical, plain English, no marketing language.>

# TONE
<For example: neutral and factual. Flag uncertainty explicitly.>

# AUDIENCE
<Who will read the output, and what they already know.>

# RESPONSE FORMAT
<Table, list, or memo. Name the columns or sections.>

# SOURCE RULES
- Use only the files I name. Do not use outside knowledge for regulatory claims.
- For every claim, quote the exact passage you rely on and give its location
  (principle number, section, point or paragraph).
- If you cannot find support, write "not found". Do not guess.
```

## Example for Hands-on 1

Use this as a starting point. Change it so it fits your own plan.

```text
# CONTEXT
I am a manager at a consultancy assessing Fake Bright Bank (FBB) against supervisory
expectations on risk data aggregation and risk reporting. Use these files only:
sources/bcbs239.pdf, sources/ecb-rdarr-guide-2024.pdf and
case/03-fbb-data-governance-policy.md.

# OBJECTIVE
Compare FBB's policy RDG-01 with BCBS 239 and the ECB guide. Identify where the policy
overlaps with, contradicts, or has gaps against the regulation, and where the policy
contradicts itself.

# STYLE
Concise and analytical. One finding per row.

# TONE
Neutral. Mark anything you are unsure about with "uncertain".

# AUDIENCE
A compliance manager who knows the regulation and will check your references.

# RESPONSE FORMAT
A markdown table with these columns:
BCBS 239 principle | ECB guide section | FBB policy clause | Overlap / contradiction / gap | Quote

# SOURCE RULES
- Quote the exact passage from the regulation and the policy clause for every row.
- Give the BCBS 239 principle number and the ECB guide section and point.
- If you cannot find support for a finding, write "not found". Do not guess.
```
