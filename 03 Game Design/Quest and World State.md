---
id: design-quest-world-state
status: draft
origin: assistant proposal
---
# Quest and world state

This is a writing contract for clear quest design, not an implementation specification. It helps future authors distinguish a story event, somebody's belief, and a fact the player has learned.

## Four separate records

The September [observer/sanctuary proposal](../02%20Narrative/The%20Observer%20and%20the%20Sanctuary.md) may add bounded in-game observations of interface use. That is a separately attributed fictional record, not permission to rewrite actual player choices or restored saves. [Tension, Stakes and Recovery](Tension%20Stakes%20and%20Recovery.md) requires explicit partial-success, separation and recovery states; a “failed” quest flag cannot stand for an unexplained vanished companion. Ordinary suspension, real-world absence and settings changes remain outside the story's consequence clock.

| Record | Meaning | Example |
|---|---|---|
| World condition | What has happened or currently exists | A bridge has been repaired |
| Character knowledge | What a particular person knows or believes | A courier thinks the repair used an unsafe accord |
| Player evidence | What the player has directly encountered | They have inspected the bridge's older foundation |
| Relationship commitment | What somebody has promised or is willing to do | A keeper has agreed to suspend work during migration |

No single “quest completed” label can replace all four. They may be described in prose while we are worldbuilding; eventual variable names can come later.

## An entry should answer

1. What invites the player into this situation?
2. What do the involved people and creatures want before the player arrives?
3. Which approaches are genuinely possible?
4. What changes because of the player's choice?
5. What happens if they leave, return, learn something early, or arrive after another event?
6. Which consequences are immediate, delayed, local, or regional?
7. Which claims are presented as uncertain, and which facts must stay consistent?

## Preserve alternatives without infinite branching

Choices can converge on a shared later event while changing its participants, available resources, or interpretation. A repaired bridge and a ferry cooperative may both allow the regional story to continue, but the community's work, travel time, and political dependency differ.

Do not advertise a choice and then erase all evidence of it. A modest recurring acknowledgment can carry more weight than a large branch that never affects anything again.

## Quest availability

Separate a quest's **invitation**, **active situation**, and **resolution opportunities**. Missing the first invitation need not remove the situation. Another person, a visible consequence, or an exploration clue can introduce it later.

Time-sensitive quests must communicate their urgency and what advances time. Merely spending a week exploring in a system without an established calendar should not unexpectedly kill an essential character.

## Re-entry and failure

Every major quest should name a return path after retreat or ordinary defeat. If an irreversible choice closes a route, describe the remaining narrative path. “Cannot complete this version” and “the game can no longer progress” are different states.

## Evidence integrity in horror

The player's current in-world journal may become unreliable as fiction. An optional stable recap or evidence viewer can still help players follow their observations. Whether the journal itself is allowed to change is an explicit design decision, not a license for arbitrary continuity changes.

Fourth-wall proposals must record the original text, altered text, trigger, duration, affected interface, and recovery. See [Horror and Fourth Wall](../02%20Narrative/Horror%20and%20Fourth%20Wall.md).

## Review questions

Read each quest once assuming the player distrusts Istravel, once assuming they distrust Orthe, and once assuming they care most about a creature rather than the city's policy. Look for a valid route through each perspective. Not all outcomes need be equally beneficial, but each should be intelligible.

[Quest Index](../02%20Narrative/Quest%20Index.md) · [Exploration and Progression](Exploration%20and%20Progression.md) · Quest Template (working-archive reference)
