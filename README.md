# Kindness & Co — Playable Prototype

A first playable slice of **Kindness & Co**, the game about rising through a company
whose business is spreading kindness. This prototype exists to let you *feel how it
plays* — the warm volume grind of Act I, the silently-accruing cost underneath it, and
the moment the whole thing turns.

It is a single self-contained file. **No install, no build, no server.**

## How to run it

Open `index.html` in any modern browser (double-click it, or drag it into a browser tab).
That's it.

## What's in this slice

This implements the **suggested first vertical slice** from the design doc (Section 16)
*plus* the **Act I onboarding beat sheet** and the **Spirit-meter reveal hinge** — the
moment the whole campaign swings on.

1. **The core loop** — spend Warmth → do an act → earn Reach + kindness-energy + Glow.
2. **Warmth** as a regenerating, humane gate (regen is accelerated ~50× here so you don't
   have to wait 85 real minutes to test it).
3. **The three act types** — rote / genuine / brave — with the payouts from Section 6.
4. **The Spirit multiplier** (×1.2 / ×1.0 / ×0.6 / ×0.3 bands), **hidden during Act I** and
   **revealed at the crisis**, exactly as the hinge spec requires. Spirit is recorded from
   your very first act so the reveal can back-fill a *real* history, not a fake one.
5. **Sincerity decay** on repeated identical rote acts (−15% each, floor 30%) — dormant in
   Act I, live once the floor opens.
6. **A live readout** of your kindness-energy vs Reach over the session, so the
   depth-versus-volume divergence is *felt, not explained*.
7. **The three exits** — Rest / Receive / Reflect — replacing wait / recruit / pay.
8. **The Goodhart framing** — the Dispatch Board renders Reach loud and celebratory while
   kindness-energy stays small and secondary.

## How to play (≈ 5–8 minutes)

1. **Act I — The Mail Room.** Pem, the quota evangelist, walks you through the beat sheet:
   the Dispatch Board, your first stamped note, a streak, a promotion (refills Warmth, and
   *silently* tops up the hidden Spirit), a stat point, a kindness received, and one
   ordinary delivery that's subtly *off* (the Beat 8 "whisper" — Reach goes up, the good
   doesn't). You should leave this stretch feeling good and a little in love with the grind.
2. **The floor opens.** Genuine acts unlock and the rails come off. **Now: just keep the
   board climbing.** Grind rote acts. Watch Reach soar.
3. **The turn.** Keep grinding and your hidden Spirit slides. The first time it crosses
   below 50, the **Spirit meter animates into existence and back-fills its whole history** —
   showing you that your recent acts have been landing flat the entire time, and the
   dashboard never said a word.
4. **The relearning.** A brave act unlocks — a real case (Maro in Accounts) that volume
   can't touch. One brave act out-earns a long stretch of your rote dispatches. The thesis,
   in your own numbers. From here, manage Spirit with Rest / Receive / Reflect, mix in depth,
   and watch the green line pull away from the orange one.

> **To reach the reveal, you have to push volume.** A careful depth-first player can keep
> their Spirit high and never trigger it — which is thematically correct, but means a
> playtester being "good" might miss the hinge. For testing, grind rote acts after the floor
> opens. (In the full game, Act III's long top-up-free crisis sessions force this naturally.)

Your open-play progress is saved in the browser. **Reset & replay** (bottom of the page)
clears it and starts the first day over.

## What is *not* in this slice (deliberately)

Per the build guidance, these are later layers: the Glow sinks (community spaces,
cosmetics), Ripples and collections, the Kindness Circle as real multiplayer, Courage as a
full economy, and the complete five-act narrative (Acts IV–V and the Coda). The Circle and
crisis here are compressed into a single solo session so the *hinge* is testable end-to-end.

## A note on the numbers

Every constant comes straight from the design docs and is illustrative by design — a
starting point for a tuning spreadsheet, not a final value. The relationships between the
numbers are the design; the exact values are a balancing job. Warmth regen is sped up for
testing and flagged as such in-game.

## Files

- `index.html` — the entire game (HTML + CSS + JS, no dependencies).
- `kindnessandcodesign.md` — the source design doc (your upload, for reference).
- `kindnessandcoact1onboarding.md` — the Act I beat sheet (your upload, for reference).
