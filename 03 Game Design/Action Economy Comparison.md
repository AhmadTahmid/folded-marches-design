---
id: design-action-economy-comparison
status: draft
origin: assistant-authored controlled paper comparison following user-authorized combat review
updated: 2026-09-28
---
# Individual activations or shared actions?

**Question:** does flexible command allocation make five active companions more satisfying, or concentrate play on a few? This is a worked author exercise, not a human playtest or a new combat selection. [Combat Design Review](Combat%20Design%20Review.md) records the source ideas and assessment. [Tactical Combat](Tactical%20Combat.md), [Status and Counterplay](Status%20and%20Counterplay.md) and [First Region Creature Kits](First%20Region%20Creature%20Kits.md) supply the unchanged cards.

## Hold the scene and cards constant

On a supervised rescue rig above Rocca's lower terraces, two padded medicine panniers must be raised before the practice hoist departs. Friendly rival creatures contest the mechanism. This fixture is an author-created training arrangement, not a new campaign quest or proof that creatures arbitrarily attack medicine deliveries.

**Objective:** complete six ratchet strokes across three rounds, with at most two strokes per round, then have at least one friendly creature standing at the end of round 3. Two available teeth are shown each round. After both engage, the rig must settle until the next round. The hoist departs only after round-3 effects resolve. Defeating every rival ends their attacks but does not advance the hoist clock or cancel the objective. Missing a stroke window fails the practice; concede and retry immediately if desired. There is no injury, lost inventory, payment or recruitment gate.

**Turn the ratchet** is a fixture-only Physical, non-Attack action: a standing front-row creature spends one activation in A or one action point and one personal command slot in B; Focus 0, no cooldown. It adds one stroke if the round has a free tooth. It is stationary, so Root alone does not prevent it. Silence and Disarm do not prevent it; Stagger is resolved as specified below. No free keeper interaction, extra body, movement or passive progress occurs. All normal equipped commands remain available.

The friendly team starts with full benchmark HP and 3 Focus each: Bellwether **B** (32 HP), Thimbleback **T** (30, Armor 2), Glassgrazer **G** (36, Armor/Ward 2), Embermole **E** (26), Doorling **D** (24). Front: B/T/G; rear: E/D. Unlisted defenses are zero. Cards and cooldowns are exactly those in the kits page; no talents, Duets or new identity-revision cards participate.

The rival team also uses the kits' complete bodies and cards: Bellwether **b** (32 HP) in front 1; Thimbleback **t** (30 HP, Armor 2) in front 2; Doorling **d** (24 HP) in rear 1. All start at 3 Focus. Queue order is b, d, t. Display the following intentions each round; the full script is available to the facilitator for reproduction.

| Rival | Round 1 | Round 2 | Round 3 |
|---|---|---|---|
| b | Horn Run at T: 12 Impact | Strike at T: 8 Impact | Horn Run at T: 12 Impact |
| d | Muffle E: Silence | Guard self: Barrier 8 | Muffle G: Silence |
| t | Nut Pitch D: 8 Impact | Nut Pitch D: 8 Impact | Nut Pitch D: 8 Impact |

If a named target is exhausted or unreachable, a rival's damage action substitutes the lowest-numbered legal front target, then rear if its delivery permits; if none exists, Guard. An invalid Muffle target becomes the first standing friendly in B/T/G/E/D order. If Silence prevents Muffle, use Guard; if Disarm prevents a listed attack, use Guard. These fallback choices are displayed before commitment. Defeated rivals are removed from the queue. All partial effects expire normally; Resolve is the stated exception. Round 1 starts friendly, round 2 rival, round 3 friendly. After the rival queue ends, remaining friendly commands still resolve.

## Two exact allocation rules

**A — baseline:** each standing friendly has one activation per round. Pick any unacted creature. Unspent activations disappear if that creature is exhausted. Enemy alternation, Focus, cooldowns and formation remain unchanged.

