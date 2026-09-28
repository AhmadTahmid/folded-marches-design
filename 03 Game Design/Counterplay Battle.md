---
id: design-counterplay-battle
status: draft
origin: assistant two-round paper exercise using first-region creature kits
---
# Counterplay battle — a plan interrupted

This **two-round snapshot** examines recovering a disrupted plan and changing targets. Both supervised teams use the identical benchmark in [First Region Creature Kits](First%20Region%20Creature%20Kits.md). The encounter remains unfinished; no optimal line or balance claim is established.

## Starting conditions and intentions

Prefix **P** means player; **O** means opponent. Suffixes: **T** Thimbleback, **B** Bellwether, **G** Glassgrazer, **E** Embermole, **D** Doorling. Both begin with T/B/G in front slots 1/2/3 and E/D in rear slots 1/2, using the complete unchanged kits. No talents, environmental modifiers, hidden traits, or human activation apply.

| Order in every audit row | T | B | G | E | D |
|---|---:|---:|---:|---:|---:|
| Starting HP, each side | 30 | 32 | 36 | 26 | 24 |
| Armor, each side | 2 | 0 | 2 | 0 | 0 |
| Ward, each side | 0 | 0 | 2 | 0 | 0 |
| Starting Focus, each side | 3 | 3 | 3 | 3 | 3 |

All techniques start ready. The player opens round 1; the opponent opens round 2. Each round's complete opponent intentions are shown beforehand and remain fixed.

**Shown fallback for every intention:** if the action is prevented by targeting, resources, cooldown, or control, use Strike against the lowest-numbered legal opposing front slot; Guard if that Strike is illegal. A rear Melee attacker therefore Guards. Stagger consumes the activation without a fallback. A target protected against Stagger or already Staggered is ineligible for Arresting Peal, so that intention uses its fallback. Steadfast rejecting Silence, Disarm, or Root after an otherwise legal activation does not grant a replacement action; the technique pays its normal Focus and cooldown. None is needed in this line; no hidden replacement action is permitted.

## Round 1 — rescue the interrupted attacker

Opponent order: **OD Screen OG → OB Arresting Peal PE → OE Furnace Breath PB → OG Fan Shove PT → OT Nut Pitch PD**. Removing the screen spends Doorling’s activation. Recovering the announced Stagger requires Glassgrazer’s distinct Strong Cleanse; Doorling’s Basic Cleanse cannot do that job.

| Step | Activation | Exact change |
|---|---|---|
| 1 | PB Calling Note on OG | PB Focus 3→2. OG gains Exposed: Armor 2→0 through round 1. |
| 2 | OD Borrowed Screen on OG | OD Focus 3→2. OG gains Barrier 8. |
| 3 | PD Pick the Latch on OG | PD Focus 3→2. OG's Barrier is removed. |
| 4 | OB Arresting Peal on PE | OB Focus 3→1. PE, still unused, is Staggered. |
| 5 | PG Settling Pulse on PE | PG Focus 3→1. Strong Cleanse removes Stagger; PE gains Resolve through round 2. Its activation remains available. |
| 6 | OE Furnace Breath on PB | OE Focus 3→2. 12−0 Ward = 12 damage; PB HP 32→20. |
| 7 | PE Furnace Breath on OG | PE Focus 3→2. 12−2 Ward = 10 damage; OG HP 36→26. |
| 8 | OG Fan Shove on PT | OG Focus 3→2. 10−2 Armor = 8 damage; PT HP 30→22. |
| 9 | PT Nut Pitch on OG | PT Focus 3→2. 8−0 Armor = 8 damage; OG HP 26→18. |
| 10 | OT Nut Pitch on PD | OT Focus 3→2. 8−0 Armor = 8 damage; PD HP 24→16. |

At round end, Exposed expires and OG returns to Armor 2. No damage-over-time or healing occurs. PE's Resolve remains. Both sides have consumed exactly five activations, and every creature is standing.

**Recovery costs an attack opportunity and two Focus.** Doorling's Basic Cleanse could not remove Stagger. Proactively protecting Embermole was another option, but would occupy the activation used for Calling Note. This is one legal response, not an exhaustive comparison.

## Round 2 — cleanse, interrupt, and change targets

Every standing creature regains 1 Focus, capped at 3. Player Focus becomes **3 / 3 / 2 / 3 / 3**; opponent Focus becomes **3 / 2 / 3 / 3 / 3**. Round-1 cooldown-2 techniques are still unavailable. Glassgrazer's rescue and the opposing Bellwether's peal are unavailable until round 4.

