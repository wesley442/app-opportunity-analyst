# Opportunity Scoring Rubric

Score each dimension from 1 to 5, then convert to a 100-point score.

| Dimension | Weight | 1 | 3 | 5 |
|---|---:|---|---|---|
| Demand Signal | 20 | Mostly speculative | Some search/social/review signal | Multiple current signals across sources |
| Willingness To Pay | 20 | Free-user behavior | Some paid competitors | Clear subscription/IAP/B2B spend evidence |
| Competition Gap | 15 | Crowded with polished incumbents | Crowded but complaint clusters exist | Clear underserved niche or workflow |
| Build Feasibility | 15 | Needs deep infra/data/network effects | Buildable in 4-8 weeks | MVP possible in 1-2 weeks |
| Distribution Feasibility | 15 | No obvious channel | Some SEO/community/app store keywords | Clear reachable channel or keyword wedge |
| Retention Potential | 10 | One-time use only | Occasional utility | Recurring habit/workflow/data lock-in |
| Indie Fit | 5 | Requires team/capital | Possible but stretched | Solo-friendly scope and support load |

Formula:

```text
score = demand*4 + pay*4 + gap*3 + build*3 + distribution*3 + retention*2 + indie*1
```

Maximum raw score is 100.

## Recommendation Bands

| Score | Verdict | Meaning |
|---:|---|---|
| 85-100 | Strong pursue | Build or pre-sell if evidence is fresh |
| 70-84 | Validate first | Good candidate, but one or two risks need testing |
| 55-69 | Watchlist | Interesting, but needs sharper niche or data |
| 0-54 | Avoid for now | Too vague, too crowded, or weak evidence |

## Red Flags

- Existing top competitors have strong ratings, mature features, and low prices.
- Idea depends on paid data access before value is proven.
- User pain is real but not frequent enough to retain.
- Acquisition relies on "going viral" without a repeatable channel.
- AI feature can be copied by incumbents with better distribution.

## Strong Signals

- Review clusters show repeated unmet needs in paid apps.
- Users complain about pricing but still pay.
- Competitors have high revenue proxies despite mediocre UX.
- A niche has repeated workflows, templates, exports, or compliance needs.
- Existing products are horizontal, but a vertical workflow is underserved.
