---
id: design-worked-battle
status: draft
origin: assistant paper example with deliberately small proposed numbers
---
# Worked battle — the practice crossing

A supervised keeper challenge uses five companions against three defenders. This is a fully resolved arithmetic example of [Tactical Combat](Tactical%20Combat.md), not a claim that five-against-three is balanced or that these are final creature kits. The challengers win by exhausting the defenders; all participants recover afterwards. No narrative canon or ecological change is implied.

## Starting state

All start with 3 Focus, no effects and ready techniques. The player opens round 1. Positions are fixed for this exercise. The HP values deliberately keep the demonstration short.

| ID / creature | Side / row | HP | Armor / Ward | Strike |
|---|---|---:|---|---|
| T — Thimbleback | Player / front | 30 | 2 / 0 | 6 Impact, Melee |
| B — Bellwether | Player / front | 32 | 0 / 0 | 8 Impact, Melee |
| G — Glassgrazer | Player / front | 36 | 2 / 2 | 6 Impact, Melee |
| E — Embermole | Player / rear | 26 | 0 / 0 | 6 Impact, Reach |
| D — Doorling | Player / rear | 24 | 0 / 0 | 5 Impact, Reach |
| H — defending Glassgrazer | Enemy / front | 24 | 2 / 0 | 10 Impact, Melee |
| C — defending Bellwether | Enemy / front | 20 | 0 / 0 | 8 Impact, Melee |
| W — defending Doorling | Enemy / rear | 10 | 0 / 0 | 5 Impact, Reach |

Species appearance, habitat and temperament remain owned by the [Bestiary](../01%20World/Bestiary.md). An Embermole's Reach Strike here is a small thrown stone; it does not establish humanlike tool use across every individual. This training technique remains a proposal to review alongside animation and ecology.

| Technique / user | Cost / cooldown | Exact effect |
|---|---|---|
| Calling Note / B | 1 / 2 | Accord, Reach; Exposed on one enemy through current round |
| Arresting Peal / B | 2 / 3 | Accord, Reach; Stagger an eligible enemy |
| Pick the Latch / D | 1 / 2 | Physical, Reach; Strip one enemy |
| Unknot / D | 1 / 2 | Physical, Reach; Basic Cleanse one ally |
| Furnace Breath / E | 1 / 2 | Accord, Attack, Reach; 12 Resonance |
| Warm Thread / E | 1 / 1 | Accord, Attack, Reach; 8 Resonance |
| Borrowed Screen / W | 1 / 2 | Physical, Reach; 8 Barrier on one ally through current round |
| Muffle / W | 1 / 2 | Accord, Reach; Silence through current round |
| Horn Run / C | 1 / 2 | Physical, Attack, Melee; 12 Impact |

Technique lists are partial equipped kits, not additional slots. Strike costs no Focus. Armor affects Impact and Ward affects Resonance; delivery and activation tags do not change that formula.

## Round 1 — break the screen

Enemy order and intentions are visible: **W Screen H → H Strike T → C Horn Run B**. All remain legal throughout the chosen line. C's declared fallback, if Horn Run cannot reach B, is Strike against the lowest-numbered legal front slot; T occupies that slot.

| Step | Activation | State change |
|---|---|---|
| 1 | B: Calling Note on H | B Focus 3→2. H Armor 2→0 through round 1 |
| 2 | W: Borrowed Screen on H | W Focus 3→2. H gains 8 Barrier |
| 3 | D: Pick the Latch on H | D Focus 3→2. H Barrier 8→0 |
| 4 | H: Strike T | 10−2 Armor = 8 HP damage; T 30→22 |
| 5 | E: Furnace Breath on H | E Focus 3→2. 12−0 Ward = 12; H 24→12 |
| 6 | C: Horn Run on B | C Focus 3→2. 12−0 Armor = 12; B 32→20 |
| 7 | G: Strike H | 6−0 Armor = 6; H 12→6 |
| 8 | T: Strike H | 6−0 Armor = 6; H 6→0, exhausted |

The enemy has used all three activations before steps 7–8, so the two unused player creatures finish. Calling Note saved two points of Armor reduction on each physical hit: without it, H would retain 4 HP. The enemy's Barrier would have absorbed another 8 damage without Doorling's Strip. Three different roles made the defeat possible within this round.

