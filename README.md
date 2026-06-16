# Kindness & Co — Playable Prototype

A playable slice of **Kindness & Co**, the game about rising through a company whose
business is spreading kindness. It exists to let you *feel how it plays*.

Single self-contained file. **No install, no build, no server.**

## How to run it

Open `index.html` in any modern browser (double-click it, or drag it into a tab).

Or play the hosted build (once Pages is enabled): **https://eeeviloliveee.github.io/kindnessandco/**

## What this version implements — the v0.2 onboarding ladder

This build follows **`kindnessandcoact1onboarding.md` (v0.2)**: instead of front-loading
every system, it introduces them **one at a time**, each gated by a trigger that only fires
once its absence would be felt. The whole point is that the opening can't overwhelm you.

**Session one is the core loop and nothing else** — spend Warmth, do an act, watch Reach
climb. No Board, no Glow, no promotion, no allocation, no Circle, no Spirit. You end topped
up and proud.

Then the nine rungs ladder in, in order, as you play:

1. **Core loop** (session one, scripted by Pem).
2. **Dispatch Board** — opens at the start of day 2 (Reach is loud; the company religion).
3. **Glow** — revealed once you've quietly banked enough, together with a one-item supply store.
4. **Promotion as reset** — at the first Reach threshold: refill Warmth, climb the board. (No allocation yet.)
5. **Genuine acts** — once rote starts feeling samey; also reveals the depth-vs-volume chart. *(The Thread A "whisper" — Reach up, kindness flat — is planted here.)*
6. **Stat allocation** — at the second promotion, when you have a playstyle.
7. **Ripples** — once a couple of story-pieces have organically dropped from your acts.
8. **The Kindness Circle** — once you're returning reliably (day 3+): receive first, then send and co-host.
9. **Community spaces** — surplus Glow + rank: the first space that accrues Glow *while you're away* (the appointment hook).
10. **The wall & its exits** — the first time Warmth actually runs low: Rest / Receive / Reflect.

And off the ladder, the hinge: **Spirit** is recorded silently from your very first act,
shown nowhere, kept reveal-proof in Acts I/II, and revealed only when it crosses below 50 in
the Act III crisis — where the meter animates in and **back-fills its real history**.

## Sessions

There's an **End the day** button. Warmth refills overnight, and any community spaces accrue
Glow while you're away — so the appointment hook is real, not faked. Some rungs gate on the
day count (the Board at day 2, the Circle at day 3+).

## The DEV panel (bottom-left) — for testing

Because the ladder is deliberately paced across days, a tester shouldn't have to grind to
reach later rungs. The **🛠 DEV** panel lets you:

- **Jump to any rung** (unlocks everything up to it, with sane prerequisites).
- Add Warmth / Glow / Reach / a Ripple.
- **Advance one day.**
- **Begin the Act III crisis** (makes the Spirit reveal reachable by grinding) or **force the reveal now**.
- Reset and replay from Day 1.

## Suggested test paths

- **The intended experience:** play session one, end the day, and let the rungs arrive on
  their own. Notice whether each new system shows up at a moment you can articulate a need for.
- **Straight to the hinge:** DEV → *Begin Act III crisis*, then grind rote acts until Spirit
  crosses below 50 and the meter back-fills. Then do the brave act it unlocks (Maro) and watch
  one act out-earn a long rote streak.
- **Feel the anti-grind:** spam the *same* rote act after Rung 4 and watch sincerity decay
  starve your payouts (this is why a pure grinder's Glow stalls).

## Design choices I made where the doc left it open

- **Board coda** opens at the start of session two (the doc flags day-1-end vs day-2-open as a
  playtest question; this is easy to flip).
- **Thread A whisper** plants at Rung 4, per the doc's recommendation.
- Glow / Reach / rank thresholds are tuned so triggers fire within a natural play session.

## Numbers

Every constant comes from the design docs and is illustrative — a starting point for tuning,
not final values. Warmth regen is sped up ~50× so you don't wait 85 real minutes.

## Files

- `index.html` — the entire game (HTML + CSS + JS, no dependencies).
- `kindnessandcodesign.md` — the main design doc.
- `kindnessandcoact1onboarding.md` — the v0.2 onboarding ladder this build follows.
