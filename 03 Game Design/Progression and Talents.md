---
id: design-progression-talents
status: draft
origin: assistant proposal implementing user-selected progression direction
---
# Progression and talents

**v0.1 reading:** [Adventure Rules v0.1](Adventure%20Rules%20v0.1.md) selects one working interpretation for this edition. The comparisons below remain useful alternatives; they are not all simultaneous requirements. User-selected turn-based combat and the five-active ceiling still govern.

**Established direction:** levels and growth remain part of the RPG; repetitive grinding should contribute much less than exploration, learning, and good decisions. Monster talent choices are a candidate the user wants explored, not a finalized system. All numbers and detailed rules below are proposals.

## Three kinds of progress

| Progress | What improves | What the player can feel |
|---|---|---|
| Creature level | A restrained amount of health, offense, and defense; access to techniques and candidate talent milestones | A companion survives something difficult and has a new way to contribute |
| Build knowledge | Understanding roles, targeting, resource windows, counters, and team combinations | The same roster beats a situation that defeated a careless approach |
| World knowledge | Habitats, conditions, routes, useful field abilities, local relationships | A journey becomes richer because the player understands the place |

These should reinforce one another. Level gains have visible value, but a moderate level advantage should not erase positioning, protection, disabling, and resource management. A rare creature is an interesting opportunity rather than a universally stronger replacement for common partners.

## Where experience comes from

Reward meaningful creature encounters, new discoveries, difficult traversal, resolved quests, and first demonstrations of field knowledge. One event awards its discovery reward once, with a clear journal record. Watching the same animal perform the same routine indefinitely does not generate an experience economy.

Ordinary battles still award experience. Repeat encounters can be enjoyable practice, but easy repetition should not be the expected bridge between story chapters. Optional rematches can offer different team compositions, challenge rules, and cosmetic or technique rewards. A player who enjoys battle can continue battling; a player who explores and follows quests should also stay ready for ordinary progression.

Defeat does not confiscate accumulated experience. Learning a difficult encounter should leave the player with knowledge, readable feedback, and a practical return route rather than an obligation to rebuild lost progress.

## Share growth without erasing individuals

The proposed five-member combat team shares encounter experience without requiring every creature to land a hit. A recruited partner resting elsewhere can benefit from a **training floor** unlocked by the player's regional progress. This is a catch-up mechanism, not a new daily chore or currency sink.

Illustration only: the established team is around level 18 and a newly recruited creature is level 6. At a safe rest, an already-earned regional training floor could bring it to level 16, allowing it to join the next journey immediately. The remaining growth, techniques, and chosen talents give room to develop it. The exact level curve and floor need later testing; there is no approved final level cap.

Training floors come from durable progress, not the highest creature temporarily placed in a team. Borrowing, recruiting, or otherwise obtaining one powerful creature cannot recursively raise the entire roster. Lowering a team member's level for a challenge does not undo earned progress.

Named relationships, appearances, field habits, and personal history remain individual. Catch-up does not make every creature feel as if it has already shared the protagonist's adventures.

## Habitats retain identity

The initial proposal uses identifiable regional threat bands and a few specifically authored exceptions. Familiar areas should visibly become easier as the party grows. Avoid scaling every creature to the player's exact level, which would erase much of the felt benefit of progress.

Entering a difficult area early is possible when its danger is communicated. Knowledge, escape options, preparation, and a well-composed team can help. A distant creature's grandeur does not guarantee that it is intended as a fight at the player's current stage.

Difficulty settings can adjust damage, resources, and the amount of information presented without secretly changing the meanings of silence, roots, cleansing, or protection. The base rules should remain learnable.

## A small talent tree with meaningful forks

Start by comparing **three binary choices per species** at milestones such as levels 6, 12, and 18. These levels illustrate spacing, not a selected total campaign length. Six authored options create eight possible combinations before technique selection and team composition; that is already a substantial design space.

The shared structure makes trees readable. The choices themselves should express a species' body and behavior. A broad, ornate tree full of minor percentage increases would demand more reading while doing little for tactical identity.

Every fork needs a genuine cost or opportunity cost. A defensive option should sometimes be preferable to a damage option because of the encounter, not because the player has misread the numbers. Do not promise all combinations will be equally good in every situation; aim for several intelligible uses and no deliberate trap picks.

