---
id: design-opening-progression-state
status: draft
origin: implementation-facing writing contract for the authored first-five-hours package
updated: 2026-09-28
---
# Opening progression, pacing and state

This page connects the [First Five Hours](../02%20Narrative/First%20Five%20Hours.md) script, [detailed atlas](../01%20World/Rocca%20Selva%20Detailed%20Atlas.md), [residents](../02%20Narrative/Rocca%20Residents%20and%20Side%20Stories.md) and [creatures/commerce](Opening%20Creatures%20and%20Commerce.md). It describes authored behavior for the user's implementation; it is not a running quest engine or measured playtest. All new values remain draft.

## A representative five-hour route

The following is an **authoring budget of 300 minutes**, not a clock imposed on the player or a claim of measured duration. Times include looking, talking, moving, choosing, trying an interaction and enjoying its consequence; no segment consists of waiting for an unlock. Players who already know the answers, skip optional talk or decline local stories will finish much faster. The package should be built and reviewed for whether each interval contains enough interest; do not slow walking, pad dialogue or add repeat battles to hit a number.

| Elapsed target | What the player does | Why this moment earns its place | Source / milestone |
|---|---|---|---|
| 0–10 | Wake, negotiate the shirt, meet the family in action, leave with lunch | Know the personal ambition and concrete first destination before leaving home | F5-M01A |
| 10–27 | Discover the arriving wagon, owned Cragmantle, smith/shop thresholds and market smells | See that goods, travelers and remarkable creatures have reasons to be here | F5-M01B, RS-C06, RS-E arrival |
| 27–45 | Help or watch Clatter, try the walk and optional first duel at Pass House | Recognize a partner's behavior, then enjoy a characteristic action; loan if no recruit | F5-M01C / RS-C01, F5-B01 |
| 45–55 | Discuss the finite job and actual terms with Pell and Ada; take the advance | Have a goal, route, reason and known reward | F5-M02, Contract Accepted |
| 55–88 | Follow the table story and test Bera's carriage by either approach | Learn the inhabited shortcuts while Ada, Lina and Bera pursue their own work | F5-S01, S02 |
| 88–108 | Find Neri's missing purchase; meet the unattached Doorling | Comedy reveals a private preference and a second kind of partnership | F5-S03 / RS-C04 |
| 108–133 | Follow the Thimbleback cache, record the cistern, explore the waterkeeper's room and upper view | Move between discovery, a real commission observation and an inhabited place | RS-C02, F5-M03A, RS-I04 |
| 133–155 | Walk the two Bell Road bends, meet Vela, choose footing approach and investigate the optional lookout warning | Earn an outward view and exercise judgment; observe, pass peacefully or challenge the cache defender | F5-M03B–C, F5-B04 / RS-C10 |
| 155–170 | Deliver the report; see Asta use it; inspect the reference and optional keeper exercise | Finish a real job, get paid, see what better practice can offer | F5-M04, Survey Settled |
| 170–210 | Choose one complete afternoon: canopy expedition or wagon route | Experience a distinct adventure with an honest opportunity cost | F5-M05, [Two Bookings](../02%20Narrative/Two%20Bookings%20Script.md) |
| 210–235 | Return through changed activity; resolve the warm-room story and meet its adult Embermole | Returning is discovery; local lives progressed and a creature has preferences | F5-M06A, S04 / RS-C03 |
| 235–265 | Rehearse around a Kitefin's shade; discover the roof room and Ada's old picture | Aerial wonder, a physical place with history, and a parent with her own desires | S05, S06 / RS-C05 |
| 265–280 | Visit the pass-house wing-check, spend a chosen amount or buy nothing | See an aspirational relationship and enjoy having earned some choice | RS-C07, shops |
| 280–300 | Share one true story at home, watch or join the small performance, choose a city or local day | Complete the emotional day and want a next destination | F5-M06B–C |

This route includes all six side stories to demonstrate the available depth; it is **not** the recommended mandatory checklist. The play experience should allow the player to abandon a less interesting invitation and follow a creature instead. It also makes more invitations available than most players will take: the team is not automatically filled, and no menu forces five simultaneous novices into the first battle.

**Short direct route:** opening, terms, three observations, report, household/evening and destination. Estimate 60–100 minutes of first-time play depending on exploration and presentation; keep this route satisfying in itself. **One-adventure route:** add either booking and selected local stories, roughly 2–3.5 hours. **Curious route:** the table above plus detours/reading can occupy around five hours or longer. These are hypotheses for pacing review. Coverage is supplied by specific scenes and interactions, not a promise that the shortest route lasts five hours.

