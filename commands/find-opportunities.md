# Find App Opportunities

Use `app-opportunity-discoverer` first to find evidence-backed opportunities in a market, then use `app-opportunity-analyst` to deeply analyze the top candidate.

## Input

```text
Find app opportunities in: <category, audience, platform, or trend>
Builder constraints: <optional stack, time budget, geography, distribution strengths>
```

## Instructions

1. Clarify assumptions if the user did not provide platform, geography, or time budget.
2. Gather current evidence from primary and secondary sources.
3. Identify 5-10 competitors or adjacent products.
4. Extract repeated pain patterns and monetization signals.
5. Generate 3-5 opportunity ideas.
6. Score raw ideas using the discoverer's `references/discovery-scorecard.md`.
7. Recommend one idea for deep analysis.
8. Hand the top idea to `app-opportunity-analyst` for final validation if the user wants a full report.

## Output

Use `templates/opportunity-report.md`.

## Example

```text
Find app opportunities in AI journaling for solo iOS developers.
Builder constraints: SwiftUI, 2-week MVP, English-speaking users, comfortable with TikTok and Reddit distribution.
```
