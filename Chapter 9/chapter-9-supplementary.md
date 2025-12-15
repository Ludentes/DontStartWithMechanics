# Chapter 9 Supplementary: The Complete Derivation

## Purpose of This Document

The main chapter demonstrates the derivation chain through narrative—showing how "stories worth telling about characters they care about" leads to a game resembling *Rimworld*. That narrative necessarily compresses the reasoning.

This supplementary exposes the fuller process. Every term, every concept, every parameter was derived from principles rather than borrowed from existing games. The goal isn't to reverse-engineer *Rimworld*—it's to show that similar inputs produce similar outputs through systematic derivation.

If you want to understand the approach, read the chapter. If you want to see the complete reasoning, continue here.

---

## Part 1: Terminology Derivation

A common concern: "Aren't you just copying *Rimworld* and pretending you derived it?"

The answer lies in how terminology emerges. We don't start with "colonists" and "raids" and "the Rim." We start with abstract requirements, then adopt vocabulary that fits.

### From Abstract to Concrete

**Level 0 establishes setting:** Sci-fi frontier—crash survivors on a distant, hostile planet.

**Setting suggests vocabulary:**
- Survivors on a hostile planet → "colonists" (people establishing presence in dangerous territory)
- The hostile planet itself → "the Rim" (edge of civilization, frontier)
- External human threats → "raiders" (hostile groups attacking settlements)
- The place being built → "colony" or "base" or "settlement"

This isn't copying *Rimworld*. It's the natural vocabulary for "sci-fi frontier survival." A fantasy version would use "settlers" and "the Wilds" and "bandits." A post-apocalyptic version would use "survivors" and "the Wastes" and "marauders."

**Why terminology matters:** Abstract language creates distance. "Persistent distinguishable entities" doesn't engage intuition. "Colonists" does. When we say "Rosa is starving," we immediately understand stakes that "Agent 3's hunger resource is depleted" obscures.

The derivation adopts setting-appropriate language not because we're copying, but because clear communication accelerates design thinking.

### Vocabulary Reference

| Abstract Concept | Setting-Appropriate Term |
|------------------|-------------------------|
| Persistent distinguishable agents | Colonists (or survivors, pawns) |
| Constructed shelter location | Colony (or base, settlement) |
| External hostile human agents | Raiders (or pirates, hostiles) |
| The hostile environment | The Rim (or the planet, the world) |
| Resource depletion events | Starvation, freezing, exhaustion |
| Agent emotional state | Mood |
| Agent capability degradation | Injury, illness, breakdown |

---

## Part 2: Expanded Dynamics Analysis

The main chapter summarizes required dynamics. Here's the complete derivation for each aesthetic component.

### Dynamics for Attachment

What creates attachment? Not game-specific attachment—human attachment generally. Research and common experience suggest we attach to things that are:

- **Distinguishable** (not identical to others)
- **Persistent** (exist over time)
- **Vulnerable** (can be lost)
- **Invested in** (we put effort/attention toward them)

**Derived dynamics:**

**Individuation**—Each colonist must feel distinct. Not "worker #7" but "Rosa, the neurotic surgeon who hates the dark." Players need handles to differentiate and remember. This requires: varied traits, visible personality, memorable names, distinct appearance.

**Investment accumulation**—Time spent with a colonist builds attachment. The colonist who survived three raids and lost an arm means more than one who arrived yesterday. Rosa mattered because she'd been there from the beginning, because the player watched her save Chen, because her history was the colony's history.

**Vulnerability**—Colonists can be hurt, suffer, die permanently. Attachment requires stakes. If colonists are replaceable or immortal, no attachment forms. Rosa's run to the gate mattered because she could die—and did.

**Legible interiority**—Players need windows into what colonists feel, want, fear. Not just "hungry" but moods, relationships, breaking points. We knew Rosa was brave. We knew she cared about the colony. Her choice to run made *sense* because we could see inside her.

### Dynamics for Drama

Drama requires:
- **Change** (something different happens)
- **Stakes** (the change matters)
- **Causation** (the change happened *because* of something)

**Derived dynamics:**

**Consequential state changes**—Events happen that matter and persist. The raid that killed Rosa shapes the colony forever. Chen's grief affects his mood for weeks. The gate she closed still stands.

**Causal chains**—Events happen *because* of prior states. Rosa ran for the gate because she was brave (trait), because she was closest (position), because the manhunters came through that direction (threat), because the colony had been successful enough to attract attention (wealth). Maria's breakdown next week happens because Rosa died, because they were friends, because loss accumulates.

