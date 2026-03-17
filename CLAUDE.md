# RevOps AI Agents

## Project Overview
This repo contains 16 AI-powered RevOps workflow agents built for Claude Code CLI.
Each agent is a specialized subagent that processes CRM data, call transcripts, and pipeline information to automate Revenue Operations tasks.

## Business Context
- **Company type:** B2B SaaS
- **Sales methodology:** MEDDIC
- **CRM:** Sample data in `/data/crm/` (CSV format)
- **Call transcripts:** Sample transcripts in `/data/transcripts/`
- **Reports output:** Generated reports go to `/data/reports/`

## Data Files
- `data/crm/deals.csv` — All deals (open + closed) with stage, ACV, dates, reps, segments
- `data/crm/accounts.csv` — Customer accounts with firmographics, NPS, usage metrics
- `data/crm/contacts.csv` — Stakeholders and decision-makers per account
- `data/crm/activities.csv` — Emails, calls, meetings logged per deal
- `data/transcripts/` — Call transcript files (one .txt per call)

## Agent Conventions
- Agents live in `.claude/agents/` as markdown files
- Each agent has a clear role, allowed tools, and structured output format
- Agents read from `/data/` and write reports to `/data/reports/`
- All output should be structured (tables, scorecards, ranked lists)
- Agents should cite specific evidence from the data for every finding

## How to Run
```bash
# Run any agent by name
claude "Run the win-loss-analyst agent on deals from Q4"

# Or invoke directly
claude --agent .claude/agents/win-loss-analyst.md "Analyze closed deals from last quarter"
```

## Workflow Sections
1. **Revenue Intelligence** — Win/Loss, ICP Analysis, Competitive Intel, Churn Signals
2. **Deal Intelligence** — Deal Risk, Objections, MEDDIC Compliance, Call Summaries
3. **Pipeline & Forecast** — Forecast Prediction, Coverage Analysis, Pipeline Hygiene, Scenario Planning
4. **AI Productivity** — Call Coaching, CRM Updates, Methodology Summaries, Follow-Up Emails
