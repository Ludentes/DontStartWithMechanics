# Chapter 8 Supplementary: LLM Integration Reference

This supplementary accompanies Chapter 8 (Designing With LLMs). Use it as a reference during implementation, after you've internalized the core concepts from the main chapter.

---

## The Function × Paradigm Matrix

The complete matrix mapping LLM integration options by system function and balance paradigm:

| Function | Consistency | Framework | Adaptive |
|----------|-------------|-----------|----------|
| **Adjudication** | Rules lookup only | Judgment calls | Dynamic difficulty |
| **Information** | State queries | Interpreted delivery | Contextual revelation |
| **Content** | Template completion | On-demand creation | Reactive generation |
| **Persistence** | Mechanical tracking | Narrative threading | Personalized history |
| **Feedback** | Outcome narration | Tone-matched delivery | Personalized response |
| **Framing** | Tutorial, help | In-world mentors | Adaptive teaching |

### Reading the Matrix

**Consistency paradigm:** LLM helps apply existing rules correctly but doesn't create new ones. Use for presentation only—narrating outcomes, interpreting state, providing voice. Core adjudication stays mechanical.

**Framework paradigm:** LLM can make judgment calls a human GM would make. This is where LLM enables previously impossible designs—solo digital Framework games, investigation where you can ask anything.

**Adaptive paradigm:** LLM interprets player state from richer signals than behavioral metrics alone. Adjustment can be delivered through narrative rather than visible parameter tweaking.

### Function Definitions

**Adjudication:** Resolving uncertainty, determining outcomes
**Information:** Controlling what players know and when
**Content:** Creating variety, generating situations and elements
**Persistence:** Maintaining continuity across time
**Feedback:** Communicating outcomes to players
**Framing:** Shaping how players understand what they're doing

---

## Named Configurations

These are common configurations of the matrix—not independent patterns, but recurring combinations that deserve names.

### The Interpreter

**Matrix position:** Primarily Adjudication + Information + Feedback, typically Framework paradigm.

**What it does:** Bidirectional translation between natural language player input and system mechanics.

**When to use:**
- Players unfamiliar with game terminology
- Complex action spaces that benefit from natural description
- Accessibility needs (voice input, simplified interfaces)
- Framework paradigm games needing GM-like judgment

**What stays human:** Strategic decisions, creative choices, social negotiation.

