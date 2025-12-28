# Roadmap — Broadcast Baseball

This roadmap defines **what gets built, and in what order**, for Broadcast Baseball.

It is intentionally conservative.
Progress is measured by *feel*, not feature count.

---

## Guiding Principle

> **One at-bat feels alive.**

Every milestone exists to serve that goal.
Anything that does not directly support it is deferred.

---

## Phase 0 — Foundation (Complete)

**Goal:** Establish intent, constraints, and shared language.

Deliverables:
- Clear project vision
- Radio-first design principles
- Enforceable commentary style rules
- Clean separation of Dx (design) and Dv (development)
- Repository structure and tooling baseline

This phase ensures future work does not drift.

---

## Phase 1 — One At-Bat (MVP)

**Goal:** Make a single plate appearance feel believable and engaging.

### Scope
- One batter vs. one pitcher
- Pitch-by-pitch progression
- Count tracking
- Deterministic outcomes (seeded RNG)
- Text-based output only

### Required Capabilities
- Minimal player model (batter + pitcher)
- Pitch events that modify the count
- Terminal outcomes:
  - Strikeout
  - Walk
  - Ball in play (out or hit)
- Structured event emission
- Play-by-play commentary
- Optional color commentary (rules-based)

### Success Criteria
- Reading one at-bat is engaging
- Commentary follows style rules
- Count progression feels natural
- Silence and pacing feel intentional
- Results are reproducible

If this phase succeeds, the project is viable.

---

## Phase 2 — Inning Context (Deferred)

**Goal:** Provide situational context without overwhelming the broadcast.

### Additions
- Base state (empty / runners on)
- Outs tracking
- Simple run scoring
- Box score accumulation

### Constraints
- Commentary must remain pitch-centric
- No managerial decisions
- No substitutions

This phase exists only after Phase 1 feels right.

---

## Phase 3 — Full Game Loop (Deferred)

**Goal:** Stitch believable at-bats into a coherent game.

### Additions
- Nine-inning structure
- Lineup order
- Pitcher fatigue (lightweight)
- End-of-game summary

### Constraints
- No bullpen management
- No strategy trees
- Broadcast experience remains primary

---

## Phase 4 — Audio Playback (Optional)

**Goal:** Allow the game to be experienced entirely by ear.

### Additions
- Text-to-speech integration
- Voice presets (play-by-play vs. color)
- Playback controls (pause, speed)

### Constraints
- Text output remains authoritative
- Audio is a rendering layer, not a logic layer

---

## Phase 5 — Advanced Commentary (Optional)

**Goal:** Increase variety and realism without losing control.

### Additions
- Expanded rules-based color commentary
- Optional LLM-assisted color (strictly constrained)
- Narrative thread tracking (hot/cold, long at-bats)

### Constraints
- Play-by-play remains deterministic
- LLMs may never control outcomes
- Guardrails remain enforced

---

## Explicitly Out of Scope (For Now)

The following are intentionally excluded from near-term work:

- Franchise mode
- Trades, contracts, finances
- Player development systems
- Graphics-heavy UI
- Multiplayer or competitive modes

These may be revisited only after the broadcast experience is proven.

---

## Roadmap Discipline

- Phases must be completed in order
- Each phase must *feel right* before advancing
- Skipping ahead creates debt
- Refinement is progress

---

## Final Check

Before starting any new work, ask:

> **Does this help one at-bat feel more alive?**

If the answer is no, it does not belong on the roadmap.
