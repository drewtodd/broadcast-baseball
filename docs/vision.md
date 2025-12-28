

# Vision — Broadcast Baseball

## What This Is

**Broadcast Baseball** is a radio-first, text-driven baseball simulation.

Its primary goal is not visual fidelity, UI density, or managerial depth.  
Its goal is **immersion through broadcast-style play-by-play and color commentary**.

If reading (or listening to) a single at-bat does not *feel alive*, the game has failed — regardless of how sophisticated the underlying simulation might be.

---

## The Core Promise

> **One at-bat feels alive.**

Everything in this project flows from that promise.

- Each pitch has rhythm.
- Counts matter.
- Silence is allowed.
- Commentary reacts to context, not just outcomes.
- Big moments feel different from routine ones.

A full nine-inning game is simply many believable at-bats, stitched together.

---

## Radio-First, Not UI-First

Broadcast Baseball is designed from the perspective of a radio listener:

- Minimal visual dependency
- Clear, speakable language
- Natural pacing
- Emphasis on voice, timing, and tone

The simulation should be enjoyable:
- **as plain text**
- **as spoken audio**
- **without requiring a graphical interface**

Any UI or visualization added later is secondary to the broadcast experience.

---

## Design Philosophy

### Simulation Serves the Broadcast

The simulation exists to create believable moments for commentary, not the other way around.

- Deterministic, explainable outcomes
- Structured events emitted by the simulation
- Commentary consumes events, it never controls them

Accuracy and internal consistency matter more than realism for its own sake.

---

### Constraints Are a Feature

Broadcast Baseball deliberately starts small.

Early scope is limited to:
- A single at-bat
- A small, expressive player model
- A clear pitch-by-pitch event flow

This constraint forces quality:
- If one at-bat works, innings work
- If innings work, games work
- If games work, seasons can come later

---

## What This Is *Not*

Broadcast Baseball is **not**, at least initially:

- A full franchise simulator
- A roster management game
- A financial or contract simulation
- A stat-maximization exercise
- A graphical sports game

Those features may come later, but they are explicitly out of scope for the MVP.

---

## Long-Term Direction (Non-Binding)

Possible future expansions include:
- Full games and seasons
- Multiple broadcast styles or eras
- Web-based playback
- Text-to-speech “radio mode”
- LLM-assisted color commentary
- Light franchise or historical replay modes

These ideas inform design decisions but do not drive current implementation.

---

## Success Criteria

At the MVP level, Broadcast Baseball is successful if:

- Reading a single at-bat is engaging
- Listening to a single at-bat feels natural
- Commentary is varied but controlled
- The system is deterministic and testable
- The design scales cleanly without rewrites

If those criteria are met, everything else is optional.

---

## Guiding Question

At every stage of development, ask:

> **Does this make the at-bat feel more alive?**

If the answer is no, it probably does not belong in the project — at least not yet.