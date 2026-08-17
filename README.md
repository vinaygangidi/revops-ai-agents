# revops-ai-agents

Claude Code subagent definitions for RevOps analysis: win-loss, MEDDIC scoring, churn and deal risk.

![Type](https://img.shields.io/badge/type-Claude%20Code%20agents-blue?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/vinaygangidi/revops-ai-agents?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

## What This Does

Seven Claude Code subagent definitions that analyze Revenue Operations data. Each one is a
markdown file with a role prompt and a fixed output format: point it at CSV exports and
call transcripts, and it writes a structured report.

There is no application code here — no Python, no dependencies, no build. The runtime is
the Claude Code CLI, which reads the agent definitions from `.claude/agents/`. Sample CRM
data and example outputs are included so the agents run without connecting to a real CRM.

## How It Works

1. Claude Code discovers the agent definitions in `.claude/agents/`.
2. You invoke an agent by name, or point at its file directly.
3. The agent reads `data/crm/*.csv` and `data/transcripts/*.txt` using `Read`, `Grep`,
   `Glob`, and `Bash` — the four tools each definition permits.
4. It writes a markdown report following the output format in its prompt.

Agents are independent. None calls another, and there is no pipeline or orchestration —
each is invoked by hand and does one job.

### Agents

| Agent | What It Does | Suggested Cadence |
|---|---|---|
| `win-loss-analyst` | Patterns in closed deals by segment, competitor, size, and rep | Month or quarter end, min. 10 closed deals |
| `icp-analyst` | Builds an ICP from closed-won data, ranked by ACV and cycle length | Quarterly, or when win rates drop |
| `competitive-intel` | Battlecards from what buyers actually say in deal notes | Monthly, or when a competitor recurs |
| `churn-detector` | Flags declining engagement, support load, contacts going dark | Weekly or monthly |
| `deal-risk-assessor` | Scores open deals 1–10 on health with risks and rep actions | Mondays, before pipeline review |
| `meddic-checker` | Scores deals against MEDDIC, generates gap questions | Before stage advancement |
| `objection-mapper` | Groups late-stage objections with counts and winning responses | Weekly across late-stage deals |

All seven run on `sonnet`.

## Quickstart

1. Install the [Claude Code CLI](https://code.claude.com) and sign in.

2. Clone the repository:
   ```bash
   git clone https://github.com/vinaygangidi/revops-ai-agents.git
   cd revops-ai-agents
   ```

3. Run an agent against the included sample data:
   ```bash
   claude "Run the win-loss-analyst agent on all closed deals"
   ```

   Or invoke a definition directly:
   ```bash
   claude --agent .claude/agents/deal-risk-assessor.md "Score every open deal"
   ```

4. Reports are written to `data/reports/`. Six example outputs are already committed there
   so you can see the expected shape before running anything.

5. To use your own data, replace the CSVs in `data/crm/` keeping the same column names —
   the agent prompts reference these fields directly. See the schema below.

## Configuration

There are no environment variables. Nothing in this repository reads configuration — there
is no code to read it. Behavior is controlled by the agent markdown files and the input
data.

| Input | Required | Default | Description |
|---|---|---|---|
| `data/crm/deals.csv` | Yes | 40 sample rows | Deal records. 25 columns including `stage`, `status`, `acv`, `segment`, `meddic_score`, `competitor_mentioned`, `closed_lost_reason`, `champion_identified`, `economic_buyer_met`, `close_date_pushed_count` |
| `data/crm/accounts.csv` | For `churn-detector` | 23 sample rows | Account records with `nps_score`, `health_score`, `monthly_active_users`, `support_tickets_open`, `renewal_date` |
| `data/crm/contacts.csv` | For `meddic-checker` | 24 sample rows | Contacts with `title`, `role_in_deal`, `email_engagement` |
| `data/crm/activities.csv` | For `objection-mapper` | 51 sample rows | Activity log with `activity_type`, `subject`, `notes` |
| `data/transcripts/*.txt` | For `competitive-intel`, `objection-mapper` | 5 sample calls | Call transcripts, named `<deal_id>_<account>_<type>.txt` |
| `.claude/agents/*.md` | Yes | 7 definitions | Agent role prompts. Each declares `name`, `description`, `tools`, `model` |

## Limitations

- **Not runnable code.** No Python, no `package.json`, no dependencies. This is a prompt
  library that requires the Claude Code CLI and a paid Claude subscription.
- **Seven agents, not sixteen.** Earlier versions of this README advertised 16 agents
  across four sections. Nine were never written. The nine absent ones were
  `call-summarizer`, `forecast-predictor`, `coverage-analyzer`, `pipeline-hygiene`,
  `scenario-planner`, `call-coach`, `crm-updater`, `methodology-summarizer`, and
  `followup-drafter`. This README now lists only what exists.
- **Sample data is synthetic and small.** 40 deals, 23 accounts, 24 contacts, 51
  activities, 5 transcripts. Enough to demonstrate output shape, not enough for the
  statistical claims some agents make — `win-loss-analyst` asks for at least 10 closed
  deals, which the sample barely clears.
- **Output is not deterministic.** These are LLM prompts, so two runs on identical input
  can differ in wording, emphasis, and which patterns get surfaced. The committed reports
  in `data/reports/` are one sample run, not a fixed expected output.
- **No CSV schema validation.** If your export is missing a column an agent references,
  the agent will improvise or silently skip that analysis rather than fail loudly.
- **No tests.** The committed reports could serve as golden fixtures, but nothing compares
  against them.
- **Agents have `Bash` access.** Each definition grants `Read`, `Grep`, `Glob`, and
  `Bash`. `Bash` is broader than these read-only analysis tasks require — worth narrowing
  if you point these at real data.
- **Your CRM data goes to the Claude API.** Whatever CSVs and transcripts you place in
  `data/` are sent to Anthropic when an agent runs. Do not add customer data your
  agreements prohibit sending to third-party processors.
- **`scripts/` and `docs/` are empty.** Both exist as placeholder directories.

## License

MIT — see [LICENSE](LICENSE).
