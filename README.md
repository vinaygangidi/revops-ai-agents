# 🚀 RevOps AI Agents for Claude Code

16 specialized AI agents that automate Revenue Operations workflows, built for [Claude Code CLI](https://code.claude.com).

## What This Does

Each agent is a purpose-built AI workflow that takes your CRM data, call transcripts, and pipeline info as input — and delivers structured, actionable output: scorecards, risk assessments, coaching reports, and more.

**No CRM integration required.** Export your data as CSV, point the agent at it, and go.

## Agents

### Section 2: Revenue Intelligence
| Agent | What It Does |
|-------|-------------|
| `win-loss-analyst` | Patterns across closed deals — why you win, why you lose |
| `icp-analyst` | Builds your ICP from actual closed-won data |
| `competitive-intel` | Live battlecards from what buyers say in deals |
| `churn-detector` | Early warning signals before customers leave |

### Section 3: Deal Intelligence
| Agent | What It Does |
|-------|-------------|
| `deal-risk-assessor` | 1-10 health score with evidence for every deal |
| `objection-mapper` | Surfaces and groups objections from late-stage deals |
| `meddic-checker` | Scorecard showing confirmed/weak/missing MEDDIC elements |
| `call-summarizer` | Structured call summary ready to paste into CRM |

### Section 4: Pipeline & Forecast
| Agent | What It Does |
|-------|-------------|
| `forecast-predictor` | Best/base/worst revenue scenarios with assumptions |
| `coverage-analyzer` | Pipeline coverage by rep and segment with gap actions |
| `pipeline-hygiene` | Flags stale deals, pushed dates, missing fields |
| `scenario-planner` | Board-ready scenario planning table |

### Section 5: AI Productivity
| Agent | What It Does |
|-------|-------------|
| `call-coach` | Scores calls on discovery, objection handling, next steps |
| `crm-updater` | Extracts CRM-ready fields from call summaries |
| `methodology-summarizer` | MEDDIC-mapped call summary with gap questions |
| `followup-drafter` | Personalized follow-up email from call summary |

## Quick Start

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/revops-ai-agents.git
cd revops-ai-agents

# 2. Start Claude Code
claude

# 3. Run an agent
> Run the win-loss-analyst agent on all closed deals from Q4
```

## Project Structure

```
revops-ai-agents/
├── CLAUDE.md                  # Project context (Claude reads this first)
├── .claude/
│   └── agents/                # All 16 agent definitions
│       ├── win-loss-analyst.md
│       ├── deal-risk-assessor.md
│       └── ...
├── data/
│   ├── crm/                   # CSV exports (deals, accounts, contacts, activities)
│   ├── transcripts/           # Call transcript .txt files
│   └── reports/               # Agent output goes here
├── scripts/                   # Helper scripts
└── docs/                      # Documentation
```

## Requirements

- [Claude Code CLI](https://code.claude.com) installed
- Claude Pro, Team, or Enterprise subscription
- Your CRM data exported as CSV (sample data included)

## License

MIT
