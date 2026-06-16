# Kindness & Co — Onboarding sequence (early game), v0.2

> Companion to `kindness-and-co-design.md`. This **replaces v0.1**, which packed roughly ten
> systems into a single three-to-five-minute first session and overwhelmed playtesters. v0.2
> introduces systems **one at a time** across the early game (the Act I mail room and into Act
> II), on a ladder cadence: each system enters only when its absence has become a felt problem
> for the player. The Spirit-meter spec from v0.1 is preserved unchanged at the end.

## What changed from v0.1

- **Session one is now the core loop and nothing else.** No Dispatch Board, no second
  currency, no promotion, no allocation, no Circle.
- Everything v0.1 crammed into the first session is redistributed across **nine teaching
  moments**, each gated by a trigger.
- The appointment hook (passive accrual) was moved to where it actually makes sense, the
  community-spaces rung, because nothing accrues until the player owns a space. Session one no
  longer promises accrual it cannot deliver.

## Principles

1. **Teach by need, not by tour.** A system is introduced at the exact moment its absence
   becomes a felt problem, and not one beat before.
2. **One verb at a time, uncontested.** Never introduce two new systems in the same beat.
   Each teaching moment gets a clean stage.
3. **Gate attention, not just unlocks.** A system can exist in the simulation (and record
   state) long before it is allowed to occupy screen space.
4. **Pacing is uneven on purpose.** Wait for the trigger even if that means several sessions
   between rungs. An empty rung beats a premature one.

## Self-check diagnostic

For every element on the screen, ask: what problem does this solve for the player, and have
they felt that problem yet? If they have not felt the problem, the element is premature and
should be invisible until they do.

---

## The introduction sequence (the ladder)

Rung 1 is session one and is specified beat by beat. Rungs 2 through 9 use a compact template
(Trigger / Teaches / Conceals / State). Spirit is deliberately off the ladder (see the
lifecycle spec below).

### Rung 1 — Core loop (session one, in full)

The first session teaches exactly one verb: spend Warmth, do an act, watch the number climb.

- **Beat 1, Arrive.** The mail room. Warm, brief, gently corporate-cheery. The founder's
  words are framed on the wall, played straight (their irony is only legible on a replay). No
  mechanics yet.
- **Beat 2, The first act.** A friendly colleague hands the player one simple task with a
  single highlighted button. One click. Warmth ticks down a little, Reach ticks up, a
  satisfying chime. **Spirit begins recording silently here** (see lifecycle spec); the player
  sees no meter.
- **Beat 3, A few more.** A short burst of rote acts. On a streak, a light celebration
  ("five in a row, you're a natural"). **Sincerity decay is dormant**, so volume feels pure
  and rewarding.
- **Beat 4, A warm stop.** A gentle "good first day." **No accrual promise** (nothing
  accrues yet), no board, no allocation. The player ends topped up and proud.

**Concealed in session one:** Glow (earned and banked, not shown), the Dispatch Board,
promotions, stat allocation, the Circle, and Spirit.

**State after session one:** Warmth drawn down and regenerating. Reach shown. Glow recorded
but hidden. Spirit recorded but hidden, and firmly in the top band (see reveal-proof math).

#### Rung 1 coda — the Dispatch Board

Once the loop is muscle memory (a strong session one, or the open of session two), introduce
the Dispatch Board and quota culture. This is the company's religion: Reach is the sacred,
public, ranked number. It is framing, not a new verb, so it rides alongside the loop, but only
after the verb is solid. Let the player do the thing first and understand the company second.

### Rung 2 — Glow and the first supply
- **Trigger:** the player has a meaningful Glow balance (silently banked since session one)
  **and** a first supply exists to spend it on.
