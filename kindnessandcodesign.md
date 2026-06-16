# Kindness & Co — Game Design Document (v0.1)

> A social/live-service game where the player rises through a company whose entire
> business is spreading kindness. Structurally it borrows the proven systems craft of
> early social games (tight core loop, layered resources, progression-as-reset,
> social-graph-as-power, appointment mechanics, a content treadmill) and deliberately
> **inverts every extractive drain** so the systems serve the player's wellbeing and real
> relationships instead of an operator's metrics.

## Provenance and status

This document is a design exploration. It was built by reverse-engineering the systems of
a classic extractive social game (Mafia Wars) and consciously detoxifying each part for a
game about kindness. **Every number below is illustrative**, chosen to show the shape of a
curve or the relationship between variables. Treat all constants as a starting point for a
tuning spreadsheet, not as final values. The relationships between the numbers are the
actual design; the exact values are a balancing job.

Nothing here is built yet. See "Build guidance" at the end for the suggested first
vertical slice.

---

## 1. Concept

The setting is **Kindness & Co**, a company where everyone learns to spread kindness, in
the spirit of Monsters Inc where the monsters all learn to scare. The player starts in the
**mail room** and rises through the company.

The Monsters Inc framing is load-bearing, not cosmetic. In that film the plot is an
energy-source swap: scream power turns out to be weaker than laughter, and the whole
factory retools. Here, **kindness is the literal power source of the world**. Scream-energy
becomes kindness-energy. That single move means the economy *is* the message: every
mechanic is automatically on-theme because the resource the world runs on is kindness
itself.

### The central design problem

A kindness game cannot just reskin an extraction engine. If you paint the energy bar pink
and rename "attack" to "compliment," you build a game that manipulates people into
engagement while preaching kindness, and an honest player feels the extraction under the
warm paint within a week. So the job is to keep the parts of the DNA that are pure craft
and consciously invert the **drains**, the places where the original routed everything
toward the operator's wallet.

---

## 2. Non-negotiable design principles

These are the constraints that protect the whole design. Violating any one of them
re-toxifies the game.

1. **Depth over volume.** One genuine or brave act must out-earn a hundred rote ones. This
   is encoded in the payout math, not delivered as a message (see Section 6).
2. **Glow flows outward only.** The soft currency buys things that go out into the world
   (supplies, community spaces, cosmetics). It can **never** be spent to refill Warmth or
   Spirit. The moment money or currency can resolve the fatigue wall, the message collapses.
3. **No pay-to-skip-fatigue.** Warmth refills only through time. Spirit refills only
   through rest, receiving kindness, and reflection. These relief valves are the behaviors
   the game exists to teach, so they are never for sale.
4. **Discover, never lecture.** The player must learn every lesson (especially
   depth-over-volume) by watching their own numbers. If a character stops the action to
   explain the moral, the design has failed.
5. **Growth through worth, not spam.** The game grows because its artifacts are worth
   sharing (see Ripples, Section 9), never because progress is held hostage behind invites.

---

## 3. Core loop

