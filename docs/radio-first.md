# Radio-First Design — Broadcast Baseball

## What “Radio-First” Means

Broadcast Baseball is designed as if it were being experienced primarily through audio.

Text is treated as *spoken language first*, written language second.  
If a line does not sound natural when read aloud, it does not belong in the game.

This mindset drives every design decision that follows.

---

## The Listener’s Perspective

The primary user of Broadcast Baseball is not a viewer.  
It is a **listener**.

That listener:
- May not be looking at the screen
- May only glance occasionally at a box score
- Relies on pacing, emphasis, and clarity to follow the game

The broadcast must therefore:
- Establish context quickly
- Reinforce important information naturally
- Avoid visual-only cues or assumptions

---

## Pacing and Silence

Baseball on the radio is defined as much by what is *not* said as by what is.

### Silence Is a Feature
- Not every pitch needs commentary
- Not every moment needs color
- Short gaps create rhythm and anticipation

Silence should be intentional, not accidental.

---

## Speakable Language

All output must be:
- Easy to pronounce
- Free of dense visual references
- Understandable without seeing the field

Avoid:
- Long compound sentences
- Overloaded stat lines
- Visual shorthand (“that one clips the black” without context)

Prefer:
- Short sentences
- Clear verbs
- Familiar baseball phrasing

---

## Count-Centered Storytelling

The count is the backbone of radio baseball.

Listeners track tension through:
- 0–2 vs. 3–1
- Full counts
- Pitch sequences that tell a story

Broadcast Baseball should:
- Reference the count when it matters
- Let the count *shape* commentary tone
- Treat long at-bats as mini-narratives

---

## Big Moments Sound Different

Routine pitches and pivotal moments must feel distinct.

This distinction can be achieved through:
- Line length
- Word choice
- Pause length
- Frequency of commentary

A strike in a 1–0 count is not the same as a strike in a 3–2 count.

---

## Commentary Roles

The broadcast voice is conceptually split into two roles:

### Play-by-Play
- Factual
- Concise
- Deterministic
- Never speculative

### Color
- Contextual
- Optional
- Reactive, not controlling
- Adds texture without obscuring facts

Both roles must respect pacing and silence.

---

## Text as Audio Blueprint

Text output is treated as an **audio script**, not prose.

This implies:
- Consistent sentence structure
- Intentional pauses
- Lines that can be read verbatim by text-to-speech systems

Markers or conventions for pauses may be used internally, but clarity always comes first.

---

## Design Implications

A radio-first approach implies:

- The simulation emits structured events
- Commentary is layered on top
- Audio playback is a first-class future feature
- UI and visuals are always secondary

If a feature improves visuals but harms the broadcast experience, it is a net negative.

---

## Guiding Principle

At every design decision, ask:

> **Would this still work if I closed my eyes?**

If the answer is no, it is not truly radio-first.