**Conjunction**—Systems collide at inopportune moments. The manhunters arrive *while* the doctor is treating someone else. The fire starts *in* the food storage. Drama requires unfortunate (or fortunate) timing. Rosa's death was dramatic because it happened at the worst possible moment—and that conjunction emerged from systems, not authorship.

### Dynamics for Emergence

Emergence requires:
- **Multiple interacting systems** (not one monolithic system)
- **Non-predetermined outcomes** (designer didn't script what happens)
- **Player-interpretable patterns** (not just noise)

**Derived dynamics:**

**System interaction**—Multiple systems affect each other. Weather affects temperature affects colonist comfort affects mood affects behavior. Wealth affects threat attention affects raid probability affects combat affects injury affects medical needs. Isolated systems don't produce emergence; interconnected systems do.

**Autonomous agents**—Colonists make decisions based on their own states, not just player commands. They refuse tasks, break down, fall in love, pick fights. Rosa chose to run—the player didn't command it. The story partly writes itself.

**Legibility**—Players can reconstruct *why* things happened. Emergence they can't understand feels arbitrary. "Of course Rosa ran for the gate—she was the bravest and closest" is emergent but legible. "Rocks fell, everyone died" is just random.

### Dynamics for Adversity

Adversity requires:
- **Pressure** (something pushing against player goals)
- **Scarcity** (not enough of something needed)
- **Possibility of failure** (pressure can win)
- **Possibility of success** (pressure can be overcome)

**Derived dynamics:**

**Resource pressure**—Never quite enough of something. Food, medicine, materials, safety, time. The colony that has everything doesn't generate stories of struggle.

**External threats**—The world attacks. Raiders, wildlife, weather, disease. The colony doesn't fail from boredom but from assault. The manhunters that killed Rosa came from outside.

**Degradation**—Things break, wear out, run low. Entropy is constant. Just maintaining equilibrium requires effort. The wall Rosa helped build will eventually need repair.

**Recovery possibility**—Adversity must be survivable (sometimes). Pure doom isn't struggle, it's inevitability. Players need hope. The colony survived the manhunters—barely. That survival mattered because it wasn't guaranteed.

### Dynamics for Memorability

Memorable experiences have:
- **Peaks** (some moments more significant than others)
- **Specificity** (this particular thing happened)
- **Narrative shape** (situation, complication, outcome)

**Derived dynamics:**

**Variable intensity**—Not everything equally important. Some events matter more, structuring memory around peaks. Rosa's death was a peak. Hauling stone was not.

**Character-centered events**—Memorable moments involve *someone*. "The time Rosa crawled back with both legs broken" not "the time resources were low." Stories are about people.

**Narrative coherence**—Events chain into something story-shaped. Beginning (peaceful colony), middle (manhunters arrive, Rosa runs), end (gate closed, Rosa gone). The shape makes it memorable.

---

## Part 3: System Function Mapping

Chapter 2 introduced six system functions every game must fulfill. Before implementing them (Level 6), we must understand what role each plays in serving our aesthetic.

### Adjudication

**Requirement:** Clear and traceable.

Players need to know why things happened—not to optimize, but to understand the story. "Rosa died because she tried to close the gate and got caught in the crossfire" requires clear cause-and-effect.

Hidden calculations are fine (players don't need to see the hit probability math). Hidden causation breaks emergence legibility (players must understand *why* Rosa died, even if they don't know the exact damage numbers).

### Information Management

**Requirement:** Rich but not overwhelming.

Players need windows into colonist internal states (mood, relationships, memories) to understand characters. But information should invite observation, not demand spreadsheet management.

Show behavioral cues at a glance. Allow inspection of detail on demand. Don't require constant monitoring to play effectively.

### Content Generation

**Requirement:** Procedural and combinatorial.

Events emerge from system interaction, not authored scripts. Content pools (traits, backstories, event types) multiply into unique situations.

The designer creates ingredients (50+ traits, 100+ backstories, event categories). Emergence creates meals (this specific Rosa with this specific history in this specific situation).

### State Persistence

**Requirement:** Comprehensive.

Consequences must persist. Injuries last. Relationships evolve. Deaths are permanent. Construction remains. The colony accumulates story.

Rosa's death persists. Chen's grief persists. The gate she closed persists. Without persistence, no story builds.

### Feedback

**Requirement:** Emotionally weighted.

Deaths should land harder than task completions. Feedback guides emotional response through intensity, not through telling players how to feel.

Rosa's death got a pause, a notification, a lasting marker. Hauling stone got nothing. The game signals what matters.

### Cognitive Framing

**Requirement:** Agents as characters, not units.

UI language, visual presentation, and information architecture consistently frame colonists as people with inner lives, not resources to optimize.

"Your colonists" not "your units." Names prominent. Personality visible. Autonomy legible. Rosa was a person, not a pawn.

---

## Part 4: Story Structure Derivation

Before structuring time, we need clarity on what we're structuring time *for*. The target is "stories worth telling." What makes something a story versus a sequence of events?

### Minimum Story Structure

- **Situation**: A state of affairs
- **Complication**: Something changes, creates tension
- **Resolution**: The complication is addressed (successfully or not)

**Example—not a story:**
"Rosa was hungry. She found food. She ate."

**Example—a story:**
"Rosa was starving. The only food was across the frozen river. She tried to cross and fell through the ice. She nearly drowned but dragged herself out. She got the food but lost two fingers to frostbite."

The difference: stakes, obstacle, cost, character persistence.

For our systems to generate stories, they must generate this pattern—not author it, but create conditions where situation → complication → resolution emerges from play.

### Sources of Complications

Complications arise when current approach stops working:

- **Depletion**: Resource exhausts, state degrades past threshold (food runs out)
- **Intrusion**: Something external arrives (manhunters appear)
- **Eruption**: Internal state crosses threshold (colonist breaks down, relationship snaps)
- **Collision**: Systems interact badly (fire starts during siege)

These are all **state transitions that create pressure**. They emerge from systems, not authored content. Rosa's death was an intrusion (manhunters) colliding with situation (open gate, brave colonist nearby).

---

## Part 5: Full Presentation Alternatives

The main chapter mentions alternative presentations. Here's the complete treatment.

### Standard Presentation

The default specification:

| Aspect | Implementation |
|--------|----------------|
| Colonist mood | Icon + number + detailed breakdown on inspection |
| Colonist health | Bar + injury list |
| Relationships | Opinion numbers (-100 to +100) |
| Needs | Bars showing current level |
| Events | Popup notifications with priority levels |
| Storyteller | Hidden (players don't see pacing mechanics) |

This serves midcore-hardcore players who want information available but not overwhelming.

### Alternative A: "The Opaque Colony"

Same mechanics. Different information management.

| Aspect | Standard | Opaque |
|--------|----------|--------|
| Colonist mood | Icon + number + breakdown | Behavior only (moping, smiling, withdrawn) |
| Colonist health | Bar + injury list | Visible wounds, limping, bandages |
| Relationships | Opinion numbers | Observation (who eats together, who avoids whom) |
| Needs | Bars | Behavior (going to food, yawning, shivering) |
| Event notification | Popup announcement | Must notice yourself |

**Design philosophy:** This alternative *Suggests* internal states through behavior rather than *Building* them explicitly in UI. Players must watch colonists like real people.

"Rosa seems off lately" rather than "Rosa: 23 mood."

You'd notice she'd been eating alone. You'd see her staring at the wall. You'd have to *pay attention* to know something was wrong.

**Effect:** Deeper engagement for invested players. Higher barrier for casual players. Same systems, dramatically different experience. Stories feel more discovered than displayed.

**Audience shift:** This pushes toward hardcore/niche. Players who want this experience exist, but it's a smaller group than the standard presentation serves.

### Alternative B: "The Dark Colony"

Same mechanics. Radically different information architecture.

**Core change:** Player only knows what colonists collectively know.

**Vision:** Each colonist has vision range. Player sees only what at least one colonist currently sees. Unexplored areas are black. Previously visited areas fade to memory (greyed, potentially outdated).

**Communication range:** Colonists within colony radius share perception. Beyond range, colonist is alone. If they're incapacitated beyond range, player loses that viewpoint entirely.

**The silence:** Rosa goes hunting. She moves beyond the colony's sight. You wait. An hour passes. She doesn't return.

Is she dead? Injured? Captured? Lost? You don't know. You might never know. Another colonist could go looking—but then they'd be beyond sight too.

**Design philosophy:** This alternative *Omits* information no colonist perceives. It's aggressive information restriction that creates genuine uncertainty.

**Effect:** Expeditions are terrifying. "Rosa went hunting three days ago and hasn't come back" is a story in itself. The unknown becomes a character. Much narrower audience—horror-adjacent experience.

**Audience shift:** This is a fundamentally different game despite identical mechanics. It serves players seeking dread and uncertainty, not those seeking story generation with visible drama.

### The Build/Suggest/Omit Framework

Chapter 2 introduced Build/Suggest/Omit for worldbuilding. The same principle applies to presentation:

- **Build:** Show explicitly (mood numbers, health bars)
- **Suggest:** Imply through behavior (moping indicates low mood)
- **Omit:** Hide entirely (no information about colonists beyond sight)

Standard presentation Builds most information. Opaque Colony Suggests it. Dark Colony Omits it. Same simulation, three different games.

---

## Part 6: Complete Parameter Tables

The main chapter provides key parameters. Here's the complete specification with derivation reasoning.

### Temporal Anchors

All other parameters derive from these constraints:

| Scale | Target Duration | Reasoning |
|-------|-----------------|-----------|
| Game day | ~15 min real time | Long enough for events, short enough for multiple days per session |
| Season | ~2.5 hours (10 days) | Seasonal change within single session |
| Year | ~10 hours (40 days) | Full year across 2-3 sessions |
| Meso episode | 10-30 min | Complete story arc, multiple per session |
| Macro session | 1-4 hours | Target play session length |

### Colonist Need Parameters

**Target:** Needs create ongoing pressure without dominating play. Address hunger every 20-40 min, rest every 40-60 min.

| Need | Full → Empty | Empty → Crisis | Reasoning |
|------|--------------|----------------|-----------|
| Food | 1 day (15 min) | 2 days (30 min) | Creates planning horizon without constant emergency |
| Rest | 0.7 days (10 min) | 1 day (15 min) | Faster than food, creates daily rhythm |
| Recreation | 1 day | 3 days (mood penalty) | Slowest need, affects mood not survival |

### Mood Parameters

**Target:** 1-2 close calls per session, 0-2 actual breakdowns. Mood should feel consequential but not constant crisis.

| Threshold | State | Breakdown Risk |
|-----------|-------|----------------|
| 70-100 | Content | None |
| 40-69 | Stressed | Minimal |
| 20-39 | Struggling | Minor (5-10% per day) |
| 1-19 | Crisis | Major (20-40% per day) |

**Mood changes:**
- Positive events: +5 to +15
- Negative events: -5 to -40
- Passive drift: ±1-3/hour based on conditions

### Skill Parameters

**Target:** Visible improvement within session, mastery across sessions.

| Level | Description | Time to Reach |
|-------|-------------|---------------|
| 0-4 | Untrained | Starting |
| 5-9 | Competent | 2-5 hours |
| 10-14 | Skilled | 5-15 hours |
| 15-19 | Expert | 15-40 hours |
| 20 | Master | 40+ hours |

### Relationship Parameters

**Target:** Noticeable change within hour, friendship/rivalry within session.

| Parameter | Value |
|-----------|-------|
| Scale | -100 to +100 |
| Starting (strangers) | 0 |
| Positive interaction | +2 to +5 |
| Negative event | -2 to -30 |
| Friendship threshold | +50 |
| Rivalry threshold | -50 |

### Resource Parameters

**Target:** Food requires planning, shortage gives 3-5 days to react.

| Parameter | Value | Reasoning |
|-----------|-------|-----------|
| Food/colonist/day | 2 meals | Simple tracking |
| Crop growth | 5-10 days | Planning horizon |
| Crop yield | 10-20 food/tile | Meaningful farm size |
| Storage decay | 2%/day (unrefrigerated) | Pressure to build refrigeration |

### Combat Parameters

**Target:** Combat dangerous but survivable. Deaths possible, not routine. Rosa's death was notable because it wasn't inevitable.

| Parameter | Value | Reasoning |
|-----------|-------|-----------|
| Colonist health | 100 HP | Round number, easy math |
| Weapon damage | 15-35/hit | 3-6 hits to down |
| Hits to down | 3-6 | Allows reaction time |
| Natural healing | 2-5 HP/day | Slow recovery |
| Tended healing | 10-20 HP/day | Meaningful medical skill |
| Base hit chance | 50% | Modified by skill, cover, range |

### Storyteller Parameters

**Target:** Episodes every 10-30 min, variant-appropriate rhythm.

| Variant | Events/Hour | Recovery Window | Experience |
|---------|-------------|-----------------|------------|
| Classic | 0.5 → 2.0 | 15-30 min | Rising pressure |
| Pastoral | 0.3 | 30-60 min | Gentle, character-focused |
| Crucible | 2.0 | 5-15 min | Desperate survival |
| Saga | Wave pattern | 20-45 min between | Epic with acts |
| Tragedy | 0.5 → 3.0 | 15 → 5 min | Inevitable decline |

**Intensity scaling:** Threat points = Colony wealth/1000 + Population × 10

---

## Part 7: What We Didn't Cover

A complete specification would require additional derivation for systems we've sketched but not fully specified.

### Technology Progression

**Questions to derive from:**
- What capabilities should unlock over time and why?
- How does research serve pacing (new options keep long games fresh)?
- How does research serve gating (some content is late-game)?
- How does research serve goal structure (escape requires advanced tech)?

### Building Specifics

**Questions to derive from:**
- What spatial configurations serve our dynamics?
- What structures serve which needs (sleeping needs beds, eating needs tables)?
- How do defense structures work?
- What production chains create interesting resource flow?

### Job Assignment Mechanics

**Questions to derive from:**
- How much control does player need while maintaining colonist autonomy?
- How do priorities interact with needs?
- What scheduling options serve session structure?

### Faction System

**Questions to derive from:**
- What external social dynamics create interesting complications?
- How do reputation and diplomacy work?
- What faction types provide varied threats and opportunities?

### Specific Event Content

**Questions to derive from:**
- What specific complications serve our episode structure?
- What categories of events exist?
- What triggers each category?
- How do events scale with colony development?

Each could be derived through the same chain: what does our aesthetic require → what dynamics serve it → what mechanics create those dynamics → what parameters tune them. The method extends to any system.

---

## Part 8: What This Derivation Demonstrates

### The Chain Produces Coherent Output

Starting from "stories worth telling about characters they care about," the derivation produced:
- Individual colonists with internal states
- Colonist autonomy
- Interconnected systems producing emergence
- AI Storyteller for pacing
- Variable presentation architectures
- Specific parameters tied to experiential targets

Each element traces back through justified decisions. Nothing was assumed from *Rimworld*—everything was derived from requirements.

### Similar Inputs Produce Similar Outputs

The result resembles *Rimworld* because we started from similar inputs:
- "Stories worth telling" (emergent narrative as primary goal)
- Solo developer constraint (systemic over authored)
- Sci-fi frontier setting (colonists, hostile world)
- Colony sim + survival archetype (base building, resource management, threats)

A designer starting from these same inputs, following the chain, would arrive somewhere similar. That's validation: the chain produces predictable outputs from inputs.

### Different Inputs Produce Different Outputs

Change the inputs, change the outputs:
- "Competitive tactical challenge" → different aesthetic → different dynamics → different mechanics
- "Meditative building flow" → different aesthetic → different pacing → different Storyteller (or none)
- "Horror survival" → similar aesthetic but fear-focused → Dark Colony presentation → different experience

The chain doesn't prescribe what game you make. It ensures that whatever you make coheres.

### Constraints Enable Rather Than Limit

Notice how constraints clarified decisions:
- "Solo developer" eliminated authored content → pushed toward emergence → produced the very quality we were seeking
- "1-4 hour sessions" required sustainable pacing → demanded Storyteller regulation
- "Stories worth telling" required specific characters → demanded individuation, vulnerability, legible interiority
- "Emergent" required surprise → demanded colonist autonomy

Without constraints, everything is equally valid and nothing is indicated. Constraints make decisions possible.

### Presentation Architecture Is Design

Same mechanics, vastly different games:
- Standard presentation → midcore-hardcore story generator
- Opaque Colony → hardcore observation game
- Dark Colony → horror-adjacent uncertainty experience

"What players know and how they learn it" isn't polish—it's fundamental to experience. Level 6 decisions can shift your entire audience.

### Creativity Lives in Derivation

The chain might seem mechanical, but creativity pervades it:
- Choosing which aesthetic targets to prioritize
- Envisioning what dynamics serve those targets
- Imagining how mechanics create dynamics
- Balancing trade-offs between approaches

The chain provides structure for creative work, not replacement for it. It ensures creative decisions connect to each other and to experiential goals. It doesn't make the decisions for you.

---

## Conclusion

This supplementary has exposed the complete derivation process—every term derived from context, every dynamic traced to aesthetic need, every parameter tied to experiential target.

The main chapter tells the story of Rosa and shows the chain in action. This document shows the machinery behind that story: the systematic reasoning that produced a game where Rosa could exist, could matter, and could die in a way that players remember.

The derivation chain doesn't guarantee good games. It guarantees coherent games—games where every element serves a purpose traceable to player experience. Whether that experience is worth having remains a creative judgment.

But coherence is the foundation. Build on it.