The atomic action is performing a small **act of kindness**. It costs **Warmth** and pays
out **kindness-energy** (the world's fuel) plus **Glow** (soft currency), and sometimes a
**Ripple** (a collectible story of where the kindness traveled).

```
spend Warmth  ->  do an Act  ->  earn kindness-energy + Glow (+ sometimes a Ripple)
     ^                                          |
     |                                          v
  refills via time / promotion        reinvest Glow into supplies & community spaces
```

When the player runs low, they hit a soft wall, and the wall resolves to one of three
exits. This is the key inversion (Section 5).

---

## 4. Resource systems

The design runs on three player resources that form a triangle, plus the world fuel.

- **Warmth** governs *how much* you can do (the energy gate).
- **Spirit** governs *how well it lands* (a payout multiplier).
- **Glow** is the *output* you reinvest.
- **kindness-energy** is the world's fuel and the true score. It is what the company
  actually needs and what the narrative is about (Section 11).
- **Courage** is a secondary gate spent only on Brave Acts (Section 6).

### 4.1 Warmth (the gate, deliberately humane)

In the extractive original, regen is a fixed constant while capacity balloons, so
refill-from-empty stretches from ~90 minutes to ~25 hours over a player's life, and that
widening gap is the wallet funnel. **We invert this: Warmth regen scales up with rank**, so
refill time stays roughly flat for the entire game. This is a statement of intent: we are
not selling refills, so we never let the wait become a punishment only money solves.

| Rank | Warmth max | Regen / hr | Refill from empty |
|---|---|---|---|
| Mail Room | 20 | 14 | ~85 min |
| Small Gestures | 50 | 36 | ~85 min |
| Community Outreach | 90 | 64 | ~85 min |
| Crisis Response | 120 | 85 | ~85 min |

Because Warmth is generous, the real scarcity lives in **Spirit** and in the payout curve,
not in waiting for the gate to refill.

### 4.2 Spirit (the multiplier that self-regulates burnout)

Spirit sits at 0 to 100 and starts at 100. Every act spends a little. Your Spirit band sets
a multiplier on everything you produce.

| Spirit band | Payout multiplier | What it feels like |
|---|---|---|
| 80–100 | ×1.2 | giving your best |
| 50–79 | ×1.0 | steady |
| 25–49 | ×0.6 | acts landing flat |
| 0–24 | ×0.3 | running on empty |

Spirit cost per act: small act -2, genuine act -4, brave act -8.

This does the work a hard daily cap would do, without the paternalism. The player is never
blocked. Depleted grinding is simply inefficient, so the rational choice and the healthy
choice become the same choice: stop, rest, receive, reflect, then give from a full cup at
×1.2. The bonus sits at the top of the range, which means the game rewards people for **not**
grinding themselves to zero.

Note: in the campaign, the Spirit meter is **hidden during Act I** and revealed at the Act
III crisis. See Section 11.

### 4.3 Courage

A separate small gate spent only on Brave Acts. Brave acts are the highest-value,
emotionally costly kindness (reaching out to someone clearly struggling, a real apology,
kindness returned to someone who was unkind first). Courage regenerates slowly and is the
intended replacement for the original game's "attack" resource: same architecture, opposite
act.

---

## 5. The three exits (the core inversion)

In the extractive original, every wall exists to manufacture three exits: **wait, recruit,
pay**, two of which feed the operator. Here the wall ("running low / kindness fatigue")
resolves to three exits that feed the **player** or a real relationship:

| Exit | What it is | What it replaces |
|---|---|---|
| **Rest** | Framed as restoration. The game offers something gentle or simply blesses the break. | Wait (retention), but restorative rather than punitive |
| **Receive** | Someone in your Circle sends you Warmth/Spirit. | Recruit (viral), but mutual care rather than invite pressure |
| **Reflect** | A short gratitude pause that nudges wellbeing and grants a small refill. | Pay (revenue), removed from the core loop entirely |

**There is no Pay exit in the core loop.** Monetization sits outside it (Section 12).

---

## 6. Acts, payouts, and the depth-over-volume engine

Three act types, with payouts **before** the Spirit multiplier:

| Act type | Warmth cost | Other cost | kindness-energy | Glow |
|---|---|---|---|---|
| Rote small act | 2 | — | 5 | 3 |
| Genuine / personalized act | 5 | Spirit -4 | 15 | 8 |
| Brave act | 10 | Courage + Spirit -8 | 50 | 25 |

A genuine act is a 3x depth premium over rote. A brave act is a full 10x.

### Sincerity decay

Repeating the **same** rote act back to back pays 15% less each time, down to a floor of
roughly 30%. Variety and genuineness avoid the decay. **Brave acts never decay.** This is
the anti-grind mechanic: it taps the exact mindless-volume behavior the company has been
wrongly optimizing for.

### The worked comparison (the thesis, as math)

Give two players the same 100 Warmth in a session. One grinds rote acts; one plays for
depth and manages Spirit by receiving between acts. Cumulative kindness-energy, indexed:

| Warmth spent | Volume grinder (rote) | Depth player (genuine + brave) |
|---|---|---|
| 0 | 0 | 0 |
| 20 | 40 | 70 |
| 40 | 65 | 150 |
| 60 | 80 | 240 |
| 80 | 90 | 330 |
| 100 | 95 | 430 |

Same Warmth in, roughly **4.5x** the kindness out. The grinder's curve is concave (sincerity
decay plus falling Spirit eat each successive identical act, so it asymptotes). The depth
player's curve keeps climbing (brave acts never decay; receiving keeps them in the ×1.2
band). The player does not need to read this table to learn it; they feel it in their own
totals within two sessions. That felt discovery is the entire theme, expressed as economics.

