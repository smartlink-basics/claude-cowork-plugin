# SmartLink Basics — Claude Cowork Plugin

Sales CRM tools powered by the SmartLink Basics 6-KPI framework. Built by a sales leader, not a vendor.

## What This Plugin Does

Connects Claude to your SmartLink Basics CRM and gives it the sales coaching methodology to interpret your data — not just report it. When you ask "how's my pipeline?", Claude doesn't dump a spreadsheet. It tells you what needs attention this week and what to coach on.

Built on the **"inspect what you expect"** framework: focus on the 6 metrics that actually drive decisions, and coach your team on what moves deals forward.

## Commands

| Command | What It Does |
|---------|-------------|
| `/smartlink:pipeline-review` | Pulls all 6 KPIs and generates a leadership-ready pipeline brief |
| `/smartlink:deal-check` | Analyzes specific deals for risk — timeline, activity, velocity |
| `/smartlink:coaching-prep` | Prepares 1:1 coaching talking points for a rep with data-backed recommendations |
| `/smartlink:forecast` | Assesses forecast confidence with the math to back it up |

## The 6 Core KPIs

Every command and skill is built around these metrics:

1. **Pipeline Value** — How much is in play and where it sits
2. **Win Rate** — How efficiently you convert opportunities
3. **Deal Velocity** — How fast deals move from creation to close
4. **Activity Rate** — Whether reps are doing enough of the right activities
5. **Stage Conversion** — Where deals die in the funnel
6. **Forecast vs Actual** — Whether the team can predict their own performance

## Skills

The plugin includes two auto-triggered skills that Claude draws on whenever sales topics come up:

- **Sales Coaching** — The "inspect what you expect" methodology, coaching principles, and KPI interpretation framework
- **KPI Analysis** — How to pull, contextualize, and present SmartLink Basics metrics with benchmarks and recommended actions

## Requirements

- A SmartLink Basics CRM account (Growth or Pro tier)
- Claude Pro, Max, Team, or Enterprise plan

## Setup

### Option 1: Install from the Plugin Directory

```
/plugin install smartlink-basics@claude-plugins-official
```

### Option 2: Install from SmartLink Basics Marketplace

```
claude plugin marketplace add smartlink-basics/claude-cowork-plugin
claude plugin install smartlink-basics@smartlink-basics
```

### Option 3: Install Locally

Clone this repo and install from the local path:

```
git clone https://github.com/smartlink-basics/claude-cowork-plugin.git
claude plugin install /path/to/claude-cowork-plugin/smartlink-basics
```

### Connect Your CRM

The plugin connects to your SmartLink Basics CRM automatically via the included MCP server configuration. On first use, you'll authenticate with your SmartLink Basics account.

You can also add the MCP server manually in Claude Desktop under Settings > Connectors:

```
https://imxxpgyszgltjhukgimg.supabase.co/functions/v1/mcp
```

## Quick Start

Once installed, try:

- "Show me my pipeline" — Claude pulls your deal data and breaks it down by stage
- `/smartlink:pipeline-review` — Get a full 6-KPI leadership brief
- "Which deals are at risk?" — Surfaces overdue and stale deals
- `/smartlink:coaching-prep` — Prep for a 1:1 with data-backed talking points

## About SmartLink Basics

SmartLink Basics equips sales leaders with clear dashboards, practical playbooks, and AI automations that replace complexity with results. We align teams around the few metrics that matter, streamline workflows, and accelerate revenue.

**Software Is the Service.** We're operators who build tools, not vendors selling platforms.

- Website: [smartlinkbasics.com](https://smartlinkbasics.com)
- CRM: [crm.smartlinkbasics.com](https://crm.smartlinkbasics.com)
- Support: support@smartlinkbasics.com

## License

MIT
