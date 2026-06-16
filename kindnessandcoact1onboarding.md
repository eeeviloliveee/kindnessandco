# Kindness & Co — Act I Onboarding Beat Sheet and the Spirit-Meter Hinge (v0.1)

> Companion to `kindness-and-co-design.md`. This document specifies the first player session
> (Act I, the mail room) beat by beat, and nails down the full lifecycle of the Spirit meter
> from silent tracking to its Act III reveal. The reveal is the moment the whole campaign
> swings on, and you cannot build Act I correctly without knowing exactly what it is secretly
> recording and what later surfaces it. Section references below point to the main design doc.

## How to read this

Each beat uses the same template:

- **Sees** — what is on screen.
- **Does** — the player action.
- **Teaches** — the intended lesson (mechanical or cultural).
- **Conceals** — what the beat deliberately hides or under-emphasizes.
- **Feels** — the emotional target.
- **State** — the systems state after the beat.

All numbers are illustrative (see the provenance note in the main doc).

---

## What Act I onboarding must accomplish

1. Teach the core loop in one frictionless action: spend Warmth, do an act, watch the number
   climb (main doc Section 3).
2. Make volume feel genuinely good. The player should leave their first session a little in
   love with the grind. This is the "before" the campaign later transforms (Section 11, Act I
   and II).
3. Install the company religion: **Reach** is the sacred metric, the Dispatch Board is the
   altar, climbing is the point.
4. Plant exactly one visible seed of the world-level decouple (Reach and kindness-energy can
   come apart), as a whisper the player will not consciously register.
5. Begin silently recording **Spirit** from the very first act, while showing the player no
   trace of it, and guarantee the player cannot deplete it far enough to trigger its reveal.

Point 5 is the hinge. The rest of this document exists to make it precise.

---

## The two hidden threads

Keep these mechanically separate so the Act III payoff stays clean.

- **Thread A, the world decouple (visible seed).** Reach can rise while real
  kindness-energy does not. Act I plants one quiet instance of this (Beat 8). This thread
  feeds the Goodhart crisis (Section 11, Act III).
- **Thread B, the cost of giving (invisible).** Spirit. Tracked from act one, shown to the
  player **never** in Act I, with no seed and no foreshadow. Total invisibility is the point:
  the Act III reveal lands harder the more completely the player was unaware it existed.

Do not let Thread A's whisper read as a Spirit event. The recipient who is not reached
(Thread A) is about the *world*, not about the player being depleted (Thread B).

---

## The beat sheet (first session, target 3 to 5 minutes)

### Beat 0 — Arrival
- **Sees:** The mail room of Kindness & Co. Warm, busy, gently corporate-cheery. The
  founder's words are framed on the wall, already a little hollowed by overuse.
- **Does:** Walks in. No mechanics yet.
- **Teaches:** Tone and place. This is a company, and kindness is its business.
- **Conceals:** That the founder's principle has drifted (Section 11). The quote is played
  straight here; its irony is only legible on a replay.
- **Feels:** Belonging, mild awe at the scale of the operation.
- **State:** No resources spent.

### Beat 1 — The Dispatch Board
- **Sees:** A large glowing board showing everyone's **Reach** totals, names ranked by
  volume dispatched.
- **Does:** Watches a colleague's number tick up and the board celebrate it.
- **Teaches:** Reach is the number that matters here. Public, ranked, sacred.
- **Conceals:** That kindness-energy, not Reach, is what actually powers the world. The board
  does not display kindness-energy at all.
- **Feels:** Aspiration. "I want my name to climb that board."
- **State:** No resources spent.

### Beat 2 — The first act
- **Sees:** A friendly, well-meaning quota evangelist hands the player one simple task: stamp
  a kind note and send it out. A single highlighted button.
- **Does:** One click.
- **Teaches:** The atomic loop. Spend a little Warmth, perform an act.
- **Conceals:** Nothing yet, but this is the beat where **Spirit begins recording silently**
  (see lifecycle spec below). The act costs Spirit in hidden state; the player sees no meter.
- **Feels:** Easy competence. A satisfying chime.
- **State:** Warmth -2. Reach +1. kindness-energy +5 (recorded). Glow +3. Spirit
  100 -> 98 (hidden).

### Beat 3 — The first payout
- **Sees:** A celebratory Reach increment (big, loud), and quieter readouts for Glow and
  kindness-energy.
- **Does:** Reads the result.
- **Teaches:** The currencies exist. Glow is yours to spend; the act did some good.
- **Conceals:** The deliberate UI hierarchy. **Reach is rendered large and celebratory;
  kindness-energy is small and secondary.** This is an intentional framing lie that sets up
  Goodhart. Do not give kindness-energy equal billing in Act I.
