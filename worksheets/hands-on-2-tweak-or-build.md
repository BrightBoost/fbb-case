# Hands-on 2: Tweak it or build your own (40 min)

Choose a track. Most people start with Track 1. If you finish early, try the other one.

---

## Track 1: Tweak the template (30 min)

1. **Copy the agent.** Copy `.github/agents/reference-number-checker.agent.md` to `.github/agents/my-checker.agent.md`.
2. **Rename it.** In the frontmatter, change `name:` to something of your own, for example `My Checker (your name)`.
3. **Add one check of your own.** Use the issue you wrote on the flip chart at the start of the afternoon: the one you'd want an agent to catch first. Add it as a step under *Procedure*.
4. **Shape the output for you.** Change the *Output* section so the report shows what you, as a manager, want to see first. For example: only the issues, sorted by severity, with a one-line recommendation per issue.
5. **Run it.** Start a new session, pick your agent in the agent picker, and ask it to check:
   - `case/05-fbb-board-deck-draft.md` (the deck from Session 1)
   - your own table from Hands-on 1 (`reviews/hands-on-1-structured.md`)

## Track 2: Build from scratch (30 min)

1. Copy `templates/agent-skeleton.agent.md` to `.github/agents/<your-agent-name>.agent.md`.
2. Write an agent for a different check. Two ideas:
   - **Policy contradiction finder:** reads FBB's policy and lists every place where the policy contradicts itself, with both quotes.
   - **Focus reviewer:** reads the board deck and the problem-setting brief, and tells you which slides the board doesn't need for its decision, and why.
3. Optional: add an MCP server so your agent can read PDFs or PowerPoint files directly. See `docs/adding-an-mcp-server.md`.
4. Run it and refine the instructions at least once.

---

## Last 10 minutes: compare in pairs

Pair up with someone, ideally from the other track.

| Question | Your notes |
| --- | --- |
| What did your agent catch? | |
| What did it miss? | |
| What did it get wrong? | |
| How would you know, in daily work, that it missed something? | |