---

## 7. Glow economy (faucets and sinks)

Glow is the soft currency and follows ordinary faucet-and-sink discipline, with the
outward-only rule from Section 2 as an absolute constraint.

**Faucets:** acts (3 / 8 / 25 Glow by type), passive trickle from community spaces,
one-time lumps from promotions and completed Ripple sets.

**Sinks:**
- *Supplies* (recurring): small consumables, e.g. a "personal touch" that raises an act's
  quality.
- *Community spaces* (capital sink, the heavy lifter): escalating cost with deliberately
  lengthening payback, which keeps Glow scarce enough to feel worth earning and gives
  long-horizon goals. This is also the appointment mechanic in kind form: you return to
  *tend* spaces that visibly do good and accrue value while you are gone.
- *Cosmetics* (optional): decorate your mail room and your spaces.

| Community space | Cost (Glow) | Passive Glow / day | Payback |
|---|---|---|---|
| Little free library | 200 | 20 | 10 days |
| Community garden | 800 | 50 | 16 days |
| Repair café | 2,500 | 110 | 23 days |
| Neighborhood hub | 8,000 | 280 | 29 days |

Payback stretches from 10 to 29 days as you climb (diminishing ROI), which is the classic
escalating sink that prevents currency inflation.

**Load-bearing rule, restated:** Glow flows outward into the world and never inward to
refill the gates. Glow buys supplies, spaces, and cosmetics. Glow can never buy Warmth or
Spirit.

---

## 8. The resource triangle

The three resources form a closed triangle rather than a line:

- **Warmth** sets how much you can do.
- **Spirit** sets how well it lands.
- Together they produce **kindness-energy** and **Glow**, which you reinvest into supplies
  and spaces that raise tomorrow's ceiling.
- Your **Circle** quietly refills both Warmth and Spirit (Section 10).

No single resource dominates, and none has a wallet shortcut into the others.

---

## 9. Ripples (collections, deliberately not a slot machine)

When an act ripples (a note that travels through five people), the player collects the
**story** of where it went. Completing a Ripple set grants a permanent bonus plus a small
narrative payoff.

Design choice to enforce: **completion is deterministic-with-effort, not
random-with-paywall.** The extractive original used a variable-ratio schedule with a rare
last item (the slot-machine near-miss); we consciously refuse that tuning. We lose some
compulsive pull and earn it back through narrative and the social loop. Ripple stories are
also the genuine, shareable artifacts that drive growth-through-worth (principle 5): people
share them because they are good, not because the game held progress hostage.

---

## 10. The Kindness Circle (social-graph-as-power, inverted)

Your Circle's size genuinely matters, but it multiplies **replenishment and reach**, not
force. A bigger Circle means more kindness flows back to refill your Warmth and Spirit, and
unlocks larger cooperative acts (a block party, a fundraiser) that no solo player can pull
off. Watching your kindness land on a real person is empathic joy (mudita), the most
replenishing reward in the system.