- **Teaches:** Glow is a currency with a decision attached. Reveal the banked balance ("you
  have been earning this") together with a store holding one item that visibly improves acts.
- **Conceals:** the wider economy (community spaces, cosmetics). Just one supply for now.
- **State:** Glow now visible. First sink available.

### Rung 3 — Promotion as reset
- **Trigger:** the first level-up threshold.
- **Teaches:** progression doubles as a resource reset, and climbing is the goal. Pure
  reward: refill Warmth to full, celebrate, the player's name climbs the Board. **No stat
  allocation yet.**
- **Conceals:** the build/allocation layer, and the hidden Spirit restore that rides along.
- **State:** Warmth full. Spirit restored (hidden). Rank up.

### Rung 4 — Genuine acts
- **Trigger:** rote acts start feeling samey, or a recipient's situation visibly needs more
  than a rote act.
- **Teaches:** not all acts are equal; depth exists. This is the first quiet seed of
  depth-over-volume, **not yet the lesson** (the depth and volume payoff lines still overlap
  here, per Act II in the main doc).
- **Conceals:** brave acts, the Courage gate, and the full teeth of sincerity decay (still
  gentle).
- **State:** a second act type is available.

### Rung 5 — Stat allocation and build
- **Trigger:** the second promotion, once the player has a forming playstyle.
- **Teaches:** ownership and a build. Now introduce stat points (Warmth capacity vs
  Efficiency).
- **Conceals:** any Spirit-touching stat (there are still none; a Spirit stat would betray
  its existence).
- **State:** allocation available.

### Rung 6 — Ripples
- **Trigger:** the player has organically collected a couple of Ripple stories, which arrive
  as surprises from acts.
- **Teaches:** the collection meta, permanent bonuses, and shareable narrative. Reveal the
  set frame only once a few pieces exist, so it lands on real pieces rather than an empty grid.
- **Conceals:** nothing major. Keep completion deterministic-with-effort, not gacha (main doc
  Section 9).
- **State:** Ripple collection UI revealed. First set in progress.

### Rung 7 — The Kindness Circle
- **Trigger:** the solo loop is steady (the player returns reliably and is comfortable with
  acts, economy, and progression).
- **Teaches:** mutual care, cooperative acts, and social reach. Introduce **receive** first
  as a pure delight (someone sends you a kindness), then reveal that you can send and
  cooperate.
- **Conceals:** that receiving is a fatigue-recovery tool (fatigue is still invisible). The
  receive silently tops up Spirit.
- **State:** Circle active. Receive, send, and a first cooperative act.

### Rung 8 — Community spaces (passive income and the appointment hook)
- **Trigger:** surplus Glow beyond supplies **and** a rank gate.
- **Teaches:** long-horizon investment, tending, and lasting good. Introduce the first
  community space (a capital sink that accrues passive Glow while the player is away). **This
  is where the appointment mechanic lands**, because now there is finally something to return
  to.
- **Conceals:** nothing major.
- **State:** first space owned. Passive accrual and the return-to-tend loop are live.

### Rung 9 — The wall and its exits
- **Trigger:** the first time Warmth actually runs low. Given how generous Warmth is, this
  may not happen until content density rises, which is correct: teach the exit at the moment
  of the wall, never before.
- **Teaches:** what to do when low, and that the wall is humane. Introduce the three exits in
  context: rest, receive, reflect.
- **Conceals:** still no Spirit and no pay-anything.
- **State:** exits introduced contextually.

---

## Off the ladder — the Spirit-meter lifecycle (the hinge spec)

Spirit is the one system you deliberately do not teach. Its whole power is that the player
discovers it has been there all along. Keep it hidden; do not add a tutorial for it.

### Phase 1 — Silent tracking (from session one, Beat 2)
Spirit is a real variable, initialized at 100, decremented by every act from the very first
one (rote -2, genuine -4, brave -8, per main doc Section 4.2). It is recorded every act and
rendered to the player **nowhere** in the early game: no meter, no number, no icon, no stat,
no tooltip. The full history is retained because the Act III reveal surfaces it retroactively.

### Phase 2 — Why the early game is reveal-proof
The reveal trigger (below) is Spirit dropping below 50. Early content must make that
impossible through tuning, not a clamp, so the simulation stays honest.

The math, with Act I values (Warmth max 20; a rote act costs 2 Warmth and 2 Spirit):

- One full Warmth bar = 10 rote acts = **-20 Spirit**. Starting at 100, a complete dump lands
  at **80**, still in the top band (x1.2).
- To reach below 50 a player would need roughly 25-plus consecutive acts with no top-up,
  which exceeds the Warmth and content available in early sessions.

So the **Warmth budget alone guarantees reveal-proofing**. The Spirit restores from
promotions (Rung 3) and received kindness (Rung 7) are bonuses on top of that guarantee, not
load-bearing for it. Use a soft floor (do not let Acts I and II Spirit fall below ~60) only as
a backstop, never as the primary mechanism.

### Phase 3 — The reveal trigger (Act III)
- **Condition:** the first time Spirit crosses **below 50** (out of the x1.0 band into the
  x0.6 "landing flat" band).
- **Why it cannot fire earlier:** early content caps Warmth budgets and supplies regular
  top-ups, so sustained depletion below 50 is not achievable (Phase 2).
- **Why it fires in Act III:** the crisis content provides long, top-up-free sessions with
  abundant available acts, and genuine and brave acts cost more Spirit (-4, -8). A player
  grinding volume through a crisis session naturally crosses below 50 for the first time.

### Phase 4 — The reveal behavior (the back-fill)
When Spirit first crosses below 50:
1. The meter animates into existence for the first time.
2. It **back-fills**, showing the player the history it has been recording (the curve of their
   Spirit over this session, and optionally across the campaign), making visible that their
   recent acts have been paying at x0.6, not x1.2.
3. The gut-punch is retroactive: "this was happening the whole time, and I could not see it."
   This is why Phase 1 records from session one. A meter that began tracking only at the moment
   of reveal would feel cheap and the player would sense it.

No character explains the meter. The reveal is mechanical and felt (main doc Section 2,
principle 4). Any dialogue reacts to the discovery, never pre-empts it.

### Phase 5 — Edge cases
- **The determined early grinder:** covered by Phase 2 (cannot reach below 50) plus the soft
  floor backstop.
- **Reaching below 50 in Act II:** decide deliberately. Recommended: extend the same budget
  discipline through Act II to hold the reveal for the Act III crisis, which gives the
  strongest landing.
- **Spirit at 0:** out of scope for this slice but flagged in main doc Section 17. Define what
  the x0.3 band and full depletion offer the player before Act III ships.

---

## The two seeded threads

Keep these mechanically separate so the Act III payoff stays clean.

- **Thread A, the world decouple (visible seed).** Reach can rise while real kindness-energy
  does not. Plant **one** quiet instance: an ordinary-looking act whose recipient response is
  flat, or which pays visibly less kindness-energy than its neighbors while paying the same
  Reach. Plant it **no earlier than a few sessions in** (around Rung 4, once the player has a
  baseline sense of a normal act, so the off-one can register as subtly wrong). Most players
  will not consciously notice. This thread feeds the Act III crisis.
- **Thread B, the cost of giving (invisible).** Spirit. Tracked from the first act, shown
  never in the early game, with no seed and no foreshadow. Total invisibility is the point.

Do not let Thread A's whisper read as a Spirit event. The recipient who is not reached (Thread
A) is about the world, not about the player being depleted (Thread B).

