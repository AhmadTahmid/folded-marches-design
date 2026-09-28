---
id: design-tactical-combat
status: draft
origin: user direction with assistant mechanical proposals
---
# Tactical combat

**Established direction, 2026-09-26:** strategic, technical turn-based combat; up to five friendly creatures active together; positioning and coordinated abilities; Dota 2 is a major mechanical inspiration. Numerical rules below are a coherent paper proposal, not adopted balance or tested gameplay.

The intended satisfaction is seeing an opponent's plan, creating a brief opening, and spending the right resources to exploit it. A familiar companion remains valuable because the player learns its possibilities. More powerful attacks alone should not solve every encounter.

**Presentation correction, D-039:** the user wants opposing creatures visibly facing each other, a Dragon Quest/Evertale-like command menu, and animated move effects. Creature cards and the combat log are supporting information, not the primary depiction of the battle. This preserves the five-active strategic direction; it does not adopt those reference games' exact rules. See Opening and Battle Presentation (working-archive reference). Sound effects remain for a later pass.

## One readable turn structure

**September comparison:** [Tension, Stakes and Recovery](Tension%20Stakes%20and%20Recovery.md) develops clutch objectives and consequences without selecting real-time combat. [Resonance, Fusion and Last Resorts](Resonance%20Fusion%20and%20Last%20Resorts.md) compares paired actions, forms, calls for help and phase changes. Those proposals do not alter the baseline turn rules below: no sixth friendly action/body, no ordinary reserve substitution, no numerical fusion/HP contract yet adopted. Exceptional encounters must state their departures explicitly before play.

1. **Prepare the round.** From round 2 onward, standing creatures recover 1 Focus, up to 3. Refresh their activation markers. Show the enemy's ordered intentions, targets, and fallback rules. Each technique displays its next usable round.
2. **Alternate sides.** On a friendly turn, choose any friendly creature that has not activated this round. It performs one action. The enemy then resolves its next listed creature. A staggered creature consumes its activation without acting. Defeated creatures are removed from the queue.
3. **Finish the round.** If one side has no remaining activations, the other finishes its unused ones. Resolve simultaneous end-round damage, then simultaneous end-round healing on survivors, then expire effects with that round's label. No healing revives a defeated creature unless explicitly designated revival.

Ordinary encounters give the player the first activation in round 1; the opening side alternates each round. An encounter may visibly begin with enemy initiative, but never conceal that fact behind an invisible speed roll. No speed statistic grants extra turns in this baseline. Acting now versus retaining a cleanser or finisher is already a timing decision.

There are at most **five friendly activation decisions per round**, regardless of animation count. The protagonist does not add a sixth combat turn. Summoned objects are effects of their summoner, with no additional creature slot or separate activation; controllable summons would require a later explicit rule that still respects the five-body cap. A larger collection lives outside this battle roster. Mid-battle reserve replacements are not included in this draft.

No automatic counterattack or reaction grants a new action. A technique can announce one automatic protection or retaliation with a fixed trigger and value; it cannot recursively trigger another retaliation. This keeps five companions from becoming twenty menus.

## Formation with consequences

Five positions comprise three **front** slots and two **rear** slots. Empty positions are allowed. This is a compact formation, not a movement grid.

| Rule | Tactical consequence |
|---|---|
| Melee attacks require the attacker in front; they target enemy front creatures while any stand | Durable partners screen vulnerable allies |
| Reach techniques can target either row unless their card says otherwise | A rear specialist remains a real threat |
| Once the opposing front is empty, Melee can target the rear | Removing the final defender opens a concrete window |
| Move exchanges rows with a willing ally or enters an empty slot; it consumes only the mover's activation | Save a vulnerable partner at an offensive cost; the exchanged ally gains no new activation |
| Affected creatures cannot participate in a row exchange while Rooted | Movement control has a clear purpose |

Rows grant no hidden damage bonus. A technique states whether it targets a creature or a position: moving dodges a position-targeted attack but not a creature-targeted one that can still legally reach it. Environmental objectives, a sheltered position, or a flooded row may alter a particular battle; display their rules before commitment.

## The command panel

Each creature equips **four techniques**, plus common **Strike**, **Guard**, and **Move** actions. Techniques carry `Physical` or `Accord` tags; these describe how they are performed. Separately they specify damage as `Impact` or `Resonance`, and delivery as `Melee` or `Reach`. A physical-looking attack need not secretly follow the rules of a spell.

