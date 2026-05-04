---
name: forecast
description: >
  Generate a forecast confidence assessment for the current period. Use when the
  user says "forecast", "how's my forecast", "will we hit our number",
  "forecast confidence", "quarter assessment", "are we on track", or asks about
  forecast accuracy or gap analysis.
---

# Forecast

Generate a forecast confidence assessment for the current period.

## Steps

1. Pull `get_forecast_vs_actual` for current and previous periods
2. Pull `get_pipeline_value` for what's still in play
3. Pull `get_deals_at_risk` for threats to forecast
4. Pull `get_win_rate` for current conversion rate
5. Pull `get_deal_velocity` to assess if remaining deals can close in time

## Output Format

**Forecast Assessment — [Quarter/Month]**

**Confidence Level:** [High / Medium / Low]

**The Math:**
- Closed to date: $X
- Remaining target: $Y
- Pipeline available: $Z (at X% win rate = $W expected)
- Gap/surplus: $[difference]

**Risks to the Forecast:**
- [Deals past expected close]
- [Deals with no recent activity]
- [Velocity constraints]

**What Would Need to Happen:**
- Close [X] of [Y] remaining deals
- Required close rate: X% (vs Y% historical)
- [Realistic / Stretch / Unlikely]

**Recommendation:**
[One honest sentence about where the quarter stands]

## Tone

Be honest. Sales leaders need truth, not optimism. If the forecast is at
risk, say so clearly.
