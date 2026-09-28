---
id: production-first-five-hours-handoff
status: reference
origin: implementation handoff for the user's authored opening package, D-065
updated: 2026-09-28
---
# Build the opening from one source

The user owns implementation. This packet supplies the first day in Rocca Selva, its Bell Road outing, either afternoon booking and the changed evening return. It is an authored draft, not an inspected game build. Follow [First Five Hours](../02%20Narrative/First%20Five%20Hours.md) for opening continuity and [Design Status](../00%20Foundation/Design%20Status%20v0.1.md) for established direction. The older campaign remains the wider story. A beautiful reference town is not the layout for this one.

## Receive these files together

| Read order | Source | What the builder obtains |
|---|---|---|
| 1 | [First Five Hours](../02%20Narrative/First%20Five%20Hours.md) | The protagonist's want, exact commission, authority and identifier directory |
| 2 | [Opening Day](../02%20Narrative/Opening%20Day%20Script.md) | Main dialogue, staging, actions, objective text, payment and evening variants |
| 3 | [Two Bookings](../02%20Narrative/Two%20Bookings%20Script.md) | Both complete afternoon routes, commitment, physical interactions and withdrawal |
| 4 | [Detailed Atlas](../01%20World/Rocca%20Selva%20Detailed%20Atlas.md) | Coordinates, contours, paths, exterior stations, twelve interiors and event placement |
| 5 | [Residents and Side Stories](../02%20Narrative/Rocca%20Residents%20and%20Side%20Stories.md) | Recurring wants, locations, six scripted local stories, cross-conversations and performance |
| 6 | [Creatures and Commerce](../03%20Game%20Design/Opening%20Creatures%20and%20Commerce.md) | Individuals, ownership, invitations, shop stock, prices, services and use scenes |
| 7 | [Opening Battles](../03%20Game%20Design/Opening%20Battle%20Encounters.md) | Four optional encounter placements, reusable practice fixtures and the wild cache defender |
| 8 | [Progression and State](../03%20Game%20Design/Opening%20Progression%20and%20State.md) | Pacing hypotheses, journal transitions, receipts, order and recovery cases |

Also receive the linked creature species pages, [First Region Creature Kits](../03%20Game%20Design/First%20Region%20Creature%20Kits.md), [Tactical Combat](../03%20Game%20Design/Tactical%20Combat.md), [Status and Counterplay](../03%20Game%20Design/Status%20and%20Counterplay.md) and [Combat Learning Sequence](../03%20Game%20Design/Combat%20Learning%20Sequence.md) if implementing encounters. Do not substitute the alternative identity cards or shared-action study for these baseline rules. Five active companions remains a ceiling, not a required opening team.

For integration, the wiki must travel with the user's actual current source, assets, launch command and save-format information. A public repository URL cannot provide an unpublished runtime. The receiver reports the wiki revision and files actually read, plus missing source, before claiming integration. Prepared prompts are not dispatched work.

## Buildable content groups

These are dependencies within one connected opening, not instructions to create eight unrelated demos. A builder may work in any order that preserves them.

1. **Place and passage.** Lay out the nine districts, stairs and carrying incline, then the two road corridors. Preserve visible destination landmarks and non-precision alternatives. Full wagons remain in the lower yard/road; six-footed Cragmantle has room to work. The protected water intake stays separate from waste drainage. Entering and leaving a room returns to its actual threshold.
2. **Work and family.** Implement F5-M01–04 and M06 as the connected core. The player seeks work before being hired, can approach Pell directly, reviews actual terms, records three findings and reports at the red-roofed exchange. Immediate objectives always name an action and a place. Ada's arrangement and her family's dialogue follow actual events.
3. **One afternoon commitment.** Implement both choices under F5-M05, with one active booking per save/window. Orchard equipment has two verified sight lines. The wagon has exactly three persistent loads: tool barrel, jar crate and cloth bale. Retreat retains work; explicit cancellation ends the booking without undoing the base survey. No hidden timer makes the choice.
4. **People and interiors.** Place the recurring residents according to the phase table. Implement F5-S01–06 with their two approaches, refusals and changed spaces. Accepted unfinished contributions survive phase changes. The roof gallery, schoolroom, workshop, bakery and warm rooms are destinations with activities, not locked facades.
5. **Companions and wonders.** Use the RS-C individual records, not only species names. Clatter and the other invitations can be declined. The borrowed Bellwether returns after practice. Orla's Cragmantle and Eren's Sailrook keep their actual keepers. The wild cache defender is distinct from the recruitable village Thimbleback. Show habitual behavior before recruitment text.
6. **Markets and small pleasures.** Six shop records share real stock with any alternate attendant. Twenty-two goods/services use their posted prices and effects. Clothes are presets with no hidden stat benefit. Buying nothing remains a complete route. Quest tools, emergency rest and necessary observation access cannot become purchases.
7. **Optional resistance.** First duel follows the early companion walk at Pass House. The flag exercise and Rovan's comparison can wait. The cache defender guards a lookout spur, not the road required for wages. Intent, cost and target are readable before committing; animation does not alter the deterministic result.
8. **A changed return.** Resume the actual local arrangements, Pavo's outcome, Vela's chosen credit and the household's already-recorded contribution. Let the player watch or participate in Miret's performance, share something actually seen and choose a next destination. No generic congratulation should claim a withdrawn booking succeeded.