## The player's current reason must always be legible

| State | Default journal headline | Practical direction | Why the player might care |
|---|---|---|---|
| Before meeting Pell | Find paid road work | Tavio's wagon, Carrier Yard; Pell can also be approached directly | Better earnings and a first field reference |
| Job offered, terms not reviewed | Read the survey terms with Ada | Her Bell Court worktable; home fallback if her market move has not occurred | Understand what remains after costs |
| Ready to accept | Tell Pell whether you're taking the survey | Blue cloth at the route board | Start a finite paid job |
| Accepted, missing observations | Check the named remaining landmark(s) | Cistern tap, upper marker, wind-cut bend, each separately marked once known | Produce the promised report |
| Three observations held | Deliver the report | Pell, Three-Awning Exchange under the red roof | Earn the balance and reference |
| Base report paid | Choose your afternoon | Two offers at the exchange, public road home or city planning | Decide what to do with earned freedom |
| Booking active | One concrete next task from its scene | Current station, obstacle or receiving point | Complete the selected paid adventure |
| Evening return | Share the day and choose your next road | Home, fair rehearsal, route board | Enjoy what was gained and make a new plan |

Optional story tracking never silently displaces the main objective. The player can choose the displayed lead, pin an optional story or clear it. The stable journal records the actual report and payments, regardless of any much later fictional unreliable document. A conversation summary names both a verb and a place; “Speak to Pell” alone is insufficient.

## Authoritative world facts and transitions

The following are content-state names, not mandated code architecture. A save system may represent them differently if behavior is equivalent. Keep player evidence, NPC knowledge, paid receipts and relationship decisions separate, following [Quest and World State](Quest%20and%20World%20State.md).

| Record | Allowed values / mutation | Owner and invariant |
|---|---|---|
| `journey_phase` | Morning Arrival → Contract Accepted → Survey Settled → Booking Resolved → Evening Return | Main chapter. Advance only at named confirmation/completion, never elapsed browsing time. No booking can skip paying the completed base report. |
| `work_lead_known` | false → true from Tavio, notice, Pell or Ada's recap | Different introductions converge without inventing the skipped conversation. |
| `survey_terms_reviewed` | false → true through Ada's short review at either permitted location | Does not itself accept the job, pay an advance or trigger departure. |
| `survey_state` | offered, accepted, report_ready, settled | Settled only once after all three observation records are present. Values need not be favorable. |
| `survey_water` | unseen or observed actual flow/access plus optional maintenance note | Water observation owner. A repair is never necessary to fill this slot. |
| `survey_upper_marker` | unseen or numeral 14, with optional reverse-visibility note | Upper bend owner. Preserve what was actually examined. |
| `survey_wind_marker` | unseen or numeral 14, expected 16, footing secured/bypassed | Bend owner. Comparing the sketch can be deferred until report without losing the actual numeral. |
| `advance_paid`, `report_paid` | one-time receipts | Advance 12 splits 8 home/4 purse; report 24 splits 8 home/16 purse. Revisiting dialogue has no payment effect. |
| `field_reference` | absent → signed | Earned by truthful completion; not contingent on battle or party. Includes chosen protagonist name. |
| `booking` | undecided → orchard, wagon or none after explicit confirmation | One work window. Closing a dialogue leaves undecided. No switch after a branch starts; clear cancellation ends it without reopening the other. |
| `booking_result` | unstarted, active, completed, withdrawn, none | Safe retreat preserves active progress; cancellation is a separate explicit act. |
| `orchard_near_line`, `orchard_far_line` | incomplete → verified | Safe retreat preserves verified work. Instruments/sheet recovery remain reachable. |
| `vela_credit` | unasked, named_observation, anonymous | Her publication reflects the actual choice. Looking at wording does not decide it. |
| `wagon_loads` | three named loads: at exchange, stowed, secured_at_catch, received | Cargo cannot simultaneously occupy cart and apron. Unsafe release creates recoverable work, not erased inventory. |
| `booking_paid` | one-time receipt after selected booking complete | Orchard 18 splits 4/14; wagon 10 splits 2/8. None/withdrawn pays 0. |
| `first_city_plan` | unset, Istravel, Orthe, local_day | A plan is reversible before departure; neither is a faction pledge or permanent lock. |

The script's concrete facts override looser old opening examples: Pell waits at the exchange after accepting the contract; Mara offers practice and local introductions, not three obligatory errands before Pell's work. The fair is distributed through the inhabited town, with upper-saddle views available as a local excursion; it is not a second required remote fair replacing Rocca's shops.

### Optional content records

