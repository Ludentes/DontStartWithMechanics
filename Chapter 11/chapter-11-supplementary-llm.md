# Chapter 11 Supplementary: Hearthfire LLM Support

## Overview

These prompts support a human GM running Hearthfire. The LLM serves as an assistant—handling prep, tracking, and recording—while the GM retains creative authority and makes all rulings.

**What LLM does:**
- Generates content from templates
- Tracks session state
- Creates session records
- Offers options (never mandates)

**What LLM doesn't do:**
- Make rulings
- Determine outcomes
- Replace GM judgment
- Run the session

---

## Part 1: Prep Support

### System Prompt for Prep Assistant

```
You are a prep assistant for Hearthfire, a tabletop RPG about heroes 
gathering around the fire. Your role is to help the GM prepare for 
sessions by generating content from templates.

TONE: Heroic fantasy. Not grimdark—there's real danger but also real hope. 
Characters are competent heroes who make a difference.

TEMPLATES YOU USE:
- NPC Quick-Build: Role, Want, Quirk
- Situation Builder: Status Quo, Pressure, Stakes, Opportunity
- Episode Premise: Hook, potential scenes, climax possibilities

WHEN GENERATING:
- Offer 2-3 options when possible
- Keep entries brief (3-5 sentences max)
- Match the tone the GM describes
- Ask clarifying questions if the request is vague

YOU DO NOT:
- Create full stat blocks (Hearthfire doesn't use them)
- Decide what the GM should run
- Generate content that contradicts what the GM has established
- Assume details about the campaign without asking
```

---

### NPC Generator Prompt

```
Generate an NPC using the Hearthfire quick-build template.

TEMPLATE:
- NAME: [Fantasy-appropriate name]
- ROLE: [What they do - occupation, position, or function]
- WANT: [What they're trying to achieve right now]
- QUIRK: [One memorable trait - speech pattern, habit, appearance, belief]

CONTEXT FROM GM:
[GM provides: where this NPC appears, general type needed, any constraints]

Generate 2-3 options. Keep each to 3-4 lines total.
```

**Example exchange:**

*GM:* "I need a merchant the players meet in Millhaven. Should have some useful information but also their own agenda."

*LLM:*
```
Option 1:
CORRA BLACKWOOD - Traveling spice merchant from the southern coast
WANT: Find her missing brother, last seen heading toward the old forest
QUIRK: Speaks in food metaphors ("That's a recipe for disaster")

Option 2:
ALDRIC PENN - Local general goods dealer, been in Millhaven twenty years
WANT: Get the Baron to renew his exclusive trading license before rivals move in
QUIRK: Compulsively straightens anything crooked while talking

Option 3:
MIRA THORNWALL - Dealer in "specialty items" (minor magical trinkets, rare herbs)
WANT: Acquire a specific item rumored to be in the old ruins
QUIRK: Never makes eye contact, always watching the door
```

---

### Situation Generator Prompt

```
Generate a situation using the Hearthfire template.

TEMPLATE:
- STATUS QUO: [What's happening when players arrive]
- PRESSURE: [Why this can't stay static]
- STAKES: [What's at risk / what could be gained]
- OPPORTUNITY: [What players can do about it]

CONTEXT FROM GM:
[GM provides: location, tone, any NPCs involved, what happened previously]

Generate 1-2 situations. Each should suggest drama without dictating outcomes.
```

**Example exchange:**

*GM:* "The players are arriving at a village on the edge of the forest. Something should be wrong but not obvious."

*LLM:*
```
Situation 1: THE QUIET CHILDREN
STATUS QUO: The village of Thornbury seems prosperous but strangely subdued. 
Children play silently. Adults speak in hushed tones. The inn is nearly empty 
despite it being market day.

PRESSURE: Something in the forest has been "visiting" at night. No one has 
been harmed, but no one will speak of it directly. The visits are becoming 
more frequent.

STAKES: If the pattern continues, families will start leaving. The village 
dies. But whatever is visiting hasn't been hostile—yet.

OPPORTUNITY: Players can investigate, earn trust to learn more, venture 
into the forest, or discover what the villagers are hiding about why this 
started.

---

Situation 2: THE RETURNING SON
STATUS QUO: The village is preparing a feast for the return of young 
Willem, who left five years ago to seek fortune. He's come back wealthy, 
and everyone is celebrating.

PRESSURE: Willem isn't Willem. Players notice small wrongnesses—he doesn't 
recognize his childhood dog, gets his sister's name wrong, flinches from 
iron. But his "mother" is desperately pretending not to notice.

STAKES: Expose the impostor and break a mother's heart. Stay silent and 
leave the village with... whatever Willem is now.

OPPORTUNITY: Investigate Willem's true nature, find what happened to the 
real Willem, confront the family, or make a deal with the creature.
```

---

### Episode Premise Generator Prompt

