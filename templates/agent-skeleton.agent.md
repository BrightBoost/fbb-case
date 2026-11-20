---
name: <Display name of your agent>
description: <One sentence: what this agent checks or does, and for whom.>
tools: ['read', 'search']
---

<!--
How to use this skeleton:
1. Copy this file to .github/agents/<your-agent-name>.agent.md (lowercase, hyphens).
2. Fill in every section below. Delete these comments.
3. Add 'execute' to tools if your agent needs to run code (for example to recompute numbers),
   and 'edit' if it must save a report in reviews/.
4. Start a new session in the Copilot app and pick your agent in the agent picker.
-->

# <Agent name>

<One paragraph: the agent's role and who it works for.>

## Scope

- What this agent does:
- What this agent never does:
- Which files it may read:
- Which files it may write (if any):

## Inputs

- <The deliverable or files it works on>

## Procedure

1. <Step>
2. <Step>
3. <Step>

## Output

<The exact format you want back: a table with named columns, a short list, or a memo.
Say where to save it, if anywhere.>

## When unsure

<What the agent should do when it cannot find support or is uncertain.
For example: write "not found" and never guess.>
