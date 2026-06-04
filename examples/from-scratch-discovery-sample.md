# Example Report: From-Scratch App Idea Discovery

Evidence style: illustrative sample. Replace sources with fresh evidence before using for a real build decision.

## Decision

What should a solo indie developer investigate next if they do not know what app to build?

## Builder Assumptions

- Platform: iOS or web.
- Time budget: 1-2 week MVP.
- Tech stack: SwiftUI or Next.js.
- Geography/language: English-speaking users.
- Distribution strengths: Reddit, X, SEO, App Store search.

## Source Scan Summary

| Signal Bucket | Sources Checked | Useful Signals Found | Confidence |
|---|---|---|---|
| App store rankings/search | App Store and Google Play category searches | Paid consumer utilities remain viable when workflow is frequent | Medium |
| Review pain | Popular productivity, nutrition, note, plant, and document apps | Repeated complaints around pricing, export, complexity, and privacy | Medium |
| Product launches | AI notes, personal productivity, browser tools | Many products launch around capture, summarization, and automation | Medium |
| Community pain | Reddit/HN productivity, iOS, freelancer, PKM discussions | Users ask for simpler alternatives and migration paths | Medium |
| Pricing/monetization | Competitor pricing pages and IAP listings | Subscriptions are common, but one-time purchase can be a wedge | Medium |

## Raw Candidate Pool

| Candidate | User Segment | Problem Trigger | Monetization Hint | Distribution Wedge | Keep? |
|---|---|---|---|---|---|
| Private voice memory app | Founders/writers/ADHD users | Voice notes are hard to search and export | Subscription or local lifetime purchase | PKM and productivity communities | Yes |
| MyFitnessPal switcher | Macro trackers | Redesigns, clutter, migration pain | Low yearly subscription | "Alternative to MyFitnessPal" SEO | Yes |
| Pet-safe plant inventory | Pet owners with houseplants | Unsure which plants are toxic | Yearly subscription or one-time audit | TikTok/SEO around toxic plants | Yes |
| Receipt scanner for freelancers | Freelancers | Monthly reimbursement/tax admin | Yearly subscription | Freelancer tax content | Yes |
| AI habit tracker | Self-improvement users | Generic trackers do not adapt | Subscription | TikTok demos | Maybe |
| Meeting bot for sales teams | B2B sales teams | CRM note capture | Team subscription | LinkedIn outbound | No |
| AI recipe generator | Home cooks | Meal planning fatigue | Subscription | SEO | No |
| Travel itinerary AI app | Travelers | Planning overload | Freemium | Travel TikTok | No |

## Rejected Ideas

| Idea | Why Rejected |
|---|---|
| Meeting bot for sales teams | Crowded B2B category, sales integrations increase scope, support burden high |
| AI recipe generator | Too generic, weak retention, many free alternatives |
| Travel itinerary AI app | Seasonal use, many competitors, hard to monetize without bookings |

## Ranked Shortlist

| Rank | Idea | User Wedge | Score | Evidence Strength | Main Risk |
|---:|---|---|---:|---|---|
| 1 | Private voice memory app | People who think out loud and need searchable notes | 81 | Medium | Transcription cost and crowded market |
| 2 | MyFitnessPal switcher | Frustrated macro tracking power users | 77 | Medium | Food database coverage |
| 3 | Pet-safe plant inventory | Pet owners and parents with houseplants | 74 | Medium | Safety/trust risk |
| 4 | Receipt scanner for freelancers | Solo freelancers doing monthly admin | 72 | Weak-medium | OCR/export accuracy |

## Top Recommendation

- Idea: Private voice memory app.
- One-line concept: Record quick thoughts and turn them into searchable, exportable Markdown notes.
- Why this one: It has frequent use, a narrow workflow, privacy/export differentiation, and a feasible MVP.
- Why now: Users are becoming comfortable with AI notes, but many tools are meeting-first or team-first.
- Why a solo developer: The first version can focus on capture, transcript, summary, search, and export.
- Main risk: Heavy users can create high transcription costs.

## MVP Scope

- Must-have: One-tap recording, transcript, summary, search, Markdown export.
- Nice-to-have: Obsidian/Notion export, local transcription for short notes.
- Excluded: Meeting bots, team collaboration, video call integration.
- Pricing hypothesis: Free 10 notes/month, $4.99/month or $39/year.
- First distribution channel: PKM/productivity communities and X demos.

## 7-Day Validation Plan

| Day | Action | Success Signal |
|---:|---|---|
| 1 | Publish a landing page with 3 mock screenshots | 30 waitlist signups |
| 2 | Post prototype flow in productivity and PKM communities | 10 specific pain comments |
| 3 | Offer manual transcript + Markdown export | 5 users submit real audio |
| 4 | Interview users about privacy and export | 3 users ask for Obsidian/Notion |
| 5 | Test pricing page | 3 users choose a paid tier |
| 6 | Build clickable prototype | 8/10 complete record-to-export |
| 7 | Decide build/no-build | Continue if users ask for repeat use |

## Next Analysis Needed

- Fresh competitor review mining.
- Real App Store keyword search.
- Transcription cost model.
- Landing page conversion test.

## Handoff To Analyst

```text
Use app-opportunity-analyst to deeply validate this idea:

Idea: Private voice memory app that turns quick recordings into searchable, exportable Markdown notes.
Target user: Founders, writers, ADHD users, and PKM users who think out loud.
Platform: iOS first, Mac optional.
Key evidence: AI notes demand is visible, meeting-first products leave a personal-memory gap, privacy and export are repeated concerns.
Main risks: Transcription cost, crowded category, local model performance.
Builder constraints: Solo developer, SwiftUI, 1-2 week MVP, low budget.
```
