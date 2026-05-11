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

Start the demo flow from [Screen 2](screen-2-ranked.html).

## Demo path

1. Open Screen 2
2. Promote Candidate 12 → structured override modal opens (Screen 3)
3. Submit → return to Screen 2, watch Candidate 12 move into Tier A with an audit-tagged badge
4. Repeat with a second candidate to see the pattern detector advance toward the criteria-refinement nudge

Hit `↻ Reset demo` in the top right of Screen 2 to clear demo state between runs.

## Stack

Plain HTML / CSS / JS. No build step. No backend. State persists between screens via `localStorage`.