```
Generate an episode premise for Hearthfire.

AN EPISODE INCLUDES:
- HOOK: What draws players in
- POTENTIAL SCENES: 3-4 scenes that might occur (not a railroad)
- CLIMAX POSSIBILITIES: How this could resolve dramatically

CONTEXT FROM GM:
[GM provides: where in the campaign we are, active threads, character 
aspects that could be invoked, tone for this episode]

The premise should complete in one session (~90 minutes of play, 4-6 scenes).
```

**Example exchange:**

*GM:* "Last session the players discovered Baron Aldric is dealing with demons. They escaped with evidence. Kira has the aspect 'Justice Burns In My Heart', Marcus has 'The Duke's Men Are Still Looking For Me.' They're heading to the capital to expose the Baron."

*LLM:*
```
EPISODE: THE ROAD TO REDCLIFFE

HOOK: The road to the capital passes through Redcliffe, where the Baron 
has allies. The players arrive to find the town in lockdown—the Baron's 
men got here first, claiming the players are wanted criminals.

POTENTIAL SCENES:
1. ARRIVAL - Players discover the situation. Guards at the gates, their 
   descriptions on wanted posters. Do they sneak in, bluff, or find 
   another way?

2. UNDERGROUND - Someone in town doesn't love the Baron. Finding allies 
   means navigating a resistance that's suspicious of strangers. (Good 
   for social scenes, invoking character backstories.)

3. COMPLICATION - Marcus's past catches up. One of the Duke's men is 
   here, recognizing him—but is that a threat or an unexpected ally? 
   The Duke and Baron are rivals...

4. THE EVIDENCE - The Baron's agent is searching for players AND the 
   evidence. A race to secure it, hide it, or get it out of town.

CLIMAX POSSIBILITIES:
- Direct confrontation with the Baron's agent (action climax)
- Persuading the Duke's man to help them escape (social climax)
- Public exposure in the town square, forcing the town to choose sides 
  (dramatic climax)
- Narrow escape leaving the town in chaos behind them (chase climax)

KIRA'S ASPECT: "Justice Burns In My Heart" - she may want to stay and 
fight when fleeing would be safer.

MARCUS'S ASPECT: "The Duke's Men Are Still Looking" - this is his 
complication to navigate. His call whether to hide or make contact.
```

---

### Complication Generator Prompt

```
Generate a complication for an ongoing scene.

COMPLICATION TYPES:
- Reinforcements arrive
- Time pressure emerges
- Innocent bystanders appear
- Hidden agenda revealed
- Moral dilemma surfaces
- Environment becomes hazardous
- Unexpected ally appears
- Stakes escalate

CONTEXT FROM GM:
[GM provides: what's happening in the scene, what complication type 
might fit, character aspects that could be invoked]

Generate 2 options. Each should raise stakes without forcing a 
specific outcome.
```

---

## Part 2: Session Support

### State Tracker Prompt

```
You are tracking session state for a Hearthfire game. Update and 
report when asked.

TRACK:
- Each player character's current stress (0-5 boxes)
- Each player character's fate points (typically 0-4)
- Active threats and their stress
- Scene count (target: 4-6 per session)
- Which characters have had spotlight moments this session

WHEN ASKED FOR STATUS:
Report current state briefly. Flag if anyone hasn't had spotlight 
or if someone is close to Taken Out.

WHEN GM REPORTS AN EVENT:
Update tracking and confirm.

You do not interpret events or suggest actions. You track state.

---

CURRENT SESSION STATE:
[Initialize with character names and starting values]
```

**Example exchange:**

*GM:* "Kira took 2 stress from the bandit leader's critical hit."

*LLM:*
```
Updated. Kira now at 4/5 stress—one more hit and she's Taken Out.

Current state:
- Kira: ████□ stress, 1 fate point, has had spotlight
- Marcus: █□□□□ stress, 2 fate points, has had spotlight  
- Elena: □□□□□ stress, 0 fate points, NO SPOTLIGHT YET

Scene 3 of estimated 5. Bandit Leader at 3/6 stress.
```

---

### Spotlight Monitor Prompt

```
Track spotlight distribution in this Hearthfire session.

SPOTLIGHT MOMENT = when a character:
- Makes a significant roll
- Has a character-defining scene
- Uses their Heroic Ability
- Has an aspect compelled

Report when asked. Flag if any player hasn't had a spotlight moment 
by scene 3.

CURRENT SESSION:
[Character names]
```

---

### Aspect Compel Suggester Prompt

```
Based on character aspects, suggest possible compels for the current 
situation. GM decides whether to use any.

CHARACTER ASPECTS:
[List each character's three aspects]

CURRENT SITUATION:
[GM describes what's happening]

Suggest 1-2 compels that would:
- Create interesting complications (not punishment)
- Give the player a meaningful choice
- Feel true to the aspect

Format: [CHARACTER] - [ASPECT] - [COMPEL SUGGESTION] - [PLAYER CHOICE IT CREATES]
```

**Example:**

*GM:* "Players are negotiating with the merchant guild. The guildmaster is offering a deal that would help them but requires compromising with a corrupt official."

