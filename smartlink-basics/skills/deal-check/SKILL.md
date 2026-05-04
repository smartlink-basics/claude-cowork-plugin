---
name: deal-check
description: >
  Analyze specific deals for risk and coaching opportunities. Use when the user
  says "check this deal", "deal health", "deal risk", "analyze my deals",
  "which deals are at risk", "deals need attention", or asks about a specific
  deal by name.
---

# Deal Check

Analyze specific deals for risk and coaching opportunities.

## Steps

1. Ask which deal(s) to analyze (by name, stage, rep, or "at risk")
2. Pull relevant deals using `get_deals` with appropriate filters
3. For each deal, assess timeline risk, activity risk, amount risk, velocity risk

## Output Format

**Deal Check — [Deal Name]**

**Status:** [Stage] | $[Amount] | Owner: [Rep] | Expected Close: [Date]

**Risk Assessment:** [Low / Medium / High]
- [Specific risk factors]

**Recommended Next Action:**
[One specific thing the rep should do this week]

**Coaching Question for 1:1:**
"[A question the leader can ask about this deal]"

## Tone

Be direct and specific. "This deal has been in Proposal for 23 days — your
average is 11" is better than "This deal may be at risk."
