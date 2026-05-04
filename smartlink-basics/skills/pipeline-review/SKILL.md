---
name: pipeline-review
description: >
  Generate a pipeline review brief for a sales leadership meeting. Use when the
  user says "pipeline review", "how's my pipeline", "Monday pipeline meeting",
  "show me the pipeline", "pipeline health", "weekly review", or asks for a
  leadership-ready sales brief.
---

# Pipeline Review

Generate a pipeline review brief for a sales leadership meeting.

## Steps

1. Call `get_pipeline_value` for current pipeline state
2. Call `get_win_rate` trailing 90 days
3. Call `get_deal_velocity` trailing 90 days
4. Call `get_stage_conversion` trailing 90 days
5. Call `get_forecast_vs_actual` current quarter
6. Call `get_deals_at_risk` with 14-day stale threshold

## Output Format

**Pipeline Review — [Date]**

**The Headlines:**
- [1-2 sentence summary of pipeline health]
- [Biggest risk or opportunity]

**By the Numbers:**
- Pipeline: $X across Y deals (Zx coverage)
- Win Rate: X% (trend: up/down/flat)
- Velocity: X days average (trend)
- Forecast: X% accurate this quarter

**Needs Attention:**
- [Specific deals at risk with why]
- [Stage conversion drop-offs]
- [Activity gaps by rep]

**Coaching Priorities This Week:**
1. [Most impactful thing to address]
2. [Second priority if applicable]

## Tone

Write like a sales leader briefing their VP. Direct, specific, no filler.
Every sentence should inform a decision or prompt an action.
