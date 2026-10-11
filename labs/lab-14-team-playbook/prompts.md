# Prompts — Lab 14: Measure, Version and Write the Team Playbook

**Use: Claude Code — Code mode (the </> button) in the Claude desktop app, in your horizon-studio folder.** Paste each prompt as written; change only what the lab tells you to.

**Easiest:** copy each prompt from https://tertiarycourses.github.io/TGS-2023018659-Claude-Cowork-for-Digital-Marketing/prompts/claude/#lab-14 (one Copy button per prompt).

## PROMPT A — Claude Code: compare

```
Use the growth-analyst subagent. From
data/run-log.csv compare the patterns we used —
one agent, subagents, agent teams and the scheduled task
— on minutes, tokens, defects caught before a person
and human edits. Which pattern pays off for which
job? Save reports/agent-comparison.md.
Publish it as an artifact: one chart per measure,
comparing the patterns.
Write for a business owner, in plain English: no
codes, IDs, file names or line numbers; start with
what it means and what I do next. Save a Word copy
(.docx) of each result.
```

## PROMPT B — Claude Code: the playbook

```
Write strategy/team-playbook.md with
data/playbook-outline.md. Include the roster: for
each agent its instructions file in .claude/agents/, its
skills, connectors, model and what it may never do;
the approval matrix by risk; the rules in
data/responsible-ai-checklist.md; and what to do when
a wrong post goes out. Then run fin-compliance on
it.
Publish the playbook as an artifact: the roster as
cards, the approval matrix as a table.
Write for a business owner, in plain English: no
codes, IDs, file names or line numbers; start with
what it means and what I do next. Save a Word copy
(.docx) of each result.
```

## PROMPT C — Claude Code: version and propose a change

```
Keep a version history of this folder (use git;
set it up if it is not there yet). Save everything
as version 1.0 with the note "The team as built in
class".
From reports/agent-comparison.md and
data/run-log.csv, propose ONE change to how the team
works. Write review/change-proposal.md: what we saw,
the change, the files it touches, how we test it,
the risk, who approves, and how we roll back.
Make the change, test it on one recent piece with
fact-check and fin-compliance, and save version 1.1
with a one-line note. Show me what changed between
1.0 and 1.1, and how to go back to 1.0.
Publish the proposal and the version history as an
artifact.
Write for a business owner, in plain English: no
codes, IDs, file names or line numbers; start with
what it means and what I do next. Save a Word copy
(.docx) of each result.
```

## Ask about the result

Once a result opens, type any of these in the chat to get its meaning. Ask until it makes sense to you — then decide.

- "In one line each: when should we use one agent, subagents and an agent team?"
- "Who must approve a post that has a CPF figure in it?"
- "A wrong post went out. What are the first three things we do?"
- *After Prompt C:* "In plain English, what changed in version 1.1, and how would we undo it?"