---

## UI notes

- **Reach is loud, kindness-energy is quiet** from session one. Reach gets the big
  celebratory treatment; kindness-energy is present but visually secondary. This asymmetry is
  the seed of the whole Goodhart arc and must be deliberate.
- **Glow is hidden until Rung 2.** It is earned and banked from session one but not shown.
- **No Spirit affordance anywhere on the ladder.** Verify no meter, badge, stat, tooltip, or
  settings entry references Spirit in early builds.
- **One introduction at a time.** Never reveal two new systems in the same beat.
- **Streaks celebrated, decay silent** through the early rungs.

---

## Acceptance criteria

- A new player completes their first act within seconds, with no written instruction beyond
  the single highlighted button, and **session one contains only the loop** (verify no Board,
  Glow, allocation, or Circle is visible in session one).
- Asked what the game is about after session one, a playtester mentions spreading kindness and
  perhaps climbing, and does **not** mention Glow, spaces, the Circle, or Spirit.
- Each later system, when introduced, arrives at a moment the player can articulate a need for
  ("I had Glow and nowhere to spend it, then the store appeared").
- **No session ever introduces two new systems at once.**
- In instrumentation, Spirit was recorded every act, never shown, and never fell below the top
  band for any player in Acts I and II.
- The Thread A whisper went consciously unnoticed by the large majority of playtesters.

---

## Open questions specific to this slice

- The exact Glow threshold and the first supply item that trigger Rung 2.
- Which rung the Thread A whisper plants on, and its precise form (flat response vs reduced
  payout). Pick one and test which is recoverable-but-not-salient.
- Whether the Dispatch Board coda belongs at the end of session one or the open of session
  two (playtest both).
- The rank-gate value for the first community space.
- Real act content per department (still open from the main doc).