Residents own `s01`–`s06` method/completion/payment flags. Only S01/S02/S03 pay four personal coins each, once. Independent resident resolution is distinct from player completion: an ignored story can change its place without paying the player for work they did not do. Accepted unfinished content follows its stated prop-preservation/return rule.

The residents' [evening performance](../02%20Narrative/Rocca%20Residents%20and%20Side%20Stories.md#evening-performance--the-man-who-booked-good-weather) records actual staging, lead performer and whether the player watched or handled thunder, rain or sun. Do not infer that the finale was seen if the player left. A missed cue has an assistant continuation, not a rhythm score or lost evening reward.

Creature encounters use their RS-C identity, with separate seen, resolved, invitation-ready, accepted, declined and actual individual-location facts. Friendship is not the same as collection. An owned visitor never becomes recruitable because its keeper changes phase location. Loaned practice creatures return to their keeper; they are not secretly added to the player's collection.

Purchases decrement the named shared stock once, add the stated item once and subtract the posted price once. Mirror sales through Neri use the same vendor stock rather than a second copy. Consumable use shows its result and remaining quantity. Cosmetic clothes confer no hidden traversal or combat advantage. Quest scene props and free necessary loans cannot be replaced by a compulsory purchase.

## A reproducible walk through the money

| Receipt | Household total | Personal purse before purchases/optional pay |
|---|---:|---:|
| Start | 0 from this commission | 8 |
| Accept survey | 8 | 12 |
| Deliver base report | 16 | 28 |
| Complete orchard | 20 | 42 |
| Complete wagon, alternative to orchard | 18 | 36 |
| Neither booking or withdraw | 16 | 28 |

Completing all three paid side stories adds twelve personal coins to any corresponding line. Buying the cape (14), one salve (4), a turnover (2) and the picnic sketch (2) uses 22. The base-only traveler retains 6; a traveler who spends every optional coin still has free necessary tools, common rest, food under the contract and a walkable onward route. Family support is already accounted for; the evening conversation is acknowledgment, not another charge.

## Recovery, order and absence cases

1. **No companion:** all survey observations, both booking routes and onward travel have ordinary tools/people alternatives. Voluntary practice offers a disclosed loan. Creature refusal must never silently become a main-quest lock.
2. **Pell first:** use the direct notice introduction. Later Tavio acknowledges that the meeting already happened; he still has his market and creature scenes.
3. **Ada still home:** run the terms scene there, then mark it reviewed. Her move to the worktable uses the same knowledge and does not ask for a second approval.
4. **Wrong report destination:** Tavio, Mara and Pell's vacated blue-cloth station all give the same exchange directions. Returning home retains observations and opens a concise recap.
5. **Leave in the middle of a survey or side story:** preserve observations and accepted steps. Restarting a conversation does not reset cargo, payments or creature individuals. The map still names the missing step.
6. **Defeat or traversal mistake:** ordinary recovery goes to the named safe verge, shelter or supervised practice return. No reroll of invitations, lost reference, report deletion or vanished paid item. The appropriate encounter owns any stated local recovery task.
7. **Spend everything:** borrowing and free route alternatives remain reachable; no NPC mocks the player into reloading. Optional medicine cannot be a required boss-entry fee.
8. **Miss the rare visitor's departure:** preserve whether it was actually seen; its keeper's route lead remains. Do not replay the same spectacle by spawning a duplicate individual.
9. **Withdraw from a booking:** completion remains unpaid, but the base survey stays settled and local/city progression remains open. Do not narrate the unpaid booking as a success at home.
10. **Leave for a city early:** record earned references, contributions, invitation states and relevant local arrangement. The remaining Rocca stories use their late-return variants. The first city receives a short introduction if its field-contact bonus was not earned.
11. **Both booking receipts appear:** this is an implementation error, not a secret optimal path. Restore the actual committed branch and reconcile the incorrect extra reward without rewriting remembered player intent.
12. **Revisit after an evening:** the phase remains a story state until a declared next-day/departure transition. Shops use attendants/recall notes; the world does not run an unannounced real-world attendance schedule.

## What to observe in the user's later build

Ask a new player, after the first few minutes, what they want and where they would go next. Watch whether they approach a creature, doorway or shop without a quest marker, and whether they can explain the difference between the two bookings. On returning, ask what changed and whom they want to see again. Record skipped or dull scenes as evidence for revision. Avoid counting all readable words as minutes of engaging play.

This is a review procedure, not a performed test. The writing goal requires a coherent complete source package; actual fun, duration, visual appeal and movement remain to be judged through the user's implementation.
