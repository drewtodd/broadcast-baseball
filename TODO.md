# TODO — Broadcast Baseball

This file tracks **day-to-day implementation work**.
It is tactical, temporary, and expected to change frequently.

For long-term direction and scope, see `docs/roadmap.md`.

---

## Current Focus: Phase 1 — One At-Bat

### Design checks (Dx)
- [ ] Validate one–at-bat data model against commentary rules
- [ ] Confirm event naming is broadcast-friendly
- [ ] Identify “moment detection” signals (count leverage, long ABs)

### Implementation tasks (Dv)
- [ ] Define Player model (batter, pitcher)
- [ ] Define PitchEvent and PAResult event schema
- [ ] Implement count progression logic
- [ ] Implement seeded RNG handling
- [ ] Emit structured events per pitch
- [ ] Generate play-by-play lines from events
- [ ] Add basic rules-based color commentary
- [ ] Write first deterministic test for one at-bat

---

## Parking Lot (Not Now)
- [ ] LLM-assisted color exploration
- [ ] TTS experiments
- [ ] Web API scaffolding
- [ ] Multi-AB state accumulation

---

## Done (Archive as needed)
- [x] Project vision and guardrails
- [x] Radio-first design principles
- [x] Commentary style guide