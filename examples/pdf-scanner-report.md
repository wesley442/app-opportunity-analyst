# Example Report: PDF Scanner App

## Decision

Should a solo indie developer build another PDF scanner app?

## Executive Takeaway

- Verdict: Avoid broad scanner; validate a narrow workflow.
- Best wedge: Receipt and reimbursement scanner for freelancers who need clean exports to accounting tools.
- Why now: Generic scanning is commoditized, but vertical workflows still create value.
- Biggest risk: App stores are crowded with mature scanner apps.
- Recommended next step: Validate one export workflow with freelancers before building camera features.

## Category Snapshot

- Category: PDF scanning, OCR, document cleanup.
- Target users: Students, office workers, freelancers, small businesses.
- Jobs to be done: Scan paper, clean image, OCR, export/share, store documents.
- Monetization patterns: Subscription, lifetime unlock, ads in free apps.

## Competitor Matrix

| Product | Platform | Positioning | Monetization | Strength | Weakness / Complaint | Gap |
|---|---|---|---|---|---|---|
| Adobe Scan | iOS/Android | Free scanner tied to Adobe ecosystem | Adobe upsell | Brand trust and OCR | Heavy ecosystem | Lightweight vertical workflow |
| CamScanner | iOS/Android | Full scanner suite | Subscription | Mature feature set | Price/trust concerns in some markets | Simple trustworthy niche tool |
| Genius Scan | iOS/Android | Professional scanning | Subscription/lifetime | Clean utility | Generic document workflow | Specialized exports |
| Microsoft Lens | iOS/Android | Office document capture | Free | Free and integrated | Less specialized | Paid vertical features are hard |

## Pain Patterns

1. Generic scanning is already solved by free incumbents.
2. Users dislike aggressive subscriptions for basic scanning.
3. Real unmet value is downstream: naming, filing, extracting, exporting, reimbursement, compliance.

## Opportunity Ideas

| Idea | User Wedge | Score | Why It Could Work | Main Risk |
|---|---|---:|---|---|
| Freelancer receipt scanner | Freelancers | 74 | Clear recurring admin workflow | Accounting integrations can expand scope |
| Student assignment scanner | Students | 58 | Easy distribution | Low willingness to pay |
| Medical document organizer | Caregivers | 70 | Painful workflow and high value | Privacy/support burden |

## Recommended MVP

- One-line concept: Scan receipts, auto-name them, extract totals, and export monthly reimbursement packets.
- Must-have features: Receipt capture, auto-crop, merchant/date/amount extraction, monthly PDF/CSV export.
- Deliberately excluded: General document cloud, team sharing, broad OCR editor.
- Pricing hypothesis: $19/year for unlimited exports.
- Distribution wedge: SEO and community content around freelancer tax receipt workflows.

## Final Recommendation

Do not build a broad PDF scanner. Build only if the first version owns a narrow, repeated document workflow.