**B — experimental:** begin each round with five shared action points, discarded at round end. Any standing friendly may receive at most two commands that round. Each command costs one point, plus its usual personal Focus, and prompts the same next rival activation while any remain. Strike, Guard, Move and ratchet work can repeat; technique cooldowns still prevent repeating a cooldown-1 or longer technique in that round. Moving another creature grants it no command. Focus still belongs to each creature and recovers only once at round start.

Five points is intentional: it keeps the maximum number of executed friendly commands equal for this first comparison. Exhaustion does not remove unspent shared points; surviving creatures can use them within their two-command caps. With too few eligible survivors, excess points expire after the rivals finish. This makes concentration and recovery from exhaustion potential benefits as well as balance differences. Do not claim the variants differ only cosmetically.

**B's necessary Stagger extension:** friendly eligibility requires zero personal slots spent, an unreserved team point remaining, and no blocking protection. Stagger reserves one team point for that creature's lost command. The player can command another creature using unreserved points, including a Strong Cleanse that removes Stagger, frees the reservation and grants normal Resolve. Selecting the staggered creature instead consumes its reserved point and one personal slot without an action, then grants Resolve and triggers the usual rival response. It may later use its second slot. If only reservations remain, settle them in B/T/G/E/D order. Exhaustion removes the affected creature and releases its reservation. A creature already commanded once cannot newly receive Stagger, even if its second slot remains. Rivals retain baseline Stagger because they still act once. This extra reservation rule is itself a complexity cost; the worked lines below only Stagger a rival and therefore do not validate this extension in play.

In both variants, use available legal commands until the side's allocation is spent; the ordinary practice-concede option remains available. There is no free mid-round reset or undo after confirming a command.

## Worked line A — each companion contributes once

Numbers in the first column are friendly command order within that round. Rival replies appear on the same row when they follow the command. **Ratchet n** is the cumulative completed stroke count. Costs below are Focus; common commands and ratchet work cost 0.

| Round / command | Friendly action and immediate effect | Rival reply |
|---|---|---|
| 1 / 1 | B: Arresting Peal b, cost 2; Stagger | b loses its action; Resolve through round 2 |
| 1 / 2 | T: ratchet 1 | d: Muffle E, Silence |
| 1 / 3 | D: Unknot E, cost 1; remove Silence | t: Nut Pitch D; D 24 → 16 |
| 1 / 4 | E: Furnace Breath b, cost 1; b 32 → 20 | Queue finished |
| 1 / 5 | G: ratchet 2 | — |
| 2 / opening | No friendly action yet | b: Strike T; 8 − 2 Armor = 6; T 30 → 24 |
| 2 / 1 | T: ratchet 3 | d: Guard, self Barrier 8 |
| 2 / 2 | D: Borrowed Screen self, cost 1; Barrier 8 | t: Nut Pitch D; screen absorbs all 8 |
| 2 / 3 | G: ratchet 4 | Queue finished |
| 2 / 4 | B: Strike b; b 20 → 12 | — |
| 2 / 5 | E: Warm Thread b, cost 1; b 12 → 4 | — |
| 3 / 1 | E: Furnace Breath b, cost 1; b 4 → 0, removed | d: Muffle G, Silence |
| 3 / 2 | G: ratchet 5; Physical remains legal | t: Nut Pitch D; D 16 → 8 |
| 3 / 3 | D: Strike d; d 24 → 19 | Queue finished |
| 3 / 4 | T: ratchet 6 | — |
| 3 / 5 | B: Strike t; 8 − 2 Armor = 6; t 30 → 24 | — |

The round-2 screens expire before round 3. Furnace Breath used in round 1 is ready in round 3. Peal used in round 1 remains unavailable until round 4; round-2 Resolve also blocks restaggering b. Strong Cleanse would spend scarce effort on G's round-3 Silence without improving its Physical ratchet action.

## Worked line B — concentrate the work

Use the same initial state, enemy script and objective. A double command does not skip an intervening rival activation while one remains.

