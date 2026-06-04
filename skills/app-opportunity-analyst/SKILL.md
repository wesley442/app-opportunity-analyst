---
name: app-opportunity-analyst
description: Analyze and validate app ideas or app categories for indie developers using market signals from app stores, competitor reviews, pricing, search demand, social discussions, and launch platforms. Use when the user already has an app idea, app category, or shortlist and needs competitor analysis, opportunity scoring, MVP scope, pricing, risks, or a go/no-go recommendation.
---

# App Opportunity Analyst

Use this skill when the user already has an app idea, app category, or shortlist. The goal is to deeply analyze and validate whether a specific opportunity is worth pursuing.

If the user does not know what to build yet, use `app-opportunity-discoverer` first to generate and rank candidate ideas, then return here for deep analysis.

## Core Workflow

1. **Frame the decision**
   - Identify target platform: iOS, Android, web, browser extension, or cross-platform.
   - Identify builder profile: solo developer, small team, available stack, time budget, budget, distribution strengths.
   - Identify market scope: country/language, B2C/B2B, mobile-first/web-first.
   - If these are missing, assume a solo indie developer building a 1-2 week MVP for English-speaking users.

2. **Gather current evidence**
   - Browse when market facts may have changed.
   - Prefer primary sources: App Store pages, Google Play pages, pricing pages, changelogs, official product sites, Product Hunt listings, public app reviews, GitHub repos.
   - Use secondary sources only for context: market reports, blog posts, newsletters, Reddit/HN threads.
   - Capture source URLs and dates where possible.

3. **Analyze competitors**
   - Find 5-10 direct or adjacent competitors.
   - Compare positioning, rating/reviews, pricing, monetization, core features, complaint patterns, and gaps.
   - Look for painful reviews: expensive, confusing, missing feature, bad onboarding, privacy concern, poor localization, weak AI quality, bad export/import, no team support.

4. **Score opportunities**
   - Use `references/scoring-rubric.md` when ranking ideas or deciding go/no-go.
   - Score demand, willingness to pay, competition, build feasibility, distribution feasibility, retention risk, and indie fit.
   - Be conservative: a high score needs evidence, not just plausible demand.

5. **Generate output**
   - For category analysis, use `templates/opportunity-report.md`.
   - For validating one idea, use `templates/validation-report.md`.
   - For building next, use `templates/app-mvp-brief.md`.

## Output Rules

- Separate evidence from interpretation.
- Always include a go/no-go or ranked recommendation.
- Every recommended idea must include a concrete wedge: niche, user segment, workflow, distribution channel, or platform constraint.
- Prefer small, testable MVPs over broad app concepts.
- Include a 7-day validation plan before suggesting a full build.
- State unknowns and data gaps clearly.

## When To Read References

- Read `references/scoring-rubric.md` before scoring opportunities.
- Read `references/data-sources.md` when choosing sources or explaining evidence quality.
- Read `references/report-methodology.md` when producing a full report or when source evidence conflicts.