`Attack` is a separate, explicit technique tag used by Disarm. The direct damage techniques in the [five benchmark kits](First%20Region%20Creature%20Kits.md), including Furnace Breath and Warm Thread, carry it whether their activation is Physical or Accord. Do not infer it merely because an effect causes damage: a future hazard or retaliation must state its own interaction. The worked example's tags follow the same cards.

- **Strike:** the species' modest, Focus-free Physical attack, with its own displayed delivery and Impact damage. A rear specialist may have a Reach Strike; a rear-positioned Melee specialist must move or use a Reach technique.
- **Guard:** no Focus cost; grants the user an 8-point removable Barrier through the end of the current round. It is meaningful before damage arrives, and replaces that activation's attack.
- **Techniques:** usually cost 1–2 Focus. Creatures start a fresh battle with 3. Spending the last point is allowed; negative Focus is not. Costs are paid on successful activation, even if the target's protection negates the result.

Using a cooldown-2 technique in round 1 makes it available in round 3; cooldown-3 makes it available in round 4. The interface says **“Ready round 3”**, avoiding ambiguity about whose turn decrements a number. Cooldown-1 permits use in the following round. A technique prevented before execution consumes neither Focus nor cooldown, although the creature's activation is spent if it is Staggered.

Friendly players can revise an action until confirming it. Afterwards there is no retargeting or free replacement action. Invalid enemy intentions use a shown fallback: target a named legal substitute, use Strike against the lowest-numbered legal front slot, or Guard if none exists. Silenced enemies cannot secretly replace a cancelled spell with their strongest unrelated technique. Inspection previews the currently applicable fallback.

## Damage players can calculate

Use small, deterministic integers initially. **Impact** subtracts Armor; **Resonance** subtracts Ward. Damage cannot fall below zero. `Exposed` reduces Armor by 2, to a minimum of zero. A Barrier absorbs the remaining damage before HP; excess proceeds to HP. Healing has a printed value capped by maximum HP. No default random critical hits, accuracy rolls, damage ranges, or hidden level multipliers.

Example: 12 Impact against Armor 3 produces 9 damage; a 5-point Barrier absorbs 5; HP falls by 4. Neither Armor nor Barrier prevents Silence. Where a future technique deliberately uses chance, show its probability and separate guaranteed effects from contingent ones; the baseline worked battle uses no rolls.

At zero HP a creature is exhausted and loses remaining activations. Ordinary defeat does not establish permanent companion death. Combat objectives, withdrawal and recovery belong to [Encounter Design](Encounter%20Design.md).

## Depth without twenty prerequisite lessons

**Opening review, 2026-09-27:** the user found the full-roster browser trial overwhelming and pressed buttons without reading. [Engagement Reset](../04%20Production/Engagement%20Reset.md) proposes one readable 1v1, then an earned optional 2v2, before later team growth. This preserves the maximum of five active friendly creatures; the maximum was never a requirement for the first battle. The exact onboarding sequence and practice kits remain proposals. Keep the full-roster encounter as an advanced mechanical benchmark rather than assuming it is a good introduction.

The earlier teaching proposal began with Strike/Guard, followed by setup/payoff, protection, then disable/rescue. The current [Engagement Reset](../04%20Production/Engagement%20Reset.md) instead proposes testing Strike against one characterful interruption first, with the simpler Guard lesson retained as a fallback comparison. Neither teaching order is adopted. Introduce later layers when they create a clear, useful decision. Later teams combine frontline pressure, rear access, cleansing, resource denial and timed protection. A rare creature offers a different problem-solving shape; rarity is not a guaranteed statistical upgrade.

On phones, five portrait cards show HP, Focus, acted state and the two most urgent effects; tapping opens the complete effect list. Enemy intent uses a target portrait plus action verb. Preview shows resulting damage and why: **“12 − 2 Armor = 10; Barrier absorbs 6; 4 HP.”** Keyboard shortcuts and larger layouts can accelerate this same ruleset on PC. Accessibility and input claims remain design intentions until prototyped.

Future playtests must establish whether alternating activations, short status windows and five active partners feel satisfying. Paper arithmetic establishes only that this draft can be followed consistently. If a routine battle demands repeated inspection of ten cards, simplify its information burden before adding another mechanic.

[Status and Counterplay](Status%20and%20Counterplay.md) · [Worked Battle](Worked%20Battle.md) · Dota Combat Reference (working-archive reference) · [Bestiary](../01%20World/Bestiary.md)
