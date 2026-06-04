---
name: app-opportunity-discoverer
description: Proactively discover and shortlist promising app ideas for indie developers who do not know what to build. Use when asked to find app ideas from scratch, scan markets for opportunities, generate a candidate pool, rank opportunities, or decide which ideas should be analyzed next.
---

# App Opportunity Discoverer

Use this skill when the user does not already have a specific app idea or category. The goal is to proactively generate a ranked shortlist of app ideas from current market signals, then hand the strongest candidates to `app-opportunity-analyst` for deeper validation.

## Core Workflow

1. **Frame builder constraints**
   - Identify platform, stack, time budget, geography, monetization preference, excluded categories, and distribution strengths.
   - If missing, assume a solo indie developer building a 1-2 week MVP for English-speaking users with low budget.

2. **Scan signal buckets**
   - Read `references/discovery-method.md`.
   - Scan at least 4 buckets: app store rankings/search, review pain, product launches, community pain, pricing pages, GitHub/open-source demand, search/video trends.
   - Browse when current market evidence is needed.

3. **Generate raw candidate pool**
   - Generate 10-20 candidate app ideas.
   - Each candidate must include user segment, problem trigger, existing workaround or competitor, monetization hint, distribution wedge, and why a solo developer can build the first version.

4. **Reject weak candidates**
   - Reject ideas with clear reasons: large data dependency, marketplace liquidity, high trust/legal/medical risk, free polished incumbents, or generic "AI for X" framing.

5. **Rank shortlist**
   - Select 3-5 ideas and score them using `references/discovery-scorecard.md`.
   - Prefer ideas with repeated pain, paid competitors, a narrow wedge, feasible MVP, and non-viral distribution.

6. **Handoff**
   - Recommend one idea to analyze first.
   - Include a handoff prompt for `app-opportunity-analyst`.

## Output

Use `templates/idea-discovery-report.md`.

Always include:

- Source scan summary.
- Raw candidate pool.
- Rejected ideas with reasons.
- Ranked shortlist.
- Top recommendation.
- Handoff prompt for deep analysis.
