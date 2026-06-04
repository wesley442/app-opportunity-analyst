# Discovery Scorecard

Use this lightweight score when ranking raw ideas before deep analysis.

Score each dimension 1-5:

| Dimension | 1 | 3 | 5 |
|---|---|---|---|
| Signal Strength | Mostly speculative | Some public signal | Multiple current signals |
| Pain Frequency | Rare or one-off | Occasional repeated pain | Frequent workflow pain |
| Monetization Hint | No paid alternatives | Some paid tools | Clear subscriptions/IAP/B2B spend |
| Indie Buildability | Too large | Buildable with scope cuts | 1-2 week MVP is realistic |
| Distribution Wedge | No clear channel | Some community/SEO angle | Clear reachable audience |
| Differentiation | Generic | Some niche angle | Sharp workflow/user wedge |

Formula:

```text
score = signal*4 + pain*4 + monetization*4 + buildability*3 + distribution*3 + differentiation*2
```

Maximum score is 100.

Discovery score is a triage score, not a final build decision. Send the top idea to `app-opportunity-analyst` for deeper validation.