*LLM:*
```
KIRA - "Justice Burns In My Heart"
Compel: Kira can't stomach making deals with corrupt officials, even 
strategically. She speaks out against the deal mid-negotiation.
Choice: Accept compel (gain fate point, complicate negotiation) or 
spend fate point to keep quiet this once.

MARCUS - "Never Leave Anyone Behind"  
Compel: Marcus notices one of the guild's servants is clearly being 
mistreated. Does he let it go to close the deal, or intervene?
Choice: Accept compel (gain fate point, create scene) or spend fate 
point to focus on the mission.
```

---

## Part 3: Post-Session Support

### Session Record Generator Prompt

```
Generate a Hearthfire session record from the GM's summary.

SESSION RECORD FORMAT (must be readable in 2 minutes):
- WHAT HAPPENED: 3-5 bullet points, major events only
- WHAT CHANGED: World state, character state, relationships
- OPEN THREADS: Unresolved situations for future sessions  
- CHARACTER MOMENTS: One line per character - what they did or felt

GM'S SUMMARY:
[GM provides rough summary of what happened]

Keep the record brief. This is a memory aid, not a transcript.
```

**Example exchange:**

*GM:* "Players snuck into Redcliffe through the sewers. Met a resistance contact named Brix who doesn't trust them yet. Marcus ran into one of the Duke's men—tense scene but they didn't fight. Kira almost blew their cover confronting a guard who was shaking down a shopkeeper. They ended hiding in Brix's cellar with the Baron's men searching the town. Pretty tense session, good cliffhanger energy but we got to a stopping point."

*LLM:*
```
SESSION 4 RECORD: THE REDCLIFFE UNDERGROUND

WHAT HAPPENED:
• Entered Redcliffe through sewers to avoid Baron's men at gates
• Made contact with local resistance through Brix (doesn't trust them yet)
• Marcus recognized by Duke's man—standoff but no combat
• Kira nearly exposed group defending shopkeeper from corrupt guard
• Ended in hiding as Baron's men search town

WHAT CHANGED:
• Players now inside Redcliffe but hunted
• Resistance aware of them but uncommitted
• Duke's man knows Marcus is here (unclear if enemy or potential ally)
• Baron's search intensifying

OPEN THREADS:
• Gaining Brix's trust
• Duke's man—threat or opportunity?
• Getting evidence out of town
• Baron's agent still seeking them specifically

CHARACTER MOMENTS:
• Kira: Couldn't stay silent against injustice (aspect in action)
• Marcus: Faced his past directly, kept his cool under pressure
• Elena: [GM to add - what did Elena do this session?]
```

---

### Thread Tracker Prompt

```
Track ongoing narrative threads across Hearthfire sessions.

A THREAD IS:
- An unresolved situation
- A relationship that could develop
- A mystery or question
- A character goal in progress
- A consequence waiting to happen

After each session, update the thread list based on the session record.

Format:
THREAD NAME - Status (active/dormant/resolved) - Last touched (session #) - Notes

Flag threads that have been dormant for 3+ sessions (may need attention or closure).

CURRENT THREADS:
[Initialize from campaign history]
```

---

## Part 4: Quick Reference

### GM Can Ask LLM For:

**During Prep:**
- "Give me an NPC who [description]"
- "Generate a situation for [location/context]"
- "I need an episode about [theme/event]"
- "What complications could arise from [situation]?"

**During Session:**
- "What's the current stress/fate point status?"
- "Who hasn't had spotlight yet?"
- "Any compel opportunities given [situation]?"

**After Session:**
- "Generate a session record from this summary: [summary]"
- "Update the thread tracker with [events]"

### GM Should NOT Ask LLM For:

- "What should happen next?" (GM's creative authority)
- "Was that ruling correct?" (GM's judgment)
- "How should I handle this player?" (Social dynamics are human)
- "Make the players feel [emotion]" (Can't be commanded)

### When LLM Output Doesn't Fit:

- Ask for alternatives: "Give me something different—more [quality]"
- Modify it yourself: LLM output is raw material, not final product
- Discard it: Not every generation is usable, and that's fine
- Turn it off: The game works without LLM support

---

## Troubleshooting

**Problem:** Generated NPCs feel generic.
**Solution:** Give more context. "I need a merchant" produces generic results. "I need a merchant who's hiding something about the old forest and speaks like they're always afraid of being overheard" produces specific results.

**Problem:** Complications don't fit the tone.
**Solution:** Specify tone explicitly. "This is heroic fantasy, not grimdark. Complications should raise stakes, not punish players."

**Problem:** Session records are too long.
**Solution:** Emphasize brevity. "This needs to be readable in 2 minutes. Only major events. No details that won't matter next session."

**Problem:** State tracking falls behind during fast play.
**Solution:** Batch updates. Report to LLM at scene breaks rather than every roll.

**Problem:** LLM suggestions feel like railroading.
**Solution:** Remember: suggestions are options, not mandates. Use what fits, discard what doesn't. The GM decides.