The original grew through invite spam, and spam is unkind, so it would poison the theme.
Growth here must come from the artifacts being worth sharing on their own (Ripples), never
from "invite five friends to get stronger."

Async support replaces async attack: the original's "someone attacked me while I was gone,
I want revenge" becomes "someone left me a kindness while I was offline, and I want to pass
it on." Same retention architecture, opposite emotion.

---

## 11. Progression spine (the volume-to-depth narrative arc)

The intellectual engine is **Goodhart's law**: when a measure becomes a target, it stops
being a good measure. The company measures **Reach** (raw volume of kindness dispatched),
displayed on a giant **Dispatch Board** everyone worships. The world actually runs on
**kindness-energy**. The tragedy is that Reach and kindness-energy used to move together and
have silently decoupled.

Texture that keeps the company from being a cartoon villain: it was *founded* on depth. The
founder's original insight was real; the institution drifted to volume after her era simply
because volume was easier to count and scale. The endgame is therefore a **restoration**,
not an invention.

The progression must teach this by experience, never by cutscene. Promotions double as the
level curve and as resource resets (each promotion refills Warmth and grants stat points to
allocate). The departments/floors are the content treadmill: Mail Room, Cards & Letters,
Small Gestures, Community Outreach, Crisis Response. You add a floor, not a redesign.

### Five acts and a coda

**Act I — The Mail Room (induction).** Learn the loop, worship volume, get celebrated for
Reach. Only rote acts available, Warmth generous, promotions fast. **The Spirit meter is
hidden.** The player cannot see what volume is costing them. This is the game at its most
extractive, on purpose: the tutorial is the company's indoctrination.

**Act II — The Climb.** Master volume, rise through Cards & Letters and Small Gestures,
become a star. This is the region where the depth-versus-volume lines still overlap (volume
genuinely looks fine), so the player has no reason to doubt the metric. Pacing rule: never
show the divergence early, or the lesson is cheap. End on a hairline crack, not a
revelation (a recipient response that does not compute as a number).

**Act III — The Plateau (midpoint crisis).** A company-wide energy crisis: Reach at record
highs, kindness-energy dimming, nobody can explain it because the dashboard has never looked
better. **Reveal the Spirit meter here for the first time.** The player learns their acts
have been landing flatter for hours. The depth-versus-volume lines visibly diverge; grinding
stops paying. A single case that volume cannot solve forces the player's first brave act,
which pays out more than their last hundred dispatches combined. The thesis, felt in their
own totals.

**Act IV — The Relearning.** The player finds the sidelined unit (the people who kept doing
depth and were punished with low Reach) and a mentor who never bought the quota religion.
The founder's original insight resurfaces. Full second-half mechanics come online: brave and
genuine acts become primary, sincerity decay bites old habits, Spirit management becomes the
real game, and the receive-and-Circle loop turns load-bearing (depth depletes you; you
cannot solo it). Play changes from fast dispatch-spamming to slow, relational, careful work.

**Act V — Retuning the Board (endgame).** Personal change is not enough; the company still
worships Reach and the crisis is existential. Now senior, the player has standing to change
**what the Dispatch Board measures.** The climax is a decision, not a fight: choose a metric
that cannot be juiced by quietly re-toxifying the system, swapping hollow Reach for something
that captures depth and resonance. This is the literal in-fiction version of the north-star
problem from the tuning dashboard (Section 13). The victory is systemic.

**Coda — The Practice.** Post-campaign, the game becomes the sustainable loop with no
extractive pull, fed by live-ops (new community needs, seasonal crises, new floors). The
spine's job was to carry the player out of the grind into the durable mode. The endgame is
not a number to maximize, it is a practice to keep.

### The metric arc (indexed)

The whole tragedy is that the company's own dashboard betrays no problem at any point. The
gray Reach line never dips, which is exactly why the crash blindsides everyone.