| Round / command | Friendly action and immediate effect | Rival reply |
|---|---|---|
| 1 / 1 | B: Arresting Peal b, cost 2 | b loses its action; Resolve through round 2 |
| 1 / 2 | G: ratchet 1 | d: Muffle E, Silence |
| 1 / 3 | D: Unknot E, cost 1 | t: Nut Pitch D; D 24 → 16 |
| 1 / 4 | G: ratchet 2, second personal command | Queue finished |
| 1 / 5 | E: Furnace Breath b, cost 1; b 32 → 20 | — |
| 2 / opening | No friendly action yet | b: Strike T; T 30 → 24 |
| 2 / 1 | B: Strike b; b 20 → 12 | d: Guard, self Barrier 8 |
| 2 / 2 | D: Borrowed Screen self, cost 1 | t: Nut Pitch D; screen absorbs all 8 |
| 2 / 3 | B: Strike b again; b 12 → 4 | Queue finished |
| 2 / 4 | G: ratchet 3 | — |
| 2 / 5 | G: ratchet 4, second personal command | — |
| 3 / 1 | E: Furnace Breath b, cost 1; b 4 → 0 | d: Muffle G, Silence |
| 3 / 2 | D: Guard self; Barrier 8 | t: Nut Pitch D; screen absorbs all 8 |
| 3 / 3 | G: ratchet 5 | Queue finished |
| 3 / 4 | G: ratchet 6, second personal command | — |
| 3 / 5 | E: Warm Thread d, cost 1; d 24 → 16 | — |

## What these lines actually show

Both complete six strokes and win after round 3. Neither is claimed optimal.

| End-of-round checkpoint | A | B |
|---|---|---|
| Friendly HP, round 1: B/T/G/E/D | 32 / 30 / 36 / 26 / 16 | Same |
| Friendly HP, round 2 | 32 / 24 / 36 / 26 / 16 | Same |
| Friendly HP, round 3 | 32 / 24 / 36 / 26 / 8 | 32 / 24 / 36 / 26 / 16 |
| Friendly Focus, round 1: B/T/G/E/D | 1 / 3 / 3 / 2 / 2 | Same |
| Friendly Focus, round 2 | 2 / 3 / 3 / 2 / 2 | 2 / 3 / 3 / 3 / 2 |
| Friendly Focus, round 3 | 3 / 3 / 3 / 2 / 3 | 3 / 3 / 3 / 1 / 3 |
| Rival HP, round 3: b/t/d | 0 / 24 / 19 | 0 / 30 / 16 |
| Total friendly commands | 15 | 15 |
| Commands per companion: B/T/G/E/D | 3 / 3 / 3 / 3 / 3 | 3 / 0 / 6 / 3 / 3 |

B illustrates useful concentration: G performs all objective work, B repeats its free attack, and E can later use two different techniques. T remains present, takes a hit and screens the rear, but receives **no command in three rounds**. A gives every partner a task, including repetitive ratchet work. Neither count alone proves attachment or enjoyment.

B's extra eight remaining Doorling HP is not evidence of superior play: A could Guard D in round 3 instead of its five-damage Strike and preserve the same HP. Its offensive outcome would change. Compare the decision opportunities and sacrifices, not just one selected line's final totals. B's second Warm Thread also spends an additional personal resource that A retains.

## Next human comparison and provisional recommendation

Let fresh participants choose their own actions from the same starting state, with reference cards and all legal options. Counterbalance A/B order, record prior genre familiarity, and separate unfamiliarity with the cards from confusion about allocation. Record decision time, inspections, rule corrections, idle companions, repeated strongest-attacker use, and whether players can explain the consequence they intended. Ask which companion felt useful, whether they wanted another encounter, and what made a turn drag. No such sessions have occurred in this pass.

Check another objective that cannot be monopolized so easily and a fight with endangered allies before generalizing; this hoist deliberately exposes concentration. Then, if B remains promising, separately compare three shared points with enemy pressure retuned and documented. That changes pacing and throughput as well as allocation. Replacing personal Focus at the same time would add another variable; test it separately.

**Working recommendation:** retain A as the coherent baseline while B remains a reviewable alternative. B has a real tactical affordance, not an established simplification. Its Stagger extension, concentrated free attacks and uncommanded companions need scrutiny. Shorter battle duration, faster choices, fun, phone readability and Dota-like intensity are all unmeasured.
