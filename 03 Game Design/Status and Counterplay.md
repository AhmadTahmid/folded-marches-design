---
id: design-status-counterplay
status: draft
origin: assistant mechanical proposals informed by user combat direction
---
# Status and counterplay

These proposed terms belong to [Tactical Combat](Tactical%20Combat.md). Every status has a visible source, removal class, expiry round and consequence. Its name must explain a repeatable rule; creatures can give that rule different visual expression.

## A small initial vocabulary

| Effect | Exact proposed consequence | Removal / response |
|---|---|---|
| Exposed | Armor reduced by 2, minimum zero | Basic Cleanse; Guard or seek rear protection against Melee |
| Silence | Cannot activate Accord techniques; Physical techniques, Strike, Guard and Move remain legal | Basic Cleanse; use the remaining action options |
| Disarm | Cannot use Strike or techniques tagged Attack; other techniques remain usable | Basic Cleanse; support or reposition |
| Root | Cannot change rows or participate in a row exchange; still attacks and casts | Basic Cleanse; Reach techniques and protection still work |
| Stagger | Lose the next unused activation this round; cannot apply after a creature has acted | Strong Cleanse before that activation, or prevent it with Steadfast |
| Scorch | Specified Resonance damage at round end, reduced by Ward and Barrier normally | Basic Cleanse before the tick; protection can absorb it |
| Barrier | Absorbs printed damage after Armor/Ward; no prevention of statuses | Enemy Strip, sufficient damage, or expiry |
| Steadfast | Rejects new Silence, Disarm, Root and Stagger; does not remove existing ones or reduce damage | Enemy Strip before applying control; attack or wait |
| Resolve | Rejects new Stagger through the end of the following round | Cannot be stripped, copied or extended; use damage or partial control |

**Default duration is through the end of the application round.** A card that lasts longer explicitly says, for example, “through end of next round.” At application the interface converts this to “expires after round 4.” An effect applied after its relevant action window may have little value; preview says so. Only Stagger categorically requires an unused activation.

Duplicate named effects do not stack their strength. Reapplication keeps the stronger value and later expiry. Separate Barriers do not add together: retain the larger remaining amount and later expiry. Persistent hazards are location rules, not unremovable debuffs attached to a creature; leaving the affected position is their counterplay.

## Preventing a lost turn from becoming permanent exclusion

Stagger interrupts one activation. When that activation is lost—or Strong Cleanse removes Stagger before it—grant Resolve through the end of the following round. Thus a round-2 Stagger cannot lead to another round-3 Stagger. Resolve does not make its owner immune to damage or partial restrictions.

A creature cannot refresh an existing Stagger, and a protected target is visibly ineligible. The rule applies equally to player creatures, ordinary enemies and bosses. A boss may have separately telegraphed anatomy or objectives; “boss” is not blanket immunity to everything the party learned. Any exception needs its own stated rule and counterplay.

Silence and Disarm together still leave Guard and Move; Root may remove movement, but Guard remains. Early opponents must not teach three simultaneous restrictions before teaching removal. Numerical tuning must check both consecutive lost activations and the frequency with which nominal choices are useless. The protection above solves one explicit lock, not all possible oppressive team compositions.

## Removal is different from protection

**Basic Cleanse** removes all effects labeled Basic from one ally. **Strong Cleanse** also removes Stagger. **Strip** removes all removable positive effects from one enemy, including Barrier and Steadfast, but never Resolve. All require an activation and the ability's printed Focus cost/cooldown. Removal causes no damage unless the technique explicitly includes damage.

Steadfast is proactive; Cleanse repairs an existing problem. A Barrier saves HP; it will not prevent the silence that stops a healer. These distinctions create readable combinations without an encyclopedic immunity chart. The initial proposal deliberately rejects statuses on application while Steadfast lasts; it does not queue suppressed debuffs that unexpectedly activate when protection expires.

For a multi-part technique, resolve printed steps in order. “Strip, then Silence” can remove Steadfast before attempting Silence. “Damage, then Silence” first resolves mitigation, then independently checks status protection. A zero-damage hit can apply Silence if its card does not require HP damage. No unstated “on hit” convention should decide a battle.

## Counterplay examples

- A support plans to Silence the Embermole. Activate the Doorling after the silence to cleanse it, use a Physical attack instead, or prevent the effect beforehand. These spend different actions and resources.
- A protected attacker is approaching its turn. Strip its Barrier and focus it, Stagger it if eligible, or Guard the threatened ally. Waiting out the Barrier is valid when immediate damage is unnecessary.
- A rival saves its cleanse until the player has committed a setup. The player can threaten a different target or use damage independent of the removed effect. Enemy counters follow the same timing rules and are shown in the intent queue.

Horror can make the source of an attack disturbing while preserving this grammar. A voice calling the keeper by an impossible name does not justify silently deleting a turn, changing a displayed probability, or violating Resolve. Any proposed rule-breaking story event needs an authored, discoverable rule of its own.

[Worked Battle](Worked%20Battle.md) · [Encounter Design](Encounter%20Design.md) · [Horror and Fourth Wall](../02%20Narrative/Horror%20and%20Fourth%20Wall.md)