| Act | Reach (dashboard) | True kindness-energy |
|---|---|---|
| I Mail Room | 20 | 18 |
| II Climb | 45 | 38 |
| III Plateau | 70 | 22 |
| IV Relearning | 88 | 58 |
| V Retune | 100 | 96 |

The gap is widest at Act III (the crisis) and closes by Act V (recoupling). This is the same
shape as the in-session depth-versus-volume curve, at a different zoom: that one shows the
divergence inside a single session, this one shows it across the company's whole history.
The micro teaches the macro.

---

## 12. Monetization (ethical model)

Monetization sits **outside** the core loop, never as a refill or a power gate.

- **Cosmetics** for your mail room and your spaces.
- **Pay-it-forward purchases**: buying a real-world equivalent (a donation, a coffee for a
  stranger via a partner) unlocks an in-game cosmetic, so spending money *is itself a kind
  act* rather than a shortcut past one.
- **Patron tier** that supports development.

Absolute rule: the wallet must never resolve the kindness-fatigue wall. The moment you can
buy your way out of compassion fatigue, the whole message collapses.

---

## 13. Tuning levers (the live-ops dashboard)

Every lever has a "better metrics" direction that quietly betrays the theme. Here the
failure mode is not under-monetizing, it is **re-extracting**. Each lever is a tension
between two ways of being wrong.

| Lever | Cranked too high | Dropped too low | Governs |
|---|---|---|---|
| Depth premium | brave acts feel mandatory; depth becomes its own burnout grind; the rote on-ramp collapses for new players | volume wins again and the thesis evaporates | message integrity, mid-game difficulty |
| Sincerity decay | feels punitive and surveilling; punishes honest daily repetition | grind and bot farming return | anti-exploit vs player trust |
| Spirit multiplier | the wellbeing nudge curdles into scolding; a door slammed on anyone who pushes through | grinding to empty costs nothing, so rest and receive go inert | pacing, burnout prevention |
| Rank-scaled regen | Warmth stops mattering; the gate vanishes; acts feel weightless | late-game refill balloons and players churn with no relief valve we will sell | session cadence, high-rank retention |
| Space cost curve | endless saving toward nothing reachable; the Glow faucet backs up | Glow inflates; passive income outpaces acts and the game plays itself | Glow's felt value, long-horizon goals |
| Receive-refill | the Circle becomes mandatory; invite pressure and spam return | the social loop turns decorative and mutual care dies | social retention, design equity |

### The three clusters (they are not independent)

1. **Volume-farming guard** = depth premium + sincerity decay. Tune as a pair. Raise the
   premium and you can relax the decay (depth already out-earns farming). Cranking both
   punishes the same behavior twice and feels mean.
2. **Glow faucet and sink** = act payouts (driven by the depth premium) + space cost curve.
   One system. Sweeten payouts to push depth and more Glow floods in; if you do not steepen
   the cost curve to match, the currency inflates and passive income takes over.
3. **Wellbeing subsystem** = Spirit curve + rank-scaled regen + receive-refill. Together
   these decide whether the game paces people humanely or either coddles them into
   weightlessness or grinds them flat. This is where the values live, and the cluster most
   tempting to sabotage under pressure.

### The north-star warning

When a retention number dips, the cheapest fix is always a turn toward extraction (steepen
regen to manufacture urgency, crank receive-refill so people feel they must recruit, quietly
drop the depth premium because the mindless grind retains the distractible player a little
better). Each works next week and corrodes the thing over a year, invisibly, because the
dashboard still looks healthy.

Defense: pick a north-star you cannot juice by re-toxifying. **Not** daily actives or
minutes-in-app (any lever inflates those on demand). Instead something like **sustainable
depth**: are people doing meaningful acts, at a healthy Spirit, returning without being
coerced. If that number is up, you earned it. If retention is up but that number is flat,
you did not fix the game, you found a new way to extract from it, and you should put the
lever back.

