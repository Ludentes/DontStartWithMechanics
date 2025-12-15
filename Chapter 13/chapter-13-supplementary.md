# Chapter 13 Supplementary: Last Light and Diagnostic Tools

This document provides complete playable rules for both versions of Last Light, plus diagnostic tools and LLM collaboration templates.

------------------------------------------------------------------------

# Part 1: Last Light (Original)

The version that wasn't working.

## Overview

Last Light is a cooperative survival game for 3-4 players. Survivors must cross hostile terrain to reach Haven before winter. Session length: 55-65 minutes.

## Components

- 4 Survivor cards (Medic, Scout, Engineer, Leader)
- 60 Event cards
- Resource tokens: Food (20), Medicine (10), Fuel (15), Hope (10)
- Journey track (12 spaces)
- Day tracker (12 days)
- 8 Equipment cards
- 4 six-sided dice

## Setup

1. Each player takes one Survivor card (or deal randomly for 3 players; one remains unused)
2. Place all survivors at Start on the journey track
3. Set starting resources: Food 8, Medicine 4, Fuel 6, Hope 6
4. Shuffle Event deck
5. Set Day tracker to Day 1

## Survivor Cards

Each survivor has:
- Role name
- Role ability (usable once per day)
- Health track (4 boxes)

**The Medic**
- Ability: Heal one survivor for 2 health without spending Medicine (once per day)

**The Scout**
- Ability: Look at the top 3 Event cards; discard one and return others in any order (once per day)

**The Engineer**
- Ability: Repair one piece of equipment without spending Fuel (once per day)

**The Leader**
- Ability: One survivor may take 3 actions instead of 2 this day (once per day)

## Day Structure

Each day proceeds through four phases:

### Phase 1: Event

Draw the top Event card. Read it aloud. The group chooses one of the options presented.

### Phase 2: Actions

Each survivor takes 2 actions. Available actions:

**Scavenge:** Roll 1d6.
- 1-2: Nothing found
- 3-4: Gain 1 resource (player's choice)
- 5-6: Gain 2 resources (player's choice, may be different)

**Heal:** Spend 1 Medicine. One survivor restores 2 health (cannot exceed 4).

**Repair:** Spend 1 Fuel. Restore one damaged Equipment card to working condition.

**Rest:** Restore 1 Hope to the group pool.

**Use Role Ability:** Use your survivor's special ability (once per day).

### Phase 3: Travel

The group decides how far to travel. Spend 1 Fuel per space moved. You may move 0 spaces (conserving Fuel).

Must reach space 12 by end of Day 12 to win.

### Phase 4: Night

Consume 1 Food per survivor.

If insufficient Food:
- First, lose 1 Hope per missing Food
- If Hope is 0, each survivor without Food takes 1 damage

Check for deaths. Any survivor at 0 health is dead and removed from the game.

Advance Day tracker. If Day 12 ends and you haven't reached Haven, you lose.

## Event Cards (Sample)

**Blizzard**
Choose one:
- Lose 2 Fuel
- All survivors take 1 damage

**Raider Scouts**
Choose one:
- Lose 3 Food
- One survivor takes 2 damage

**Abandoned Cache**
Roll 1d6:
- 1-2: Nothing useful
- 3-4: Gain 2 Food
- 5-6: Gain 2 Food and 1 Medicine

**Rough Terrain**
Choose one:
- Spend 1 extra Fuel to travel today
- All survivors take 1 damage

**Illness**
One survivor (group chooses) is sick.
- Spend 2 Medicine to cure immediately, OR
- Survivor takes 1 damage at the end of each day until cured

**Shortcut**
Choose one:
- Take the shortcut: Move 2 spaces for free, but each survivor takes 1 damage
- Take the safe route: No effect

*(Full deck contains 60 cards with similar resource/damage trade-offs)*

## Equipment Cards

Equipment provides ongoing bonuses. If damaged, must be Repaired before use.

**Medical Kit:** +1 health restored when using Heal action
**Compass:** +1 to Scout's ability (see 4 cards instead of 3)
**Tool Set:** Engineer may repair without using an action (still once per day)
**Rations:** -1 Food consumed at Night (minimum 2 for group)
**Warm Clothes:** Take 1 less damage from cold-weather Events
**Weapon:** +1 to one damage roll per day when Events involve combat
**Map:** May look at top Event card at start of each day
**First Aid Training:** Medic ability heals 3 instead of 2

## Victory and Defeat

**Victory:** At least 2 survivors reach space 12 (Haven) by end of Day 12.
- Score: Number of survivors who reached Haven (2, 3, or 4)

**Defeat:**
- Fewer than 2 survivors remain alive, OR
- Day 12 ends without reaching Haven

## What Was Wrong

This version produced the following playtest results:

| Metric | Result | Target |
|--------|--------|--------|
| Win rate | 62% | 40-50% |
| Engagement (1-10) | 5.2 | 7+ |
| Cared about survivor | 20% | 70%+ |
| Felt tense | 25% | 60%+ |
| Would play again | 45% | 70%+ |

Players described it as "fine," "a puzzle," and "moving cubes." Characters were indistinguishable except by ability. Events felt like random obstacles. No dramatic arc emerged.

------------------------------------------------------------------------

# Part 2: Last Light (Revised)

The version that works.

## Overview

Same premise: cooperative survival, cross hostile terrain, reach Haven. But now with character attachment, moral dilemmas, and escalating threat.

## Components

- 4 Survivor cards (Jin, Marcus, Elena, Kofi) with traits, stress tracks, memory slots
- Act 1 Event deck (16 cards)
- Act 2 Event deck (16 cards)  
- Act 3 Event deck (16 cards)
- Dilemma deck (12 cards)
- Crisis deck (8 cards)
- Resource tokens: Food (20), Medicine (10), Fuel (15)
- Memory tokens (20, various types)
- Consequence tokens (12: 6 positive, 6 negative)
- Pursuit token
- Journey track (12 spaces) with Pursuit track
- Day tracker (12 days)
- 8 Equipment cards
- 4 six-sided dice

## Setup

1. Each player takes one Survivor card
2. Place all survivors at Start (space 0)
3. Place Pursuit token at space -3 (three spaces behind Start)
4. Set starting resources: Food 6, Medicine 3, Fuel 6
5. Separate Event decks by Act; shuffle each
6. Shuffle Dilemma deck and Crisis deck separately
7. Set Day tracker to Day 1

## Survivor Cards

Each survivor has:
- Name and portrait
- Trait (personality that affects play)
- Ability (mechanical capability)
- Health track (4 boxes)
- Stress track (3 boxes)
- Memory slots (3 spaces)
- Consequence slot (1 space)

### Jin Okonkwo (The Protector)

**Trait - Protective:** When a survivor adjacent to Jin would take damage, Jin may take that damage instead. If Jin chooses not to protect when she could, she gains a Guilty token.

**Ability - Shield:** Once per day, prevent 1 damage to any survivor in the same space as Jin.

**Starting Stress:** 1 (she feels responsible for everyone)

*Card back:* "Jin was a paramedic before everything fell apart. She's seen too much death to let anyone else die on her watch—even if it destroys her."

### Marcus Cole (The Calculator)

**Trait - Pragmatic:** Marcus gains +1 to all Scavenge rolls. However, when the group makes a choice Marcus considers "inefficient," he must either argue against it or gain a Cold token.

**Ability - Assess:** Once per day, look at the top 2 Event cards from the current Act deck. Return them in any order.

**Starting Stress:** 0 (emotionally detached)

*Card back:* "Marcus ran supply logistics for a major retailer. He sees the world in resources and probabilities. He's usually right about the math. He's learning that math isn't everything."

### Elena Vasquez (The Believer)

**Trait - Hopeful:** Once per day, Elena may remove 1 stress from any survivor (including herself). However, when the group makes a choice Elena considers "cruel," she gains 2 stress.

**Ability - Inspire:** Once per day, all survivors may reroll one die each on their next roll.

**Starting Stress:** 0 (faith sustains her)

*Card back:* "Elena was a hospice chaplain. She held hands with the dying and helped families say goodbye. She believes there's meaning in suffering. She's not sure she still believes that."

### Kofi Mensah (The Survivor)

**Trait - Scarred:** Kofi ignores the first stress he would gain each day. However, Kofi cannot benefit from other survivors' Comfort actions or Elena's Hopeful trait.

**Ability - Endure:** Once per day, ignore one negative effect from an Event that targets Kofi specifically.

**Starting Stress:** 2 (already carrying weight)

*Card back:* "Kofi walked out of a city that doesn't exist anymore. He doesn't talk about what happened there. He doesn't sleep well. He keeps moving because stopping means remembering."

## Stress and Breakdown

Each survivor has 3 stress boxes.

**Gaining Stress:** Various events, consequences, and situations add stress.

**Losing Stress:** The Comfort action removes 1 stress. Some events and memories allow stress removal.

**Breakdown:** When a survivor's stress track fills completely:
1. That survivor loses their next full day (cannot take actions or use abilities)
2. Clear all stress
3. Gain a Trauma consequence token

**Trauma:** A survivor with a Trauma token has -1 maximum stress (breaks down at 2 stress instead of 3). Multiple Trauma tokens stack.

## Memory Tokens

When significant events occur, place a memory token on involved survivor(s). Memory tokens are visible and accumulate across the game.

**Memory Types and Effects:**

| Memory | How Earned | Effect |
|--------|------------|--------|
| Saved [Name] | Protected another from death/major harm | Once per game, may take stress for [Name] |
| Made Sacrifice | Took significant harm for group benefit | Once per game, may add +2 to any roll after seeing result |
| Found Hope | Discovered something good during darkness | Once per game, remove 2 stress from self |
| Showed Courage | Faced danger when could have fled | Once per game, ignore one source of stress |
| Nearly Died | Reduced to 1 health | No mechanical effect; contributes to epilogue |
| Broke Down | Stress track filled | -1 max stress for remainder of game |
| Made Hard Choice | Central to a Dilemma decision | No mechanical effect; contributes to epilogue |

**Using Memory Effects:** Announce the memory, describe how it applies to the current situation, then apply the mechanical effect. Each memory effect can only be used once per game.

## Consequence Tokens

Consequence tokens represent lasting changes to a character from the choices they've made.

**Positive Consequences:**
- **Brave:** Earned through heroic action. +1 to rolls when protecting others.
- **Compassionate:** Earned through mercy. May remove 1 stress from another once per day without using action.
- **Leader:** Earned through decisive action in crisis. Once per day, give another survivor +1 action.

**Negative Consequences:**
- **Haunted:** Earned by leaving someone behind. +1 stress at start of each day until redemption.
- **Cold:** Earned by choosing efficiency over humanity. Cannot benefit from others' Comfort actions.
- **Guilty:** Earned by failing to protect when you could. -1 to all rolls until you successfully protect someone.

Redemption: Some positive actions can remove negative consequences. This is noted on relevant Event and Dilemma cards.

## Day Structure

Each day proceeds through five phases:

### Phase 1: Pursuit

Move the Pursuit token 1 space toward the group.

If the Pursuit reaches the group's space:
1. Draw a Crisis card and resolve it immediately
2. Move the Pursuit token back 2 spaces

### Phase 2: Event

Draw from the appropriate Event deck:
- Days 1-4: Act 1 deck
- Days 5-8: Act 2 deck
- Days 9-12: Act 3 deck

Additionally:
- Days 5-8: Draw 1 Dilemma card after the Event
- Days 9-12: Draw 2 Dilemma cards after the Event

Resolve all drawn cards in order. Group decides together.

### Phase 3: Actions

Each survivor (who isn't broken down) takes 2 actions:

**Scavenge:** Roll 1d6 (Marcus adds +1).
- 1-2: Nothing found
- 3-4: Gain 1 resource (choice)
- 5-6: Gain 2 resources (choice)

**Heal:** Spend 1 Medicine. One survivor restores 2 health.

**Repair:** Spend 1 Fuel. Restore one Equipment card.

**Comfort:** Remove 1 stress from any survivor. If targeting another survivor, both may optionally gain a "Supported" memory (write both names).

**Delay Pursuit:** Spend 2 resources (any combination). Move Pursuit back 1 space. Character gains "Held the Line" memory.

**Use Ability:** Use your survivor's special ability.

### Phase 4: Travel

Spend 1 Fuel per space. May move 0 spaces.

### Phase 5: Night

Consume 1 Food per survivor.

If insufficient Food:
- Each survivor without food takes 1 damage

Check for deaths (0 health = dead).

Advance Day tracker.

## Event Cards by Act

### Act 1: The Road (Days 1-4)

Establishing events. Moderate difficulty. Character traits introduced.

**Rough Terrain**
*The path ahead is treacherous. Loose rocks and hidden drops.*
Choose one:
- Spend 1 extra Fuel to proceed safely
- Each survivor tests: roll 1d6, take 1 damage on 1-2

**Cold Night**
*The temperature drops faster than expected.*
Choose one:
- Spend 2 Fuel to keep fires burning
- Each survivor gains 1 stress

**Abandoned Vehicle**
*A rusted truck sits in the road. Something might be useful inside.*
Roll 1d6:
- 1-2: Nothing but bones
- 3-4: Gain 2 Food
- 5-6: Gain 2 Food and 1 Fuel

**The Watchers**
*You spot figures on a distant ridge. They're watching you.*
Choose one:
- Spend 1 Fuel to detour around them (Pursuit advances 1 extra space)
- Continue on path (nothing happens... this time)

**Illness**
*One survivor wakes up feverish.*
Choose a survivor. That survivor:
- Spends 1 Medicine immediately to recover, OR
- Takes 1 damage and gains 1 stress

**River Crossing**
*The bridge is out. The river runs cold and fast.*
Choose one:
- Spend 2 Fuel to find a crossing upstream
- Attempt to ford: each survivor rolls 1d6, takes 1 damage on 1-3

**Old Campsite**
*Someone was here before. Recently.*
Gain 1 Food. Then choose:
- Search thoroughly: Roll 1d6. On 4+, gain 1 Medicine. On 1, the Pursuit advances 1.
- Move on quietly

**The Storm**
*Dark clouds gather. You can push through or find shelter.*
Choose one:
- Push through: All survivors take 1 damage, but travel is free today
- Shelter: No travel today, but gain 1 Food (foraging while waiting)

*(8 additional Act 1 events in similar pattern)*

### Act 2: The Trials (Days 5-8)

Pressure increases. Character-targeted events appear.

**The Wounded Stranger**
*A man lies by the road, leg clearly broken. He reaches toward you.*
Choose one:
- Help him: Spend 1 Medicine and 1 Food. He tells you of a cache (gain 2 resources of choice later, at end of day)
- Leave him: The survivor who found him gains "Haunted" consequence

**Raider Territory**
*You've entered dangerous ground. Signs of violence everywhere.*
Choose one:
- Fight through: Each survivor takes 1 damage, but gain 2 Food from their supplies
- Sneak around: Pursuit advances 2 spaces

**The Child** *(targets survivor with lowest stress)*
*A child sits alone among the wreckage. She doesn't speak.*
[Lowest-stress survivor] must choose:
- Take her: Consume +1 Food per day until Haven. If she survives, [survivor] gains "Compassionate" consequence
- Leave her: [Survivor] gains "Haunted" consequence

**Fever Dreams** *(targets survivor with highest stress)*
*[Highest-stress survivor] wakes screaming. The dreams are getting worse.*
That survivor:
- Gains 1 stress, OR
- Another survivor may take 1 stress to sit with them through the night (both may gain "Supported" memory)

**The Cache**
*You find a sealed bunker. The lock looks intact.*
Marcus (or highest-Intelligence equivalent) may attempt: Roll 1d6.
- 4+: Open it. Gain 3 Food, 2 Medicine, 1 Fuel
- 1-3: Trigger an alarm. Pursuit advances 2 spaces

**The Ambush**
*Raiders. They were waiting.*
Each survivor takes 1 damage. Then choose:
- Stand and fight: One survivor takes 2 additional damage. Gain "Showed Courage" memory. Raiders are defeated (gain 2 Food)
- Run: Pursuit advances 2 spaces. Lose 1 Food.

*(10 additional Act 2 events with escalating stakes)*

### Act 3: The Reckoning (Days 9-12)

Crisis events. Sacrifice moments. Final approach.

**The Collapse**
*The bridge ahead is failing. Timbers groan.*
Choose one:
- Everyone crosses together, quickly: Pursuit advances 2 spaces
- One survivor stays behind to stabilize the bridge: That survivor takes 3 damage. If they survive, gain "Hero" memory. If they die, all other survivors may remove 2 stress.

**Final Push**
*Haven is visible in the distance. But so is what's following you.*
Choose one:
- All-out run: Spend 3 Fuel to move 3 spaces free. Each survivor takes 1 damage from exhaustion
- Steady pace: Normal travel. But the Pursuit advances 1 extra space

**The Last Medicine**
*One dose remains. Two survivors need it.*
Choose one survivor to receive the Medicine. The other takes 2 damage and gains 1 stress. The survivor who made the choice gains "Made Hard Choice" memory.

**Sacrifice at the Pass**
*The path narrows. Only one person can hold them off.*
One survivor may volunteer to stay behind:
- That survivor cannot reach Haven (removed from game, but not "dead")
- Pursuit stops for remainder of game
- Volunteer gains "Hero" memory (noted in epilogue)
- All other survivors remove all stress

If no volunteer: Pursuit advances 3 spaces

**The Final Night**
*One more night before Haven. But the cold is deadly.*
Spend 2 Fuel or each survivor takes 2 damage and gains 1 stress.

*(8 additional Act 3 events)*

## Dilemma Cards

Drawn in addition to Events during Acts 2 and 3. Always present difficult character choices.

**The Straggler**
*You almost miss her in the snow—a woman, barely conscious, reaching toward you.*
Choose one:
- **Take her with you.** One survivor gains "Rescued" memory. Group consumes +1 Food per day. Stranger has 2 health—if group takes damage, she takes it first. If she survives to Haven, rescuer gains "Compassionate" consequence.
- **Leave her behind.** The survivor who found her gains "Haunted" consequence (+1 stress each morning until they do something redemptive).

**The Betrayer**
*You catch one of your group hiding Food. Enough for three days. For one person.*
Choose one:
- **Confront them.** That survivor gains 2 stress but adds the Food to group supplies (gain 3 Food). Others may not use Comfort on that survivor until they apologize (in-character moment).
- **Say nothing.** Gain 3 Food, but if any survivor dies of hunger later, the survivor who said nothing gains "Guilty" consequence.

**The Old Man's Request**
*He's dying. Nothing can save him. He asks you to end his suffering.*
One survivor must choose:
- **Grant his request.** Gain 1 Medicine (he gives you his supply). Gain "Made Hard Choice" memory. Survivor must roll 1d6: on 1-2, gain 1 stress.
- **Refuse.** He dies anyway, hours later, in pain. All survivors gain 1 stress.

**The Shortcut**
*There's a faster path. Through the place that burned. Where the bodies are.*
Choose one:
- **Take the shortcut.** Move 2 spaces for free. Each survivor gains 1 stress. Elena (if present) gains 2 stress instead.
- **Go around.** Pursuit advances 2 spaces.

**The Weak Link**
*One survivor is slowing everyone down. Injured, stressed, struggling.*
(Target: survivor with lowest health + most stress)
Choose one:
- **Wait for them.** Pursuit advances 1 space. Target removes 1 stress. All others may gain "Supported" memory with target.
- **Push them harder.** Target takes 1 damage and gains 1 stress. If this causes death or breakdown, all survivors gain 1 stress.

**The Trader**
*A stranger offers supplies. But the price is service.*
Choose one:
- **Accept:** Gain 3 Food and 2 Medicine. One survivor must stay with the trader for a day (cannot take actions on the next day). That survivor gains "Made Sacrifice" memory.
- **Refuse:** Nothing happens. But you'll wonder.

**The Signal**
*There's a radio. It might still work. Haven might hear you. But so might others.*
Choose one:
- **Use the radio.** Roll 1d6. On 4+: gain 2 Food (supply drop). On 1-3: Pursuit advances 2 spaces.
- **Stay silent.** Nothing happens.

**The Child's Choice**
*(Only if group has a child from earlier event)*
*The child speaks for the first time. She tells you where raiders store their supplies. But getting there means crossing open ground they're watching.*
Choose one:
- **Trust her.** Dangerous. Each survivor rolls 1d6; take 1 damage on 1-2. If successful, gain 4 Food and 2 Medicine.
- **Don't risk it.** The child stops speaking again. Survivor who originally saved her gains 1 stress.

**The Reckoning**
*A survivor who was left behind earlier appears. They survived. They found you. They have a knife.*
(Only triggers if "Haunted" consequence exists from earlier event)
The Haunted survivor must choose:
- **Face them.** Take 2 damage. Roll 1d6: on 4+, talk them down (remove Haunted, gain "Found Hope" memory). On 1-3, they attack (take 1 more damage, but Haunted is still removed).
- **Hide.** Haunted remains. Gain 1 stress. They'll be back (draw an extra Crisis card on next Pursuit catch).

**The Mercy**
*A survivor is barely alive. No medicine left. They're in pain.*
(Triggers when a survivor reaches 1 health with no Medicine in supply)
Choose one:
- **Use everything trying.** Spend 2 Food (improvised treatment). Roll 1d6: on 4+, survivor stabilizes at 1 health. On 1-3, they die anyway.
- **Let them go.** Survivor dies. All other survivors may remove 1 stress (peaceful ending).

**The Leader Falls**
*(Triggers when first survivor dies)*
*You've lost someone. The group looks to each other.*
Highest-Stress survivor must choose:
- **Take charge.** Remove 1 stress from all other survivors. Gain "Leader" consequence. Gain 2 stress yourself.
- **Fall apart.** All survivors gain 1 stress.

**The Threshold**
*(Triggers on Day 11 or 12 when Haven is 2 or fewer spaces away)*
*You can see it. You can almost touch it. But the way is blocked.*
Choose one:
- **Burn the obstacle.** Spend 3 Fuel. Path is clear. Travel is free for remaining days.
- **Climb over.** Each survivor takes 1 damage. One survivor (choice) may fall: roll 1d6, on 1-2 take 2 additional damage. If anyone volunteers to go first (taking the risk alone), they gain "Showed Courage" memory.

## Crisis Cards

Drawn when Pursuit catches the group. Always bad.

**They're Here**
Each survivor takes 2 damage. Lose 2 Food.

**The Hunt**
Choose one survivor to lead them away. That survivor takes 3 damage and cannot take actions next day. Others take no damage.

**Cornered**
Lose all Fuel OR each survivor takes 2 damage and gains 1 stress.

**The Price**
Choose: Lose one piece of Equipment permanently, OR one survivor gains "Traumatized" (permanent -1 max stress).

**Overrun**
Each survivor takes 1 damage and gains 1 stress. Pursuit does not reset (remains at group's position).

**The Trade**
Lose 3 Food and 2 Medicine OR one survivor (group chooses) is captured (removed from game, but may appear again if you reach Haven).

**Scattered**
Separate into two groups until end of next day. Each group takes separate Events and cannot share resources or use abilities on each other.

**Nightmare Fuel**
Each survivor gains 2 stress. Anyone who breaks down from this takes 1 damage in addition to normal breakdown effects.

## The Pursuit

The Pursuit represents whatever is following the group—raiders, creatures, the consequences of past decisions. It is always visible on the track.

**Movement:**
- Advances 1 space at start of each day (Phase 1)
- Various Events and choices advance it additional spaces
- Players can spend 2 resources (any combination) as an action to push it back 1 space

**Catch-Up:**
When Pursuit reaches the group's space:
1. Draw and resolve a Crisis card
2. Move Pursuit back 2 spaces

**Strategic Implications:**
- Can't be permanently escaped
- Creates constant tension and second-order decisions
- Allows voluntary delay (push it back) at resource cost
- Late-game catches are more dangerous (Crisis cards are bad)

## Victory and Defeat

**Victory Conditions (all required):**
1. At least 2 survivors reach Haven (space 12) by end of Day 12
2. At least 1 survivor has no Trauma tokens

**Defeat Conditions (any):**
- Fewer than 2 survivors remain alive
- Day 12 ends without reaching Haven
- All surviving characters have Trauma (hollow victory—reframe as bittersweet loss)

**Scoring:**
- 2 survivors reach Haven: Pyrrhic victory
- 3 survivors reach Haven: Victory
- 4 survivors reach Haven: Triumphant victory
- Bonus: Each survivor without Trauma: +1
- Bonus: Each survivor with 2+ positive memories: +1

## Epilogue

After the game ends (win or lose), go around the table. Each player narrates what happens to their survivor, incorporating:
- Their memories
- Their consequences  
- Their relationships formed during play
- Whether they reached Haven

This takes 5-10 minutes and provides closure.

------------------------------------------------------------------------

# Part 3: Diagnostic Toolkit

## Framework Summary (Copy-Paste for LLM)

```
DIAGNOSTIC FRAMEWORK

The derivation chain has eight levels. Problems at higher levels can't be fixed by changes at lower levels.

Level 0 - Context: Medium, platform, constraints, setting, archetype
Level 1 - Aesthetic: What experience players should have (Tension, Narrative, Challenge, Fellowship, etc.)
Level 2 - Dynamics: What players must do/perceive for the aesthetic to emerge
Level 3 - Temporal: Loop scales, session structure, pacing, dramatic beats
Level 4 - Paradigm: Consistency (fixed rules), Framework (judgment-based), or Adaptive (adjusts to player)
Level 5 - Mechanics: Specific systems that produce the dynamics
Level 6 - Presentation: How the game communicates with players
Level 7 - Parameters: Specific numbers that tune intensity

DIAGNOSTIC PROCESS

1. Gather symptoms (what players say/do, metrics, gaps between intended and actual)
2. Map symptoms to candidate levels
3. Check candidates top-down (highest first—if high level is broken, lower fixes won't help)
4. Identify primary cause (highest broken level)
5. Fix at that level first, then adjust lower levels

SYMPTOM MAPPING

"Boring/nothing happens" → Check Level 3, then Level 2
"Don't care about X" → Check Level 2 (attachment dynamics), then Level 6
"Feels random/unfair" → Check Level 4, then Level 5
"Too easy/hard" → Check Level 7, then Level 3
"Feels like puzzle not story" → Check Level 1, then Level 2
"Nothing memorable" → Check Level 2 (peak dynamics), then Level 3
"Confusing" → Check Level 6, then Level 5
"Sessions drag/end abruptly" → Check Level 3, then Level 7
"Theme doesn't fit" → Check Level 0, then Level 2

KEY MEASURABLES

Attachment: Name usage %, emotional response to loss, post-session stories referencing characters
Tension: Self-reported tension curve, perceived danger progression, physical indicators
Dilemma: Discussion time, disagreement frequency, tone shift, post-choice affect
Pacing: Engagement peaks distribution, session "shape" description, stopping-point satisfaction
```

## Symptom-to-Level Mapping (Detailed)

| Symptom | First Check | What to Look For | Then Check |
|---------|-------------|------------------|------------|
| "It's boring" | Level 3 | Flat temporal structure, no peaks | Level 2: Missing dynamics |
| "I don't care about [X]" | Level 2 | Attachment dynamics absent | Level 6: X not foregrounded |
| "It feels random" | Level 4 | Paradigm mismatch | Level 5: Unclear mechanics |
| "It feels unfair" | Level 5 | Rules unclear or inconsistent | Level 4: Wrong paradigm |
| "Too easy" | Level 7 | Parameters too forgiving | Level 3: No pressure build |
| "Too hard" | Level 7 | Parameters too punishing | Level 4: Paradigm too harsh |
| "Feels like a puzzle" | Level 1 | Delivering Challenge not Narrative | Level 2: Optimization dynamics |
| "Nothing memorable" | Level 2 | No peak dynamics | Level 3: Peaks left to chance |
| "I'm confused" | Level 6 | Presentation unclear | Level 5: Mechanics ambiguous |
| "Sessions drag" | Level 3 | Missing stopping points | Level 7: Duration wrong |
| "Theme doesn't fit" | Level 0 | Context conflicts | Level 2: Dynamics contradict theme |
| "Same every time" | Level 2 | No emergence dynamics | Level 5: Too deterministic |
| "Can't stop playing" | Level 3 | Missing stopping points | Level 2: Exploitative dynamics |
| "Don't know what to do" | Level 6 | Goals unclear | Level 2: Missing decision forcing |

## Level-by-Level Diagnostic Questions

### Level 0: Context

- Does the medium support the intended experience?
- Are platform constraints compatible with the aesthetic?
- Do time/player count constraints permit the dynamics?
- Does the archetype fit the experience goal?
- Reference: What other games achieve similar goals in similar constraints?

### Level 1: Aesthetic

- What experience IS being delivered? (Not intended—actual)
- What do players report feeling?
- Does delivered experience match intended?
- If mismatch: Is the intended aesthetic achievable, or does the game want to be something else?

### Level 2: Dynamics

- List required dynamics for intended aesthetic
- For each: Is it present? What measurable would show it?
- Check attachment: Do players use names? Care about loss?
- Check tension: Is it persistent or sporadic?
- Check forcing: Are decisions forced, or can players optimize around them?
- Check dilemma: Are trade-offs calculable or incommensurable?
- Check emergence: Are there surprising developments, or is everything predictable?

### Level 3: Temporal

- Draw the intended tension curve
- Draw the actual tension curve (from playtests)
- Are peaks designed or accidental?
- Do sessions have satisfying arc?
- Are stopping points clear?
- Is escalation present?

### Level 4: Paradigm

- Which paradigm is implemented? (Consistency/Framework/Adaptive)
- Does that paradigm fit the aesthetic?
- Is calculation displacing experience?
- Is ambiguity creating confusion rather than emergence?

### Level 5: Mechanics

- For each required dynamic: what mechanic should produce it?
- Is that mechanic present?
- Is it working as intended?
- Are any mechanics working against the aesthetic?

### Level 6: Presentation

- Can players perceive what matters?
- Are important elements foregrounded?
- Does visual/textual hierarchy match importance?
- Does framing support emotional engagement?

### Level 7: Parameters

- What are your measurable targets?
- What are actual results?
- Is the gap fixable by number tuning, or is it structural?

## Key Measurables by Dynamic

### Attachment Dynamics

| Measurable | Method | Healthy Range |
|------------|--------|---------------|
| Name usage | Count character names vs. role names in play | 50%+ character names |
| Death response | Observe reaction to character death | Pause, tone shift, expressions |
| Post-session stories | Ask "what happened?" note subject | 50%+ mention specific characters |
| Character decision time | Time discussions about individual characters | 60+ seconds on character-specific choices |
| Unprompted character voice | Count "X would/wouldn't do that" statements | 2+ per session per player |

### Tension Dynamics

| Measurable | Method | Healthy Range |
|------------|--------|---------------|
| Self-reported tension | Ask players to rate tension 1-10 at intervals | Rising curve toward climax |
| Perceived danger | Ask "how likely did failure seem?" | Should increase over session |
| Physical indicators | Observe posture, leaning in, expressions | Increased engagement in later phases |
| "Close call" reports | Count post-session reports of near-failure | 1-3 per session |

### Dilemma Dynamics

| Measurable | Method | Healthy Range |
|------------|--------|---------------|
| Discussion time | Time deliberation on choices | 60+ seconds on dilemmas vs. 20 on standard |
| Disagreement rate | Note when players initially disagree | 40%+ of dilemmas |
| Tone shift | Observe change from analytical to values-based | Present in true dilemmas |
| Post-choice affect | Note residual emotion after choosing | Lingering discomfort/satisfaction |

### Pacing Dynamics

| Measurable | Method | Healthy Range |
|------------|--------|---------------|
| Engagement curve | Ask players to graph engagement over session | Peaks in second half |
| Stopping satisfaction | Rate satisfaction at stopping points | 4+/5 at designed stops |
| Time perception | Ask how long session felt | Close to actual (flow state) |
| "One more" requests | Count requests to continue past stopping point | 1-2 (engaged) not 5+ (trapped) |

## Diagnostic Worksheet

```
GAME: _______________________
INTENDED AESTHETIC: _______________________
DELIVERED AESTHETIC: _______________________

SYMPTOMS OBSERVED:
1. _______________________
2. _______________________
3. _______________________

CANDIDATE LEVELS (from symptom mapping):
Level ___: because _______________________
Level ___: because _______________________

TOP-DOWN VERIFICATION:

Level 0 (Context): Pass / Fail
Notes: _______________________

Level 1 (Aesthetic): Mismatch identified? Y/N
If yes, what's actually being delivered? _______________________

Level 2 (Dynamics): Required dynamics present?
- ____________: Present / Absent
- ____________: Present / Absent  
- ____________: Present / Absent

Level 3 (Temporal): Structure supports peaks? Y/N
Notes: _______________________

Level 4 (Paradigm): Paradigm fits aesthetic? Y/N
Notes: _______________________

Level 5 (Mechanics): Mechanics produce dynamics? Y/N
Notes: _______________________

PRIMARY CAUSE: Level ___
Reasoning: _______________________

CONTRIBUTING CAUSES: Levels ___
Reasoning: _______________________

FIX APPROACH:
[ ] Accept what was built (reframe aesthetic)
[ ] Rebuild toward vision (significant rework)
[ ] Patch the gaps (targeted fixes)

SPECIFIC CHANGES NEEDED:
1. _______________________
2. _______________________
3. _______________________
```

------------------------------------------------------------------------

# Part 4: LLM Collaboration Templates

## Initial Context Prompt

```
I'm using the derivation chain framework to diagnose a broken game. The framework has 8 levels:

0-Context, 1-Aesthetic, 2-Dynamics, 3-Temporal, 4-Paradigm, 5-Mechanics, 6-Presentation, 7-Parameters

Problems at higher levels can't be fixed by lower-level changes.

MY GAME:
[Brief rules summary - 2-3 paragraphs max]

INTENDED EXPERIENCE:
[What players should feel - specific aesthetics]

ACTUAL EXPERIENCE (from playtests):
[What players report - quotes if possible]

THE GAP:
[Specific differences between intended and actual]

Based on these symptoms, which levels should we check first?
```

## Level-Specific Diagnostic Prompts

### Level 2 (Dynamics)

```
We're checking Level 2 (Dynamics) for [GAME NAME].

Intended aesthetic: [AESTHETIC]

For this aesthetic, what dynamics would need to be present? 
(e.g., for Narrative/Attachment: individuation, investment accumulation, legible interiority, consequential history)

Here are my current mechanics:
[RELEVANT MECHANICS SUMMARY]

For each required dynamic:
1. Is it present in these mechanics?
2. What measurable behavior would indicate its presence?
3. If absent, what mechanical addition would produce it?
```

### Level 3 (Temporal)

```
We're checking Level 3 (Temporal Architecture) for [GAME NAME].

Current structure:
[SESSION STRUCTURE - phases, duration, loops]

Intended experience arc:
[WHAT SHOULD THE TENSION/ENGAGEMENT CURVE LOOK LIKE]

Observed experience arc:
[WHAT PLAYTESTERS REPORT]

Questions:
1. Does the current structure guarantee dramatic peaks or leave them to chance?
2. Where should peaks occur for this aesthetic?
3. What structural changes would produce designed rhythm instead of random rhythm?
```

### Level 5 (Mechanics)

```
We're diagnosing Level 5 (Mechanics) for [GAME NAME].

Required dynamics (from Level 2):
- [DYNAMIC 1]
- [DYNAMIC 2]
- [DYNAMIC 3]

Current mechanics:
[MECHANICS SUMMARY]

For each required dynamic:
1. What mechanic should produce it?
2. Is that mechanic present?
3. If present, is it producing the intended dynamic or something else?
4. If absent, what mechanic would produce it?

Additionally: Are any current mechanics working against the intended aesthetic?
```

## Fix Derivation Prompts

### Generating Options

```
We've identified the primary cause: Level [X] is broken.

Specifically: [WHAT'S WRONG]

The game currently works like this:
[RELEVANT MECHANICS]

Generate 3 different approaches to fix this:
1. A minimal intervention (smallest change that might work)
2. A structural change (redesign the problematic system)
3. A reframe (accept what's built, adjust expectations)

For each, note:
- What changes
- What this affects downstream
- Risks/tradeoffs
```

### Evaluating Fixes

```
We're considering this fix for [GAME NAME]:

[PROPOSED CHANGE]

Check this against the chain:

1. Does it serve the intended aesthetic (Level 1)?
2. Does it produce the required dynamics (Level 2)?
3. Does it fit the temporal architecture (Level 3)?
4. Is it consistent with the paradigm (Level 4)?
5. Does it integrate with existing mechanics (Level 5)?
6. Can it be clearly presented (Level 6)?
7. Can it be tuned via parameters (Level 7)?

What issues do you see? What refinements would help?
```

### Defining Measurables

```
We're implementing this fix:

[CHANGE DESCRIPTION]

Before we test, we need to define success.

For this change to work, what should we observe?
1. What player behaviors would indicate success?
2. What metrics should we track?
3. What's the target range for each metric?
4. What would indicate failure (need to iterate further)?
```

------------------------------------------------------------------------

# Quick Reference Card

**The Diagnostic Process**

1. Gather symptoms → 2. Map to levels → 3. Check top-down → 4. Find primary cause → 5. Fix at that level

**Symptom Shortcuts**

- Boring → Level 3
- Don't care → Level 2
- Random/unfair → Level 4-5
- Too easy/hard → Level 7
- Puzzle not story → Level 1-2
- Nothing memorable → Level 2-3

**Key Principle**

Symptoms manifest low. Causes live high. Don't tune parameters for a dynamics problem.

**Measurables Tell Truth**

- Attachment: Name usage, death response, character stories
- Tension: Reported curve, perceived danger, physical lean-in
- Dilemma: Discussion time, disagreement, post-choice discomfort
- Pacing: Engagement peaks, stopping satisfaction, time perception
