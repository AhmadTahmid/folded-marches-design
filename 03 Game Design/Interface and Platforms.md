---
id: design-interface-platforms
status: draft
origin: assistant proposal
---
# Interface and platforms

The user selected the browser/WebGL foundation for development (D-035), with Steam, Google Play and Apple App Store as eventual targets. This page records experience requirements and unresolved constraints; it does not establish that a specific rendering pipeline, package or world scale meets them.

## Shared experience

Exploration, companion selection, readable encounters, dialogue choices, maps, and journals should remain complete on each intended platform. Platform differences should be handled deliberately rather than assuming a desktop interface can be shrunk.

## Controls to compare later

| Activity | PC proposal | Touch proposal | Open question |
|---|---|---|---|
| Travel | Keyboard/controller movement with camera control | Virtual movement plus restrained camera gestures | Free camera, constrained orbit, or authored camera zones? |
| Creature command | Shortcuts and contextual menu | Large contextual choices with confirmation for costly actions | How many commands can be readable at once? |
| Encounter | Pointer/controller selection and clear previews | Tap selection, preview, then confirm | How clearly can five active creatures, positioning, and enemy intentions fit on each display? |
| Journal | Search, links, map and evidence tabs | Large type and focused panels | Can a long investigation be followed in short sessions? |

No minimum device, orientation, frame-rate target, or controller policy is approved yet. These are requirements to choose before the art pipeline is locked.

## Five companions at once

The five-active maximum, turn-based mode, positioning, and coordination are selected direction. The proposed interface shows each creature's row, health, Focus, whether it has acted, and urgent conditions. Selecting one opens its techniques; it need not display twenty technique buttons at once. Enemy intentions and fallback targets remain inspectable alongside the active choice.

**Browser 0.3 feedback, 2026-09-27:** the user found the opening combatants overwhelming and the interface cluttered. [Engagement Reset](../04%20Production/Engagement%20Reset.md) proposes beginning with one partner, then two, and growing toward five later. Its default view prioritizes the current actor, target, enemy intention and action consequence. Detailed calculations and complete status history remain available through inspection and an optional log; legal learned actions must not be silently hidden to force a tutorial response. This is a design proposal, not a tested replacement layout.

D-039 requires creatures visibly facing each other in a battle scene, with a command menu and clear animated move outcomes. Cards and logs support this view; they do not replace the visible encounter. Art and action effects should communicate which creature acts, which target is affected and what changed.

Previews explain damage, protection, legal targets, and resource costs before confirmation. Effects show their exact expiry round and techniques their next usable round. A row exchange previews both partners' resulting vulnerability. These requirements follow [Tactical Combat](Tactical%20Combat.md); whether the proposed layout reads comfortably on a phone still needs testing.

## Legibility and access

**Dialogue delivery (D-040):** use short beats, one at a time, with the actual speaker's name and portrait. Distinguish narrated action from speech and avoid attributing another character's words to the person who opened the conversation. Advance and skip must be explicit; skipping text reveals any response choices without selecting one. A held advance key must not commit a response. Longer reference material belongs in an optional journal, not a mandatory wall of text. Portrait designs and exact word limits remain open.

The user subsequently rejected obscure dialogue and questioned the visible “Narration” label. Show ordinary stage actions through the scene; keep author directions offscreen. Where a caption or accessible description is necessary, identify the event plainly without inventing a narrator character. [Engagement Reset](../04%20Production/Engagement%20Reset.md#speech-samples-not-lore-delivery) supplies short, concrete Ada/Pell/Clatter scene examples. This does not prohibit rich prose in the private wiki or establish a speaking, omniscient narrator in the fiction.

Use adjustable text size, distinguish important information by more than color alone, provide subtitles for meaningful audio, and keep interaction targets large enough for touch. Offer reduction of flashing, intense distortion, or camera effects where those are proposed. These features protect the intended experience for players who otherwise cannot read its clues.

## Session continuity

The narrative should support returning after days away through a useful recap of observed facts, current invitations, and unresolved questions. Mobile suspension and interrupted sessions need explicit future testing. They are not narrative events and should not be mistaken for fourth-wall fiction.

## Fourth-wall design contract

The September source includes false cooldowns, targeting inversions, fake system reports, process inspection and pause threats. These are **unselected prompts**, not accepted requirements. [The Observer and the Sanctuary](../02%20Narrative/The%20Observer%20and%20the%20Sanctuary.md) compares fictional records, accurate in-game observation and visible menu intrusion while keeping tactical values, selection/cancel, pause, exit and saved progress dependable. [Tension, Stakes and Recovery](Tension%20Stakes%20and%20Recovery.md) separates anxiety about time loss from enjoyable mastery. Later adoption of any stronger illusion would require its own concrete design, rather than inference from the pasted argument.

The current safest creative starting point is a fictional journal, bestiary, route annotation, or in-game character addressing the act of choosing. It can use actions observed inside the game. It does not need real names, desktop files, microphone input, or account data to become unsettling.

Save integrity, settings, exit controls, and accessibility controls remain dependable in the proposed baseline. A fictional corrupted entry is presentation, not destruction of actual player progress. If stronger illusions are later proposed, they need their own explicit experience design and recovery plan.

An option to reduce interface deception could preserve the scene's dialogue and evidence while displaying a stable explanatory recap. Whether to expose this before play or through a broad effects preference is undecided.

## Documentation boundary

[Horror and Fourth Wall](../02%20Narrative/Horror%20and%20Fourth%20Wall.md) owns narrative effects and their escalation. This page owns dependable controls and player access. Production pages own engine support evidence and technical uncertainties.

[Game Direction](Game%20Direction.md) · [Art and Sound Direction](Art%20and%20Sound%20Direction.md) · Production Overview (working-archive reference)