## Scene and asset boundaries

| Layer | Authored requirements | Builder's freedom |
|---|---|---|
| Scene data | Stable IDs, named speakers, conditions, choices, objectives and acknowledgments from the scripts | Internal data format, localization keys and dialogue tooling |
| World | District/route connections, thresholds, useful sight lines, public/owned spaces and safe alternatives | Mesh construction, exact terrain fit and camera compositions that preserve those relationships |
| Humans | Established identities and pronouns, work clothing, occupied hands, meaningful poses and scene props | Final sprite treatment and reusable animation method |
| Creatures | Species anatomy, individual ownership, characteristic actions, invitations and physical contact | Painted, layered, generated or assisted sprite production; no mandatory fixed frame count or resolution |
| Interactions | Explicit move/place/inspect/record/ask/decline verbs and stated outcomes | Input mapping and accessible equivalents with the same outcome |
| State | One-time receipts, known/unknown evidence, actual actor and cargo locations, persisted branch choice | Storage architecture and save migration after inspecting the user's runtime |
| Sound and music | Space for ordinary work, comic pauses, creature tells and quiet views | Later sound direction; this writing pass commissions no new audio |

Sprite humans and creatures inhabit the 3D WebGL2 world. Keep visible feet, hauling lines, perches and carried objects in contact with their scene. A proxy must be named as a proxy; availability cannot rewrite a creature or resident. Preserve editable art and motion inputs. The wiki does not claim final art, runtime performance or a fixed production cost.

## Concrete review routes

These are specified acceptance walks for the later build, **not tests already run**.

| Walk | Expected result |
|---|---|
| Skip Tavio, decline every invitation, buy nothing | Pell's direct introduction works; all observations and either booking are achievable with public paths/tools/people; first practice offers a disclosed loan |
| Skip dialogue | Job card still says three observations, exchange destination, 36 total/12 advance, covered necessities and payment for unsafe findings |
| Get S01's schoolroom result before terms | Ada is reachable at the market-side door; she does not reset to the sagging stand or request the table again |
| Inspect tap without inspecting leaves | Report says only observed flow/access; it does not invent the maintenance note |
| Visit village between observations | Pell's old station directs to the exchange; report data survives; ordinary exploration does not expire the commission |
| Attempt both afternoon payments | One committed branch owns the window; the second booking cannot start or pay |
| Release the wagon without securing it | The same tool barrel reaches the catch apron; secure/recover it, deliver all three loads once, receive the single posted wage |
| Withdraw from either booking | No extra wage or unearned field contact; base reference and family support remain; evening lines name the actual result |
| Follow the representative return route | S04 remains available for the returning player; household stories acknowledge actual encounters; Miret's staging follows S05 |
| Spend the entire personal purse | Main observations, recovery and walking onward still work; no hidden required purchase |
| Decline or revisit a creature | Individual location and invitation state persist; no duplicate animal or automatic recruitment; owned visitors remain owned |
| Save/quit during a carried prop or conversation | Resume with one prop, one location and no repeated receipt; canceled dialogue is not a new reward trigger |

Then ask a newcomer where they want to go, what Pell is paying for, which person they want to meet again and whether the return feels different. Record actual dull or confusing moments and actual session duration. A clean state graph and a pleasing screenshot answer different questions from enjoyable play.

## Ready-to-adapt assignment

> Read the First Five Hours packet at the supplied wiki revision and name the source files received. I am supplying my current game source separately. Build the connected authored Rocca opening in that project, preserving useful existing movement and rendering. Follow Opening Day, the atlas, residents, creatures/commerce, battles and progression owners. Implement both afternoon choices with one commitment per run. Keep the protagonist's motive, direct Pell introduction, voluntary companionship, prices and free necessary routes explicit. Treat new fiction as the current draft, not an invitation to copy a reference town or silently replace the story. Return editable source, launch instructions, the changed file list, intentional departures, remaining proxies and evidence from the review routes. Report what you actually tested; do not claim the writing is fun or lasts five hours without player evidence.

The user can scope that prompt to one connected content group while retaining the full packet as context. Sending a smaller assignment does not delete the remainder of the designed opening. See [Build from the Wiki](Build%20from%20the%20Wiki.md) for the browser handoff and return process.