- **Feels:** Reward. The board noticed me.
- **State:** As Beat 2, surfaced to the player except Spirit.

### Beat 4 — The streak
- **Sees:** A few more rote acts available in a row. On the third, a celebration: "Five in a
  row, you're a natural."
- **Does:** Performs a short burst of rote acts.
- **Teaches:** Volume is good and gets celebrated. Streaks feel great.
- **Conceals:** **Sincerity decay is dormant in Act I** (effectively zero, see Section 6).
  The player must learn that grinding is pure upside, because the later discovery that it is
  not is the whole point. Do not let decay bite here.
- **Feels:** Flow, momentum, mastery.
- **State:** Warmth drawn down further; Reach climbing; Spirit drifting down in hidden state
  but still firmly in the top band (math below).

### Beat 5 — The first promotion
- **Sees:** A promotion ceremony. Mail Room Clerk to the next rung. Confetti, a badge, the
  player's name moves up the Dispatch Board.
- **Does:** Accepts the promotion.
- **Teaches:** Progression doubles as a resource reset. The promotion **refills Warmth to
  full and restores Spirit** (hidden), and climbing is framed as the goal.
- **Conceals:** That the Spirit restore even happened. The player experiences a Warmth refill
  and a rank-up; the Spirit top-up rides along invisibly and helps guarantee Act I stays
  reveal-proof.
- **Feels:** Pride, ascent, "this is working."
- **State:** Warmth full. Spirit restored toward 100 (hidden). +1 stat point.

### Beat 6 — Stat allocation
- **Sees:** A light allocation screen: Warmth capacity vs Efficiency.
- **Does:** Spends one point.
- **Teaches:** A faint sense of a build and ownership.
- **Conceals:** Any hint of Spirit. **Offer no Spirit-related stat in Act I.** A stat that
  touched Spirit would betray its existence.
- **Feels:** Agency.
- **State:** Stat applied.

### Beat 7 — A kindness received
- **Sees:** A small unprompted kindness arrives from a peer (NPC or another player), with a
  warm little animation.
- **Does:** Receives it. No action required.
- **Teaches:** Seeds the Circle and the receive mechanic. It simply feels nice.
- **Conceals:** That receiving just topped up the player's hidden Spirit. In Act I, receiving
  is framed purely as a pleasant social moment, not as a fatigue-recovery tool, because
  fatigue is not yet visible.
- **Feels:** Warmth, connection, being thought of.
- **State:** Spirit nudged up (hidden). Circle seeded.

### Beat 8 — The whisper (Thread A seed)
- **Sees:** One ordinary-looking delivery whose result is subtly off. Either the recipient's
  response is flat or absent, or the act pays visibly less kindness-energy than its identical
  neighbors while still paying the same Reach.
- **Does:** Performs the act like any other.
- **Teaches:** Nothing explicitly. This is a seed, not a lesson.
- **Conceals:** Its own importance. Most players will not consciously notice. It plants
  Thread A: Reach and kindness-energy can come apart. Act II's hairline crack and Act III's
  crisis harvest this.
- **Feels:** A barely-there flicker of "huh," gone in a second.
- **State:** Reach +1, kindness-energy below the usual for that act (recorded). Keep this a
  one-off; do not let it read as Spirit depletion.

### Beat 9 — Soft close
- **Sees:** A gentle "great first day" wrap, the player's Reach total shown proudly, and a
  note that their mail and spaces will accrue while they are away.
- **Does:** Ends the session.
- **Teaches:** The appointment hook (come back, things accrue). Section 7's passive trickle,
  framed kindly.
- **Conceals:** Nothing new. Critically, the player ends **topped up and proud, never
  depleted.** Spirit is in the top band. The reveal is held in reserve.
- **Feels:** Satisfaction, anticipation, "I did well, I'll be back."
- **State:** Session end. Spirit high (hidden). Appointment timer running.

---

## The Spirit-meter lifecycle (the hinge spec)

### Phase 1 — Silent tracking (from Beat 2)
Spirit is a real variable, initialized at 100, decremented by every act from the very first
one (rote -2, genuine -4, brave -8 per Section 4.2). It is recorded in player state every
beat. It is rendered to the player **nowhere** in Act I: no meter, no number, no icon, no
stat, no tooltip. The complete history is retained because the Act III reveal will surface
it retroactively.

### Phase 2 — Why Act I is arithmetically reveal-proof
The reveal trigger (below) is Spirit dropping below 50. Act I must make that impossible
through content tuning, not through a clamp, so the simulation stays honest.

