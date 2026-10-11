# Prompts — Lab 04: Connect the Tools and Check Compatibility

**Use: Claude Code — Code mode (the </> button) in the Claude desktop app, in your horizon-studio folder.** Paste each prompt as written; change only what the lab tells you to.

**Easiest:** copy each prompt from https://tertiarycourses.github.io/TGS-2023018659-Claude-Cowork-for-Digital-Marketing/prompts/claude/#lab-4 (one Copy button per prompt).

## PROMPT A — Claude Code: give each agent its connectors

```
Read data/connectors-setup.md. For each
subagent in .claude/agents/, replace its tools line
with the one given there, add the disallowedTools
line where one is given, and update its
"Connectors" section: what it may use, and that
Gmail is drafts only. Change nothing else.
```

## PROMPT B — Claude Code: test each agent

```
First tell me which connectors and plugins you
can use.
Then run these five checks, each by its own subagent:
1. growth-strategist: Firecrawl — search for one
   2026 news item about financial planning in
   Singapore, scrape it and cite it.
2. growth-analyst: Google Drive — read
   firm-metrics.csv from Horizon Studio; report
   average monthly enquiries.
3. content-creator: Gmail — a DRAFT to me with the
   subject "Connector test". Do not send.
4. creative-designer: render a 1080x1080 test card
   in Horizon colours and save it in content/test/.
5. website-designer: built-in browser — open our
   own copy of the site (web/site/index.html) at
   375px wide and report any problem.
Report each result in one line. If a check fails,
say which tool was missing.
```

## PROMPT C — Claude Code: the compatibility matrix

```
Act as our integration checker. Make a
compatibility matrix for the team: one row for each
agent and each system it connects to (Google Drive,
Gmail, Google Calendar, Firecrawl, the built-in
browser, our website). For each row give the
interface (connector, file or browser), what the
agent's job needs, the access it has now, the result
of its test in Prompt B, and a status: Compatible,
Conditional or Blocked — with the fix for anything
not Compatible. Flag any agent with more access
than its job needs. Save it as
reports/compatibility-matrix.md and publish it as an
artifact in plain English, coloured by status.
```