---

## 14. Design risks

1. **The Act-I-too-good trap.** If the volume grind is genuinely compelling (and it should
   be), you have built an extractive game with a redemption arc bolted on the far end, and
   most players quit before the turn. **Time-to-turn is the single most important pacing
   decision in the project.** Act III must land within a player's first few sessions, not
   weeks in. But pull it too early and they never built the belief the turn is meant to
   shatter. Living in that narrow band is the job.
2. **Preachiness.** The turn must be discovered in the numbers, never delivered in a
   cutscene. The moment a wise character explains that depth beats volume, the design has
   failed.
3. **The resentment trap.** "Your volume era was a mistake" retroactively invalidates the
   player's Act I and II effort and can leave them feeling tricked. Fix it in the framing:
   the volume era was an **apprenticeship, not a folly**. Sulley had to become the best
   scarer in the building before he could discover laughter. The skill transfers entirely;
   only the metric changes.
4. **Acceptable loss.** The player who reaches Act II, decides they only ever wanted the
   grind, and leaves, is the correct loss to take. This game is not for the person who only
   wants to extract, and declining to chase them is itself a design statement.

---

## 15. Mafia Wars to Kindness & Co (the mapping, for reference)

| Original (extractive) | Kindness & Co (inverted) |
|---|---|
| Energy (gate to wallet) | Warmth (gate, regen scales with rank so refills stay humane) |
| Stamina + async PvP attack | Courage + async mutual support |
| Health (worn down to push healing/pay) | Spirit (effectiveness multiplier; teaches sustainable giving) |
| Money | Glow (flows outward only) |
| Properties (passive rent) | Community spaces (passive good you tend) |
| Loot collections (slot-machine near-miss) | Ripples (deterministic, narrative, shareable) |
| Mafia size = combat power; invite spam | Circle = replenishment and reach; growth through worth |
| Cities (NY, Cuba, Moscow) | Departments/floors (Mail Room ... Crisis Response) |
| Premium currency to skip the wall | Monetization outside the loop; never skips fatigue |
| Exits: wait / recruit / pay | Exits: rest / receive / reflect (no pay in core) |

---

## 16. Build guidance (suggested first vertical slice)

Do not build all of this at once. The tractable, testable first slice is the **core loop
with the depth-over-volume engine made legible**, because that is where the whole thesis
lives. Concretely:

1. Warmth as a regenerating gate (single rank to start; the rank-scaling can come later).
2. The three act types (rote / genuine / brave) with the payouts in Section 6.
3. The Spirit multiplier (Section 4.2), **including the Act I reveal hinge**: build it so the
   meter can be hidden and then revealed, because that reveal is the moment the entire
   campaign swings on.
4. Sincerity decay on repeated rote acts.
5. A simple readout that lets a playtester *see* their cumulative kindness-energy, so the
   depth-versus-volume divergence is felt, not explained.

Glow, community spaces, the Circle, Ripples, and the full five-act narrative are layers to
add once the core loop proves that depth-over-volume is fun to discover rather than annoying
to be told.

A useful companion tool for the team (not player-facing) would be an interactive version of
the Section 13 dashboard: six sliders for the levers wired to a live readout of the
depth-versus-volume curve and the Glow balance, so the team can feel the couplings instead
of arguing about them in the abstract.

---

## 17. Open questions / not yet designed

- The Act I mail-room onboarding, beat by beat, including the exact trigger and staging of
  the Spirit-meter reveal.
- Concrete act content per department (what an act actually *is* on each floor).
- The Courage economy in detail (regen rate, what gates a brave act besides cost).
- Cooperative act design for the Circle (how a multi-player act is initiated and resolved).
- The exact replacement metric chosen at the Act V climax, and how it is computed.
- Failure and edge states: what happens at Spirit 0, what "rest" actually offers the player.