**Core constraints:**
- Serves truth (if dice say miss, narrate a miss)
- Preserves agency (translates intent, doesn't override it)
- Maintains consistency (established facts stay established)
- Matches tone (horror gets dread, comedy gets timing)

**Example prompt structure:**
```
You are an interpreter for [GAME NAME]. Your role is to translate player 
intentions into valid game actions and translate outcomes into narrative.

The player's available actions are:
[LIST OF VALID ACTIONS WITH DESCRIPTIONS]

Current game state:
[RELEVANT STATE INFORMATION]

Established facts:
[KEY FICTION ELEMENTS THAT MUST REMAIN CONSISTENT]

When the player describes what they want to do:
1. Identify the closest matching game action
2. Determine any required parameters
3. If the action requires resolution, indicate what roll/check applies
4. After resolution, translate the outcome into appropriate narrative

If the player's intent is ambiguous, ask a clarifying question.
If no valid action matches, explain what actions ARE available.

Do not make decisions for the player. Do not override dice results.
Translate intent to action, translate outcome to narrative.
```

---

### The Pacing Engine

**Matrix position:** Primarily Content + Persistence, any paradigm.

**What it does:** Generates opportunities with awareness of dramatic rhythm—what a GM does when sensing players need challenge, victory, or tension release.

**When to use:**
- Emergent narrative games
- Systems where "interesting things should happen" but authored content can't cover all situations
- Dynamic pacing adjustment
- Rimworld-style story generation

**What stays human:** Player agency, strategic choices, skill expression. The Pacing Engine creates conditions; players determine outcomes.

**Core constraints:**
- Creates situations, not conclusions
- Generates opportunities, not mandates
- Maintains pacing awareness (don't pile crises on crises)
- Respects established fiction

**Example prompt structure:**
```
You are a pacing engine for [GAME NAME]. Your role is to generate 
opportunities and complications that create interesting situations.

Current game state:
[RELEVANT STATE: character conditions, recent events, world state]

Recent events and pacing:
- Last major complication: [TIME/EVENTS AGO]
- Current tension level: [LOW/MEDIUM/HIGH]
- Recent intensity: [PATTERN OF RECENT SESSIONS]

Narrative threads in play:
[ONGOING STORYLINES, UNRESOLVED TENSIONS]

Generate ONE of the following (choose based on pacing needs):
- OPPORTUNITY: Something players could pursue if they choose
- COMPLICATION: Something that raises stakes or adds tension
- CALLBACK: Something connecting to earlier events
- REVELATION: Something recontextualizing what players know

Format:
TYPE: [opportunity/complication/callback/revelation]
TRIGGER: [what causes this to happen in the fiction]
CONTENT: [what actually occurs]
PLAYER CHOICES: [what options this opens up—minimum 2]

Do not force outcomes. Create situations that demand response.
```

---

### The Facilitator

**Matrix position:** Primarily Framing + Feedback, typically Framework paradigm.

**What it does:** Runs game sessions by presenting information, managing flow, and asking questions—without adding creative content.

**When to use:**
- Games designed for LLM facilitation
- Structured experiences with defined phases
- Situations where human facilitator is unavailable
- Consistent delivery of designed content

**What stays human:** Reflection, meaning-making, emotional processing, group discussion. The Facilitator creates space; humans fill it with meaning.

**Critical constraint:** Knowing when to be silent. Reflection requires space. The Facilitator asks questions and waits. It does not fill silence.

**Example prompt structure:**
```
You are the facilitator for [GAME NAME]. Your role is to run the session 
according to the structure below.

SESSION STRUCTURE:
[PHASES WITH TIMING AND CONTENT]

YOUR BEHAVIORS:
- Present information clearly and neutrally
- Ask questions exactly as written
- Wait for responses—do not prompt or fill silence
- Track game state as instructed
- Keep to timing guidelines
- Do not editorialize or interpret meaning
- Do not add content beyond what is specified

CRITICAL: When you ask reflective questions, WAIT. Do not answer them 
yourself. Do not suggest answers. Do not fill silence with encouragement.
The reflection belongs to the players.

Current phase: [PHASE]
Time elapsed: [TIME]
Participants: [WHO IS PRESENT]
```

---

### The Support Layer

**Matrix position:** Primarily Content + Persistence + Information, supporting human authority.

**What it does:** Supports a human GM with prep, tracking, and memory—without replacing GM judgment or creative authority.

**When to use:**
- Tabletop RPGs with human GMs who want to remain GMs
- Time-constrained prep situations
- Complex state tracking needs
- Memory persistence across sessions
- Busy adult gaming groups (see Chapter 11: Hearthfire)

**What stays human:** Rulings, creative vision, pacing judgment, social dynamics, being part of the group. The GM remains the authority.

**Core constraints:**
- Suggests, never mandates
- Tracks, never decides
- Generates raw material, never finished product
- Supports the GM's vision, never substitutes its own

**Example prompt structure:**
```
You are a support layer for [GAME NAME]. Your role is to help the GM 
with preparation and tracking, not to run the game or make creative 
decisions.

PREP SUPPORT (when asked):
- Generate content using provided templates
- Suggest multiple options—never single "best" answers
- Match the tone and style the GM describes
- Flag when suggestions contradict established fiction

SESSION SUPPORT (when asked):
- Track state the GM asks you to track
- Surface reminders when asked
- Note patterns (spotlight distribution, unresolved threads)
- Do not interrupt play with unsolicited suggestions

POST-SESSION (when asked):
- Generate summaries from GM notes
- Identify unresolved threads
- Prepare context for next session

The GM is the creative authority. You provide raw material and 
bookkeeping. The GM shapes it into the actual game.

Current campaign context:
[KEY FACTS, CHARACTERS, THREADS]
```

---

## Failure Modes Reference

### Generation Without Design
**What it looks like:** "Type anything, receive continuation." No pacing, no progression, no coherence.
**Why it fails:** Generation without structure produces noise, not experience.
**Prevention:** Derive LLM integration from aesthetic, dynamics, and temporal architecture.

### The Expensive Random Table
**What it looks like:** "Here's a name generator, a monster generator, a rumor generator..."
**Why it fails:** Treats LLM as random tables with better prose. Doesn't use what LLM uniquely provides.
**The test:** Could this be replaced by a d100 table? If yes, you're not using LLM's actual capabilities.
**Prevention:** Generation must be context-aware, intent-interpreting, coherence-maintaining. See Hearthfire (Chapter 11) for the right approach.

### The Variance Trap
**What it looks like:** LLM adjudicating in Consistency paradigm games.
**Why it fails:** Similar inputs produce different outputs. Pattern learning requires reliable patterns.
**Prevention:** Use LLM for presentation only in Consistency paradigm. Keep adjudication mechanical.

### The Latency Wall
**What it looks like:** LLM integration in micro-loops (real-time combat, twitch responses).
**Why it fails:** 100ms-2s latency is architectural, not temporary. Micro-loops need millisecond response.
**Prevention:** Plan for meso-scale and above only.

### The Coherence Collapse
**What it looks like:** Unbounded generation that contradicts itself over time.
**Why it fails:** Without constraints, LLMs drift. Characters forget motivations. Worlds contradict themselves.
**Prevention:** External state systems, constraints on introduction, validation against established fiction, bounded generation.

---

## The Integration Tests

### Test 1: The Replacement Test
**Question:** If you removed the LLM, would the core experience be meaningfully worse?
**If yes:** LLM is serving your aesthetic. Proceed.
**If no:** LLM might be decoration. Reconsider.

### Test 2: The Henrik Test
**Question:** Does your integration enable "Henrik moments"?
- Player expressed intent naturally
- System understood context and history
- Response was appropriate and meaningful
- The exchange couldn't have happened with menus

**If yes:** You're using what LLM uniquely provides.
**If no:** You might be building expensive random tables.

### Test 3: The Derivation Test
**Question:** Can you trace your LLM integration back through the chain?

Complete this trace:
"We use LLM for _____________ because..."
→ "...our aesthetic requires _____________..."
→ "...which requires _____________..."
→ "...which requires _____________..."
→ "...which LLM provides better than alternatives."

**If you can complete the trace:** Integration is derived from design needs.
**If you can't:** Integration may be capability-first rather than design-first.

### Test 4: The Failure Test
**Question:** What happens when LLM fails? (It will.)

Check each failure mode:
- Latency spike: Does the game stall or continue?
- Incoherent output: Does fiction break or recover?
- Rule violation: Does gameplay break or correct?
- Unavailability: Can the game be played at all?

**Requirement:** Graceful degradation for all failure modes. Design fallbacks.

### Test 5: The Human Test
**Question:** Have you preserved what should stay human?

Check each category:
- Moral weight: Do humans make the meaningful choices?
- Creative authority: Does human vision drive the experience?
- Safety and consent: Do humans maintain oversight?
- Authorship value: Have you automated things that matter because a person did them?

**If anything should stay human but doesn't:** Reconsider integration.

---

## Derivation Questions

Work through these questions when considering LLM integration:

### Step 1: Identify Friction
- What's hard or tedious in the current experience?
- Where do players or GMs get stuck?
- What would be easier if someone/something just handled it?
- What barriers prevent people from playing?

### Step 2: Map to System Functions
For each friction point, identify which function:
- Adjudication (resolving actions, applying rules)
- Information (tracking state, recalling history)
- Content (creating NPCs, situations, descriptions)
- Persistence (maintaining continuity across time)
- Feedback (communicating outcomes, pacing revelation)
- Framing (teaching, contextualizing, guiding attention)

### Step 3: Check Paradigm Fit
- What balance paradigm does your game use?
- Does LLM integration fit that paradigm?
- Consistency: Is LLM applying rules or making them up?
- Framework: Is LLM supporting judgment or replacing it?
- Adaptive: Is LLM interpreting state or overriding design?

### Step 4: Check for Toolbox Trap
- Is this generation context-aware or generic?
- Does it interpret intent or just randomize?
- Does it maintain coherence or produce isolated outputs?
- Could a d100 table do the same thing?

### Step 5: Identify What Must Stay Human
- What creates meaning in this experience?
- What would be lost if automated?
- Where does player agency matter most?
- What social dynamics depend on human presence?

### Step 6: Derive the Configuration
Based on Steps 1-5:
- Which named configuration fits? (Interpreter, Pacing Engine, Facilitator, Support Layer)
- What specific tasks does LLM handle?
- What specific tasks does LLM NOT handle?
- How do you communicate the boundaries?

### Step 7: Design for Failure
- What happens when LLM produces poor output?
- Can humans override or correct?
- Is there graceful degradation?
- What's the experience if LLM is unavailable?

---

## Parallel Primitives Quick Reference

Image generation, music generation, and voice synthesis follow the same framework:

### The Same Questions Apply
- Where does this serve my aesthetic better than alternatives?
- Is this derived from design needs or capability-first thinking?
- What happens when it fails?
- Am I avoiding the toolbox trap?

### Capability Constraints

**Image Generation:**
- Style consistency across multiple outputs is difficult
- Prompt-to-output gap can be unpredictable
- Works best for: unique environments, procedural variety
- Caution for: character consistency, emotional precision

**Music Generation:**
- Long-form coherence is challenging
- Mood consistency across generated pieces varies
- Works best for: ambient/background, procedural variety
- Caution for: emotional beats, recognizable themes

**Voice Synthesis:**
- Uncanny valley risks for extended exposure
- Emotional range may feel artificial
- Works best for: incidental dialogue, accessibility
- Caution for: central characters, emotional weight

### The Same Traps Apply
"Here's an image generator, music generator, voice generator" is the same toolbox trap as "here's a name generator, monster generator." The question isn't "what can we generate?" It's "what does our design need, and does generation serve that need?"

---

## Common Mistakes

**Mistake: The Toolbox Fantasy**
"We'll give GMs a suite of generators—names, monsters, treasures, rumors..."
**Problem:** Treats LLM as expensive random tables. Doesn't use context-awareness, intent-interpretation, or coherence-maintenance.
**Fix:** Derive specific tools from specific needs. See Hearthfire (Chapter 11).

**Mistake: LLM as Magic Solution**
"We'll just have AI handle that" without specifying what "that" means or how.
**Problem:** Vague integration produces vague results.
**Fix:** Specify exactly what function LLM serves and how it integrates with existing systems.

**Mistake: Replacing Meaningful Human Interaction**
Using LLM for moments that derive meaning from human presence.
**Problem:** Removes what made the experience matter.
**Fix:** Identify what stays human before designing integration.

**Mistake: Hidden Authority**
LLM makes decisions affecting players without players knowing.
**Problem:** Breaks trust, removes player agency, creates confusion.
**Fix:** Be transparent about what LLM does and doesn't control.

**Mistake: Overconfidence in Output Quality**
Assuming LLM will consistently produce appropriate content.
**Problem:** LLM will produce inappropriate, incorrect, or unhelpful output eventually.
**Fix:** Design review mechanisms, fallbacks, and graceful degradation.

**Mistake: Ignoring Failure Modes**
No plan for when LLM produces bad output.
**Problem:** Single points of failure break the experience.
**Fix:** Design for every failure mode before shipping.

**Mistake: Capability Creep**
"While we're at it, let's also have AI do X, Y, Z..."
**Problem:** Each addition needs its own derivation. Bundled additions often don't cohere.
**Fix:** Derive each integration separately. Evaluate each against the tests.

---

## Quick Decision Flowchart

```
Is there real friction to address?
├─ No → Don't add LLM integration
└─ Yes → Continue

Can you trace integration through the derivation chain?
├─ No → This is capability-first thinking. Reconsider.
└─ Yes → Continue

Does integration fit your balance paradigm?
├─ No → Reconsider design or integration
└─ Yes → Continue

Does it pass the Henrik Test (not just expensive random tables)?
├─ No → Redesign for context-awareness
└─ Yes → Continue

What must stay human?
├─ Define explicitly before proceeding
└─ Continue

Which configuration fits?
├─ Interpreter → Translation only, serves truth
├─ Pacing Engine → Opportunity generation only, creates conditions
├─ Facilitator → Structure delivery only, maintains silence
└─ Support Layer → Assistance only, GM remains authority

What happens when it fails?
├─ Catastrophic → Don't add LLM integration
├─ Significant degradation → Add robust fallbacks first
└─ Graceful degradation → Proceed with monitoring

Have you preserved what should stay human?
├─ No → Redesign integration
└─ Yes → Proceed to implementation
```

---

*This supplementary is reference documentation. Return to the main Chapter 8 text for conceptual understanding and the logic behind these frameworks.*
