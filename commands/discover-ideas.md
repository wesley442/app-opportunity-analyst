# Discover App Ideas From Scratch

Use the `app-opportunity-discoverer` skill when the user does not know what app to build.

## Input

```text
Discover app ideas for me.
Optional constraints: <platform, stack, time budget, geography, interests, excluded categories, distribution strengths>
```

## Instructions

1. Do not require the user to provide an app idea.
2. If constraints are missing, assume a solo indie developer building a 1-2 week MVP for English-speaking users.
3. Read `references/discovery-method.md`.
4. Scan at least 4 signal buckets:
   - App store rankings/search.
   - Review pain.
   - Product launches.
   - Community pain.
   - Pricing/monetization.
   - GitHub/open-source demand.
   - Search/video trends.
5. Generate 10-20 raw candidate ideas.
6. Reject weak ideas with explicit reasons.
7. Score the top 3-5 using `references/discovery-scorecard.md`.
8. Recommend one idea to validate first.
9. Include a handoff prompt for `app-opportunity-analyst`.

## Output

Use `templates/idea-discovery-report.md`.

## Example

```text
Discover app ideas for me.
Optional constraints: solo developer, SwiftUI or Next.js, 2-week MVP, wants subscription or one-time purchase, no marketplace ideas.
```