**Positional alternative:** D could spend step 3 exchanging rows with B instead of stripping H. Horn Run could no longer reach B behind the front line, so C would use its declared Strike fallback against T: 8−2 = 6 additional damage. B would retain 32 HP and T would end at 16. H's unremoved Barrier would absorb 8 of the later damage, leaving H alive at 8 HP. The player saves 6 total HP but faces another enemy activation next round. Moving is a genuine tradeoff, not a free dodge.

## Round 2 — rescue the finisher

Standing creatures regain 1 Focus, bringing every survivor to 3 in this example. The enemy opens. Its declared order is **W Muffle E → C Guard**. H is exhausted and has no activation. B's Calling Note, D's Strip and E's Furnace Breath are unavailable until round 3.

| Step | Activation | State change |
|---|---|---|
| 1 | W: Muffle E | W Focus 3→2. E is Silenced |
| 2 | B: Arresting Peal C | B Focus 3→1. C is Staggered |
| 3 | C: activation lost | Guard does not happen; no resource cost. C gains Resolve through round 3 |
| 4 | D: Unknot E | D Focus 3→2. Silence removed |
| 5 | G: Strike C | 6−0 Armor = 6; C 20→14 |
| 6 | E: Warm Thread C | E Focus 3→2. 8−0 Ward = 8; C 14→6 |
| 7 | T: Strike C | 6−0 Armor = 6; C 6→0, exhausted |

The player prevented Guard before it could resolve, then rescued an Accord user. Without Unknot, E could still Strike for 6; C would survive this sequence at 2 HP and enter round 3 with Resolve. The lower-resource line is legal and changes the next round. Stagger is not a permanent answer: if C survived, another peal in round 3 would fail even if the technique were available.

## Round 3 — cooldowns create another window

The player opens. W intends to Screen itself. With no enemy front remaining, friendly Melee attacks can reach it. Friendly Focus is now T3, B2, G3, E3, D3; W has 3.

| Step | Activation | State change |
|---|---|---|
| 1 | B: Strike W | 8−0 Armor = 8; W 10→2 |
| 2 | W: Borrowed Screen on self | Ready again after round-1 use. W Focus 3→2; gains 8 Barrier |
| 3 | D: Pick the Latch W | Also ready again. D Focus 3→2; Barrier removed |
| 4 | G: Strike W | 6 Impact; W loses its remaining 2 HP, reaches zero; 4 excess damage has no further effect |

Combat ends immediately. E and T do not need meaningless final commands.

The complete [five creature kits](First%20Region%20Creature%20Kits.md) retain these abilities and stats. [Counterplay Battle](Counterplay%20Battle.md) examines two rounds against an equally sized opponent; it is a separate scenario, not an extension of this victory.

## State audit

HP entries follow **T / B / G / E / D** for the player and **H / C / W** for opponents. Focus freezes on exhausted creatures; their retained value has no combat use.

| Checkpoint | Player HP | Enemy HP | Player Focus | Enemy Focus | Relevant remaining effects |
|---|---|---|---|---|---|
| Start | 30 / 32 / 36 / 26 / 24 | 24 / 20 / 10 | 3 / 3 / 3 / 3 / 3 | 3 / 3 / 3 | None |
| End round 1 | 22 / 20 / 36 / 26 / 24 | 0 / 20 / 10 | 3 / 2 / 3 / 2 / 2 | 3 / 2 / 2 | None on standing creatures |
| End round 2 | 22 / 20 / 36 / 26 / 24 | 0 / 0 / 10 | 3 / 1 / 3 / 2 / 2 | 3 / 3 / 2 | C's Resolve would expire after round 3; C exhausted |
| Victory, round 3 | 22 / 20 / 36 / 26 / 24 | 0 / 0 / 0 | 3 / 2 / 3 / 3 / 2 | 3 / 3 / 2 | All combat effects end with the encounter |

The player lost 20 total HP: 8 to T and 12 to B. Opponents lost 54: H24, C20, W10. No random rolls, regeneration, unexplained free action or unlisted damage occurs. Friendly activations are 5, 5 and 3 across the rounds; enemy activations are 3, 2 (one lost) and 1. Each technique stays within its Focus budget and next-ready-round rule.

This example demonstrates a consistent support sequence and enemy protection/control, not encounter difficulty, a solved optimal strategy, or long-term combat quality. A later opposing five-creature team must test whether the player can recover when its own planned sequence is interrupted.

[Status and Counterplay](Status%20and%20Counterplay.md) · [Encounter Design](Encounter%20Design.md)