Opponent order: **OD Muffle PE → OB Horn Run PB → OT Burrow Grip PT → OE Warm Thread PG → OG Shed Screen OB**. PE's Resolve prevents Stagger, not Silence. The opponent's two restrictions therefore have different possible answers.

| Step | Activation | Exact change |
|---|---|---|
| 1 | OD Muffle on PE | OD Focus 3→2. PE gains Silence through round 2. |
| 2 | PD Unknot on PE | PD Focus 3→2. Basic Cleanse removes Silence; Resolve remains. |
| 3 | OB Horn Run on PB | OB Focus 2→1. 12−0 Armor = 12 damage; PB HP 20→8. |
| 4 | PB Arresting Peal on OT | PB Focus 3→1. OT, still unused, is Staggered. |
| 5 | OT loses its activation | Burrow Grip does not execute; no Focus or cooldown paid. OT gains Resolve through round 3. |
| 6 | PE Warm Thread on OB | PE Focus 3→2. 8−0 Ward = 8 damage; OB HP 32→24. |
| 7 | OE Warm Thread on PG | OE Focus 3→2. 8−2 Ward = 6 damage; PG HP 36→30. |
| 8 | PG Fan Shove on OB | PG Focus 2→1. 10−0 Armor = 10 damage; OB HP 24→14. |
| 9 | OG Shed Screen on OB | OG Focus 3→1. OB gains Barrier 10. |
| 10 | PT Nut Pitch on OG | PT Focus 3→2. 8−2 Armor = 6 damage; OG HP 18→12. |

At round end, OB's unused Barrier expires and PE's Resolve expires. OT retains Resolve through round 3. The player has five completed activations; the opponent has four completed actions and one activation lost to Stagger. No slot moved or creature was exhausted.

**A worse choice at the same cost:** Nut Pitch into lower-HP OB at step 10 loses all 8 damage to its Barrier. The remaining Barrier 2 expires; OG retains 18 HP instead of 12. Changing targets therefore gains 6 lasting damage for identical Focus and cooldown. This local conclusion depends on the displayed state and absence of end-round damage.

## HP, Focus, and cooldown audit

All value lists use **T / B / G / E / D**.

| Checkpoint | Player HP | Opponent HP | Player Focus | Opponent Focus |
|---|---|---|---|---|
| Start | 30 / 32 / 36 / 26 / 24 | 30 / 32 / 36 / 26 / 24 | 3 / 3 / 3 / 3 / 3 | 3 / 3 / 3 / 3 / 3 |
| End round 1 | 22 / 20 / 36 / 26 / 16 | 30 / 32 / 18 / 26 / 24 | 2 / 2 / 1 / 2 / 2 | 2 / 1 / 2 / 2 / 2 |
| End round 2 | 22 / 8 / 30 / 26 / 16 | 30 / 14 / 12 / 26 / 24 | 2 / 1 / 1 / 2 / 2 | 3 / 1 / 1 / 2 / 2 |

| Creature | Player: used techniques → next ready round | Opponent: used techniques → next ready round |
|---|---|---|
| T | Nut Pitch → 3, last used round 2 | Nut Pitch → 2; Burrow Grip remains ready because interrupted |
| B | Calling Note → 3; Arresting Peal → 5 | Arresting Peal → 4; Horn Run → 4 |
| G | Settling Pulse → 4; Fan Shove → 4 | Fan Shove → 3; Shed Screen → 4 |
| E | Furnace Breath → 3; Warm Thread → 3 | Furnace Breath → 3; Warm Thread → 3 |
| D | Pick the Latch → 3; Unknot → 4 | Borrowed Screen → 3; Muffle → 4 |

The player loses **28 HP in round 1 and 18 in round 2: 46 total**, leaving 102 of the initial 148. The opponent loses **18 and 24: 42 total**, leaving 106. Every lost point appears in the action tables. Neither team has won. If play continues, the player opens round 3, round-start Focus recovery occurs, and OT still cannot be Staggered that round. PB at 8 HP and PD at 16 face a real protection decision; two weakened opposing front creatures offer a competing opportunity.

Arithmetic consistency does not establish enjoyable pacing or balance; those need further encounter design and eventually playtesting.

[Worked Battle](Worked%20Battle.md) · [First Region Creature Kits](First%20Region%20Creature%20Kits.md) · [Status and Counterplay](Status%20and%20Counterplay.md)