The math, with Act I values (Warmth max 20, rote act costs 2 Warmth and 2 Spirit):

- One full Warmth bar = 10 rote acts = **-20 Spirit**. Starting at 100, a complete dump
  lands at **80**, still in the top band (×1.2).
- Promotions (Beat 5) and received kindness (Beat 7) restore Spirit, resetting the drain.
- To reach Spirit below 50 a player would need roughly 25-plus consecutive rote acts with no
  top-up, which exceeds the Warmth and content available in an Act I session.

So depletion past the reveal threshold is not reachable in Act I by construction. Use a soft
floor (for example, do not let Act I or II Spirit fall below ~60) only as a backstop against
edge cases, not as the primary mechanism. Preferred order: tune budgets so it cannot happen;
floor as insurance.

### Phase 3 — The reveal trigger (Act III)
- **Condition:** the first time Spirit crosses **below 50** (out of the ×1.0 band into the
  ×0.6 "landing flat" band).
- **Why it cannot fire earlier:** Act I and II content caps Warmth budgets and supplies
  regular top-ups, so sustained depletion below 50 is not achievable (Phase 2).
- **Why it fires in Act III:** the crisis content provides long, top-up-free sessions with
  abundant available acts, and genuine and brave acts cost more Spirit (-4, -8). A player
  grinding volume through a crisis session naturally pushes Spirit below 50 for the first
  time.

### Phase 4 — The reveal behavior (the back-fill)
When Spirit first crosses below 50:

1. The meter animates into existence for the first time.
2. It **back-fills**: it shows the player the history it has been recording, the curve of
   their Spirit over this session (and optionally across the campaign), making visible that
   their recent acts have been paying at ×0.6, not ×1.2.
3. The gut-punch is retroactive: "this was happening the whole time, and I could not see it."
   This is why Phase 1 must record from Beat 2. The reveal surfaces a real history, not a
   fabricated one. A meter that began tracking only at the moment of reveal would feel cheap
   and the player would sense it.

No character explains the meter. The reveal is mechanical and felt, per principle 4 (main
doc Section 2). Any accompanying dialogue should react to the player's discovery, never
pre-empt it.

### Phase 5 — Edge cases to handle
- **The determined Act I grinder.** Covered by Phase 2 (cannot reach below 50) plus the soft
  floor backstop.
- **A player who reaches Spirit below 50 in Act II** (longer content than Act I). Decide
  deliberately: either extend the same budget discipline through Act II to hold the reveal
  for Act III, or accept that an unusually persistent Act II player triggers the reveal a
  little early. The reveal is robust either way, but holding it for the Act III crisis gives
  the strongest narrative landing. Recommend holding it.
- **Spirit at 0.** Out of scope for this onboarding slice but flagged in the main doc Section
  17. Define what the ×0.3 band and a full depletion actually offer the player before Act III
  ships.

---

## UI notes specific to Act I

- **Reach is loud, kindness-energy is quiet.** Reach gets the big celebratory treatment;
  kindness-energy is present but visually secondary. This asymmetry is the seed of the whole
  Goodhart arc and must be deliberate, not an accident of layout.
- **No Spirit affordance of any kind.** Verify there is no meter, badge, stat, tooltip, or
  settings entry that references Spirit in Act I builds.
- **Streaks are celebrated; decay is silent.** Sincerity decay should be effectively zero in
  Act I content so volume reads as pure upside.

---

## Acceptance criteria (how to know onboarding worked)

- A new player can complete their first act within seconds of gaining control, with no
  written instruction beyond the single highlighted button.
- At session end, asked what the game is about, a playtester says something about spreading
  kindness and climbing, and talks about their Reach number. They do **not** mention Spirit
  or any cost of giving.
- Playtesters report the first session felt good and they would return. Volume felt
  rewarding.
- In instrumentation, Spirit was recorded every act and never fell below the top band for any
  player, and no player saw any Spirit UI.
- The Beat 8 whisper went consciously unnoticed by the large majority of playtesters (it
  should be recoverable on a replay, not salient on a first run).

---

## Open questions specific to this slice

- Exact copy for the founder's wall quote, written so it plays straight on first read and
  turns ironic on replay.
- The precise form of the Beat 8 whisper: flat recipient response vs reduced kindness-energy
  payout. Pick one and test which is recoverable-but-not-salient.
- Whether promotions restore Spirit fully or partially, and how that interacts with the
  reveal-proof math if Act I content is later expanded.
- Session length and Warmth budget for Act I once real act content exists per department.