## Bellwether example — candidate specialization

These are illustrative extensions of the rules in [Tactical Combat](Tactical%20Combat.md) and [Status and Counterplay](Status%20and%20Counterplay.md). They are **not equipped in the baseline Worked Battle**. The exact technique kit owns targeting, base costs, and cooldowns.

| Milestone | Choice A | Choice B | Decision it creates |
|---|---|---|---|
| First fork | **Firm Footing:** self-Guard grants a 10-point Barrier instead of the baseline 8 | **Sheltering Call:** Guard may instead place a 6-point Barrier on one ally, costing 1 Focus and granting none to itself | Efficient self-protection or flexible rescue at a resource cost |
| Second fork | **Cracking Note:** Calling Note's Exposed penalty becomes 3 Armor rather than 2 on its existing target | **Chorus of Faults:** Calling Note may instead apply the baseline Exposed to two eligible front-row enemies for 2 Focus, with cooldown 3 | Focus one target or prepare a wider coordinated attack |
| Third fork | **Long Breath:** after using Guard, recover one additional Focus at the next round's start, still respecting the cap | **Measured Interruption:** the kit's hard-interrupt technique costs one less Focus, but takes one additional round to become available again | Sustainable protection or a cheaper, less frequent control window |

The alternate action versions are explicit choices, not automatic extra casts. All effects obey the common expiry and non-stacking rules. The broad Exposed option replaces Calling Note's single-target version for that activation. Both versions share one cooldown: using either prevents the other until the chosen version's next-ready round. No talent creates an extra full activation, bypasses a target's control protection, or raises the five-active-creature limit.

For the illustrative three-round cooldown, use the combat page's notation: if used in round 2, next ready in round 5. The UI should show that exact return round. A smaller Focus cost may be valuable even with a longer cooldown; whether that tradeoff is sufficient is a balance question to test later.

## Learning, equipping, and changing one's mind

The working proposal is four equipped techniques plus common Strike, Guard, and Move actions. Learning a new technique adds it to a permanent library; it need not delete an old favorite. Field capabilities such as climbing, carrying, surveying, or swimming do not consume these four combat slots.

Change equipped techniques and selected talents freely at safe rest points outside an active encounter or committed expedition segment. The interface previews what changes. Respecialization does not heal damage, reset world consequences, or recover spent expedition resources. The aim is to encourage experimentation, not build an infinite recovery loop.

Show recommended starter configurations with a one-sentence explanation. Advanced players can inspect complete costs, durations, targeting, and interactions. Tooltips should explain why a combination works. A new player should not need an external guide to discover that one effect removes a protective buff before another can disable a target.

## Frictions to remove from this game

This is a design list, not a claim that every named comparison game has every problem.

- Repeated trivial fights solely to bring a newly recruited partner into use.
- Mandatory breeding or repeated capture for invisible superior combat-stat rolls. Baseline species growth should be legible; individual cosmetic and behavioral variation can remain.
- Relearning a forgotten technique through a scarce consumable after every experiment.
- Rotating an unwanted creature into the combat team solely to pass a traversal check.
- Long recovery trips after ordinary practice encounters.
- Daily-login growth gates, real-calendar rare encounters, and unbounded reroll hunting.
- Inventory assembly or compulsory meals before every worthwhile battle.

Exact rewards, recovery, difficulty, and training-floor values remain proposals. Cooking, crafting, and base building are currently optional and deferred; progression must work without them.

## What we should evaluate next on paper

Take the same five creatures through the [Worked Battle](Worked%20Battle.md) with a beginner configuration, a coordinated configuration, and an imperfect but understandable configuration. First compare decisions and mistakes at equal level; then introduce a modest level difference. The lesson should remain visible when raw numbers change.

For later playable validation, record encounter length, meaningful decisions, recovery time, new-recruit readiness, whether players can explain a loss, and how often they feel obliged to repeat easy content. None of those experiential claims is proven by these written rules.

[Game Direction](Game%20Direction.md) · [Rare Encounters](Rare%20Encounters.md) · [Feature Priorities](Feature%20Priorities.md)
