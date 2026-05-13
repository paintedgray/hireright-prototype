# HireRight Prototype

An AI-augmented hiring workflow prototype built around three principles:

1. **Bias control upstream** — checks happen at criteria definition, not after a shortlist is produced
2. **Honest confidence bands** — the model commits to a top-10 but surfaces where it can't reliably separate candidates
3. **Override reasoning as first-class data** — when a recruiter overrides the model, the *why* is captured structurally, not as free text

## Screens

| # | Screen | Purpose |
|---|---|---|
| 1 | [Criteria Builder + Proxy Stress Test](screen-1-criteria.html) | Define must-haves and signal weights. Three-tier action system catches problematic criteria upstream. |
| 2 | [Ranked Candidate View](screen-2-ranked.html) | Tier-grouped list with confidence bands. All 150 candidates remain visible. |
| 3 | [Structured Override Capture](screen-3-override.html) | Hero screen — captures override reasoning as structured data. |
| 4 | [Per-Candidate Context Drawer](screen-4-context.html) | Evidence-based context: snapshot, must-have checklist, resume excerpt with highlighted bullets. |
| 5 | [Decision Log](screen-5-audit.html) | Audit-grade trail of every override, criteria change, and flag acknowledgment. CSV export. |

Start the demo flow from [Screen 2](screen-2-ranked.html).

## Demo path (~2 min)

1. Open Screen 2
2. Scroll past the shortlist commit line and click Candidate 12 at rank #15 → context drawer (Screen 4)
3. Click "↑ Promote to top 10" → structured override modal (Screen 3)
4. Submit → return to Screen 2, watch Candidate 12 land in Tier A with an audit-tagged badge
5. Click "📋 Decision log" in the Screen 2 header → see the override appended to the audit trail
6. Repeat to see the override pattern detector advance toward the criteria-refinement nudge

Hit `↻ Reset demo` in Screen 2's header to clear demo state between runs.

## Stack

Plain HTML / CSS / JS. No build step. No backend. State persists between screens via `localStorage`.
