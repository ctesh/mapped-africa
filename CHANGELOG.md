# mapped.africa — changelog

Versioning scheme:
- **Site**: `site-v<major>.<minor>` — bumped on every meaningful public change (this file is the record).
- **Mapped Score™ (the metric)**: `mapped-score-v<major>.<minor>` — the 7 dimensions, 14 questions, scoring formula and 5 levels are FROZEN per version. Any change to the measurement itself requires a version bump here and in the `data-mapped-score-version` attribute in clarity-check.html, so scores stay comparable over time.

## site-v2.0 (Phase 1) — 2026-07-06 · branch `2-phase1`
- **Mapped Score™ v1.0 ships** (clarity-check.html, URL kept for continuity): 7 dimensions × 2 questions, 5 levels (Invisible / Founder-Dependent / Partially Visible / Managed / Adaptive), founder-dependency flag from Q4b. Result: radar vs illustrative benchmark, 7 dimension bars with benchmark ticks, level gauge, flywheel.
- **Homepage repositioned** as category homepage: "Your business cannot scale while it lives in people's heads." Two-versions section, Mapped Score centre, products flywheel (Score it / Build it / Stay Mapped), AI-context, Built in Africa, Founding Organisations + benchmark consent line, Research Programme (000/001/002), Founding Benchmark signup.
- Naming sweep: Clarity Index / Clarity Score / Self-Check → **Mapped Score** across all live pages, including the sample-map badges.
- GA4: real measurement ID on all pages; new events `mapped_score_started`, `mapped_score_completed`, `book_assessment_click`, `publication_download`.
- Lead delivery unchanged: FormSubmit endpoint + n8n-first-with-fallback (endpoint blank until n8n live). All contact points → mappedafricameroeafrica@gmail.com.

## site-v1.x — 2026-06-29 → 2026-07-05 (main, pre-Phase 1)
- Initial MAPPED product site (Business Clarity Toolkit positioning, pricing tiers, Clarity Index self-check).
- Clarity Self-Check upgraded to 5-pillar Clarity Index with radar + fixes (2026-07-03).
- GA4 funnel instrumentation, SEO/structured data, MAPPED PRESS page + *The Invisible Organisation* paper (2026-07-05).
- Lead-pipeline reconciliation: n8n-first with FormSubmit fallback on both forms; bounce fixes (hello@ addresses → working inbox).
