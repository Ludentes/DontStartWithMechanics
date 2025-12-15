# Chapter 7 Supplementary Material: Derivation Chain Quick Reference

This supplementary material accompanies Chapter 7 (The Derivation Chain). Use it during active design work as a checklist, diagnostic tool, and documentation template.

## Related Supplementary Documents

This is the primary Chapter 7 reference. Additional supplementaries provide deeper coverage of specific topics:

| Document | Contents | Use When... |
|----------|----------|-------------|
| **The Dimming** | Complete playable TTRPG one-shot | You want to see a finished artifact from the derivation chain |
| **Casual Mobile Roguelike** | Extended worked example with production numbers | You need content derivation examples (art budgets, word counts) |
| **Archetype Library** | 15+ archetypes with full profiles | You're selecting or modifying an archetype at Level 0 |
| **Testing and Playtesting** | Validation methodology by chain level | You're preparing for or interpreting playtests |

---

## What's In This Document

| Section | What You'll Find | Use When... |
|---------|------------------|-------------|
| **The Chain At a Glance** | Single-page summary of all levels | Quick reference during design |
| **Level-by-Level Checklist** | Questions and outputs for each level | Working through a derivation |
| **Entry Point Flowchart** | Decision tree for where to start | Beginning a new project |
| **Coherence Audit Template** | Verification questions between levels | Checking design integrity |
| **Decision Matrices** | Lookup tables for all levels | Quick reference for common patterns |
| **Symptom-to-Level Diagnostic** | Problem → Likely cause mapping | Troubleshooting broken designs |
| **Iteration Documentation Template** | Structured change tracking | Recording and learning from iterations |
| **System Functions Reference** | Six functions with design options | Specifying presentation architecture |

---

## The Chain At a Glance

```
LEVEL 0: CONTEXT
What's fixed? Medium, platform, constraints, setting, archetype
                    ↓
LEVEL 1: AESTHETIC PROFILE  
What experience? Primary/secondary aesthetics, player profile, success criteria
                    ↓
LEVEL 2: REQUIRED DYNAMICS
What behaviors? Observable dynamics, economic dynamics, spatial dynamics, anti-dynamics
                    ↓
LEVEL 3: TEMPORAL ARCHITECTURE
What rhythm? Loop scales, durations, pacing pattern, stopping points
                    ↓
LEVEL 4: BALANCE PARADIGM
What approach? Consistency / Framework / Adaptive (or hybrid)
                    ↓
LEVEL 5: MECHANICAL SPECIFICATION
What systems? Core mechanics, resources, content approach
                    ↓
LEVEL 6: PRESENTATION ARCHITECTURE
How communicated? Adjudication, information, feedback, framing
                    ↓
LEVEL 7: PARAMETERS
What numbers? Specific values derived from measurable targets
                    ↓
VALIDATION: Does it work? Coherence audit → Playtest → Iterate
```

---

## Level-by-Level Checklist

### Level 0: Context

**Questions to answer:**
- [ ] What medium? (Video game, tabletop, hybrid)
- [ ] What platform? (PC, mobile, console, in-person, online)
- [ ] What development constraints? (Time, team size, budget)
- [ ] What content constraints? (Rating, cultural considerations)
- [ ] What setting? (Even if cosmetic, name it)
- [ ] What archetype? (Or explicitly: no existing archetype)

**Outputs:**
- [ ] Fixed constraints documented
- [ ] Flexible constraints identified
- [ ] Setting vocabulary established
- [ ] Archetype expectations clear (see Archetype Library supplementary)

---

### Level 1: Aesthetic Profile

**Questions to answer:**
- [ ] What primary aesthetic?
- [ ] What secondary aesthetics (priority order)?
- [ ] What excluded aesthetics?
- [ ] Who is target player? (Casual/midcore/hardcore)
- [ ] What cognitive budget? (Tracked elements capacity)
- [ ] What session expectations?
- [ ] What defines success? (Testable criteria)

**Outputs:**
- [ ] Primary aesthetic named and defined
- [ ] Secondary aesthetics prioritized
- [ ] Player profile with cognitive implications
- [ ] Success criteria that can be tested

---

### Level 2: Required Dynamics

**Questions to answer:**
- [ ] What must players DO to experience target aesthetic?
- [ ] What must players FEEL at key moments?
- [ ] What must players LEARN or master?
- [ ] What behaviors would UNDERMINE the aesthetic?
- [ ] Do dynamics have SPATIAL expression?
- [ ] What ECONOMIC dynamics serve the aesthetic?
- [ ] How does each SYSTEM FUNCTION serve the aesthetic?

**Outputs:**
- [ ] Core loop behaviors identified
- [ ] Peak moment dynamics specified
- [ ] Anti-dynamics listed (what to prevent)
- [ ] Economic dynamics (scarcity level, recovery needs)
- [ ] Spatial requirements (if any)
- [ ] System function requirements sketched

---

### Level 3: Temporal Architecture

**Questions to answer:**
- [ ] How long is a complete play session?
- [ ] What loops exist? (Micro, meso, macro, meta)
- [ ] What are loop durations?
- [ ] How do loops relate?
- [ ] Where are natural stopping points?
- [ ] What pacing pattern? (Escalating, steady-state, episodic, wave)
- [ ] What content scale does this require?

**Outputs:**
- [ ] Session duration targets
- [ ] Loop structure with specific durations
- [ ] Pacing pattern selected
- [ ] Stopping point locations
- [ ] Content scale requirements derived

---

### Level 4: Balance Paradigm

**Questions to answer:**
- [ ] Which paradigm? (Consistency, Framework, Adaptive, Hybrid)
- [ ] Why this paradigm for this aesthetic?
- [ ] How are edge cases handled?
- [ ] If Framework: What triggers mechanics vs. judgment?
- [ ] If Adaptive: What does system observe? How does it respond?
- [ ] If Hybrid: Where are paradigm boundaries?

**Outputs:**
- [ ] Paradigm selected with rationale
- [ ] Edge case handling approach
- [ ] For Framework: Mechanic/judgment triggers specified
- [ ] For Adaptive: Observation and response rules
- [ ] LLM integration implications noted (see Ch. 8)

---

### Level 5: Mechanical Specification

**Questions to answer:**
- [ ] What core verbs does the game require?
- [ ] What mechanical alternatives were considered?
- [ ] What are core mechanics?
- [ ] What resources exist? What function does each serve?
- [ ] What scarcity and recovery patterns?
- [ ] How is content generated? (Procedural, authored, hybrid)
- [ ] What content categories and quantities?
- [ ] What safety mechanics (if applicable)?

**Outputs:**
- [ ] Core mechanics selected with rationale
- [ ] 2-3 alternatives documented with evaluation
- [ ] Resource system designed (functions, types, scarcity, recovery)
- [ ] Content requirements listed
- [ ] Safety mechanics specified (if applicable)
- [ ] Cognitive fit verified against budget

---

### Level 6: Presentation Architecture

**Questions to answer:**
- [ ] ADJUDICATION: How are outcomes determined and communicated?
- [ ] INFORMATION: What do players know? When do they learn it?
- [ ] CONTENT: How is content delivered and paced?
- [ ] PERSISTENCE: What does the game remember?
- [ ] FEEDBACK: How does the game signal what's happening?
- [ ] FRAMING: How do players learn and understand?

**Outputs:**
- [ ] All six system functions specified
- [ ] Information budget verified against player profile
- [ ] Feedback timing matched to aesthetic
- [ ] Tutorial/onboarding approach determined

---

### Level 7: Parameters

**Questions to answer:**
- [ ] What measurable targets exist for each system?
- [ ] What constraints do targets impose?
- [ ] What specific values satisfy constraints?
- [ ] How do values interact across systems?

**Outputs:**
- [ ] All key parameters specified
- [ ] Each parameter traceable to measurable target
- [ ] Each target traceable to dynamic/aesthetic
- [ ] Initial values ready for playtesting

---

## Entry Point Flowchart

```
START: What sparked this project?

"I want players to feel ___"
    → AESTHETIC-FIRST
    → Go directly to Level 1
    → Proceed down chain

"I have these constraints: ___"
    → CONSTRAINT-FIRST  
    → Fill Level 0
    → Derive achievable aesthetics at Level 1
    → Proceed down chain

"I want to explore this theme: ___"
    → THEME-FIRST
    → Theme informs Setting (Level 0)
    → Theme suggests Aesthetic (Level 1)
    → Proceed down chain

"I have this cool mechanic: ___"
    → MECHANIC-FIRST
    → Work BACKWARD: What dynamics does this create?
    → What aesthetic do those dynamics serve?
    → If coherent: proceed from aesthetic
    → If incoherent: set mechanic aside or find fitting aesthetic

"I want to use LLM in my game"
    → CAPABILITY-FIRST
    → Ask: What does this enable that wasn't practical?
    → Convert to aesthetic goal
    → Proceed as aesthetic-first
    → See Chapter 8 for LLM specifics
```

---

## Coherence Audit Template

Use between levels or when design feels wrong.

| Check | Question | Pass/Fail | Notes |
|-------|----------|-----------|-------|
| 0→1 | Does aesthetic serve the player profile from context? | | |
| 1→2 | Do these dynamics actually create the target aesthetic? | | |
| 2→3 | Does temporal structure support required dynamics? | | |
| 3→4 | Does paradigm enable dynamics within temporal structure? | | |
| 4→5 | Do mechanics implement paradigm and create dynamics? | | |
| 5→6 | Does presentation serve aesthetic and fit cognitive budget? | | |
| 6→7 | Do parameters tune systems to hit measurable targets? | | |

**If any check fails:** The problem is at that transition. Don't proceed until resolved.

---

## Decision Matrices

These matrices encode relationships established throughout the book. They're lookup tools, not substitutes for understanding the underlying principles.

### Matrix 1: Aesthetic → Primary Dynamics

For each aesthetic, what dynamics must emerge for the aesthetic to land?

| Aesthetic | Core Loop Dynamic | Peak Moment Dynamic | Anti-Dynamics |
|-----------|------------------|--------------------|--------------------|
| **Challenge** | Attempt, fail, learn, retry | Triumph after struggle | Trivial success, unfair failure, grind bypass |
| **Discovery** | Explore, observe, theorize, verify | Revelation / "aha!" moment | Empty world, obvious information, arbitrary secrets |
| **Mastery** | Experiment, observe, optimize | Elegant solution / efficiency breakthrough | Shallow systems, solved optimal, execution gates |
| **Tension** | Assess threat, commit, experience uncertainty | Close call / narrow escape | Safety, hopelessness, predictability |
| **Expression** | Create, modify, share | Satisfaction with creation | Constrained options, judgment, meaningless choices |
| **Fellowship** | Communicate, coordinate, share experience | Shared triumph or experience | Isolation, competition undermining cooperation |
| **Submission** | Engage in pleasant activity | Flow state / absorption | Stress, punishment, forced attention, time pressure |
| **Progression** | Acquire, grow, advance | Power spike / new capability | Stagnation, cap reached too early |
| **Narrative** | Engage with story, make choices | Emotional story beats | Disconnection, meaningless choices, broken immersion |

**Usage:** After defining your aesthetic target (Level 1), use this matrix to derive required dynamics (Level 2).

---

### Matrix 2: Aesthetic → Temporal Architecture Tendencies

| Aesthetic | Micro Loop | Meso Loop | Pacing Pattern | Stopping Points |
|-----------|-----------|-----------|----------------|-----------------|
| **Challenge** | Quick attempts (sec-2min) | Encounter/level (10-30min) | Escalating | After meso completion |
| **Discovery** | Observation (sec-1min) | Area/mystery (15-60min) | Episodic | After revelations |
| **Mastery** | Single decision (variable) | Strategy test (30-90min) | Steady-state | After runs |
| **Tension** | Threat response (seconds) | Encounter sequence (15-45min) | Escalating with valleys | After release moments |
| **Fellowship** | Communication beat (seconds) | Shared activity (30-90min) | Variable (group-driven) | Natural group breaks |
| **Submission** | Rhythmic action (seconds) | Short session (5-15min) | Steady-state | Very frequent, anywhere |
| **Progression** | Gain increment (sec-min) | Milestone (5-30min) | Steady or stepped | After milestones |
| **Narrative** | Story beat (min) | Scene/chapter (15-60min) | Narrative arc | Between scenes/chapters |

**Usage:** After defining dynamics (Level 2), use this matrix to inform temporal architecture decisions (Level 3).

---

### Matrix 3: Aesthetic → Balance Paradigm

| Aesthetic | Primary Paradigm | Why | Secondary Options |
|-----------|-----------------|-----|-------------------|
| **Challenge** | Consistency | Pattern learning requires predictability | Adaptive (difficulty scaling) |
| **Discovery** | Framework or Consistency | Framework for narrative discovery; Consistency for systemic | — |
| **Mastery** | Consistency | Optimization requires deterministic systems | — |
| **Tension** | Adaptive | Maintained tension requires adjustment | Consistency (if carefully calibrated) |
| **Fellowship** | Framework | Human dynamics need flexibility | Consistency (for competitive) |
| **Submission** | Adaptive | Protected flow requires adjustment | Consistency (very forgiving) |
| **Progression** | Consistency | Progression legibility requires predictable advancement | Adaptive (difficulty scaling) |
| **Narrative** | Framework | Story needs flexibility over mechanical precision | Consistency (mechanics supporting narrative) |

**Usage:** After determining temporal architecture (Level 3), use this matrix to select balance paradigm (Level 4).

---

### Matrix 4: Player Profile → Constraints

| Parameter | Casual | Midcore | Hardcore |
|-----------|--------|---------|----------|
| **Session Length** | 5-30 minutes | 30-90 minutes | 2+ hours |
| **Micro Loop Duration** | Seconds to 1 minute | Seconds to 2 minutes | Variable (up to 5+ min) |
| **Meso Loop Duration** | 5-15 minutes | 15-45 minutes | 30-90 minutes |
| **Stopping Point Frequency** | Every 5-15 minutes | Every 30-60 minutes | Every 1-2 hours acceptable |
| **Cognitive Load Ceiling** | 3±2 tracked elements | 5-7 systems | 8-15+ elements |
| **Decision Complexity** | Simple, intuitive | Moderate, learnable | Complex, mastery-rewarding |

**Usage:** Use throughout derivation to verify decisions fit target player profile.

---

### Matrix 5: Resource Functions

| Function | Purpose | Examples | Serves Aesthetic |
|----------|---------|----------|------------------|
| **Limiter** | Constrain what players can do | Health, ammo, action points | Challenge, Tension |
| **Currency** | Create trade-off decisions | Gold, XP, crafting materials | Mastery, Progression |
| **Tracker** | Show progress without scarcity | Quest completion, relationship levels | Discovery, Narrative |
| **Meta-resource** | Create long-term investment | Unlocks, permanent upgrades | Progression |

**Usage:** At Level 5, identify which resource functions your aesthetic requires, then design resources to fill those functions.

---

### Matrix 6: Medium → Constraints

| Constraint | Video Game | Board Game | TTRPG | Mobile |
|------------|-----------|-----------|-------|--------|
| **Real-time possible** | Yes | Limited (timers) | No | Yes |
| **Hidden information** | Complete | Partial | Complete (GM) | Complete |
| **State tracking** | Automated | Manual (limited) | Manual or GM | Automated |
| **Complexity ceiling** | Very high | Moderate | Moderate (GM-dependent) | Low-moderate |
| **Content volume needed** | High | Low-moderate | Low (GM generates) | Moderate |
| **Framework paradigm viable** | With AI/LLM only | Possible | Native | With AI/LLM only |
| **Adaptive paradigm viable** | Yes | Difficult | Yes (GM) | Yes |

**Usage:** Consult when establishing context (Level 0) and throughout design.

---

### Matrix 7: Archetype → Inherited Commitments (Summary)

| Archetype | Temporal | Mechanical | Aesthetic Affinity | Cognitive |
|-----------|----------|------------|-------------------|-----------|
| **Roguelike** | Run-based macro, escalating | Permadeath, procedural, builds | Challenge, Mastery | Midcore-hardcore |
| **Puzzle** | Single puzzle meso | Deterministic, clear solution | Challenge, Mastery | Variable |
| **4X** | Very long macro, turn-based | Interlocking systems, territory | Mastery, Challenge | Hardcore |
| **Metroidvania** | Ability-gated exploration | Interconnected map, ability gates | Discovery, Challenge | Midcore |
| **Idle/Incremental** | Prestige macro, passive | Exponential growth, automation | Progression, Submission | Casual-midcore |
| **Campaign TTRPG** | Multi-session macro, scene micro | Character persistence, GM | Narrative, Fellowship | Midcore-hardcore |
| **One-Shot TTRPG** | Single session macro | Contained scenario | Variable | Variable |
| **Euro Board Game** | Single session macro | Resource conversion, VP | Mastery, Challenge | Midcore-hardcore |
| **Cooperative Board** | Single session, escalating | Shared win/loss, roles | Fellowship, Challenge | Midcore |

**Usage:** When choosing archetype (Level 0), review commitments. See Archetype Library supplementary for full profiles.

---

## Symptom-to-Level Diagnostic

When playtesting reveals problems, use this guide to locate the cause.

| Symptom | Likely Level | Investigation |
|---------|--------------|---------------|
| "Not fun" (vague) | Level 1 | Aesthetic unclear—what experience should it be? |
| Wrong emotion emerges | Level 2 | Dynamics not producing aesthetic—check behaviors |
| "Too easy" or "Too hard" | Level 7 | Parameters—adjust numbers first |
| "Confusing" | Level 6 | Presentation—check information, feedback, framing |
| "Overwhelming" | Level 1, 5, or 6 | Cognitive load—reduce complexity or improve presentation |
| Pacing feels off | Level 3 | Temporal—check loop durations, stopping points |
| "Unfair" | Level 4 or 6 | Paradigm or presentation—check consistency, visibility |
| Exploits / dominant strategies | Level 5 | Mechanics—redesign systems |
| Players don't do expected things | Level 2 or 5 | Dynamics or mechanics—check if systems enable behaviors |
| "Feels random" (Consistency game) | Level 4 or 6 | Hidden randomness—make rules transparent |
| "Feels arbitrary" (Framework game) | Level 4 or 6 | Inconsistent rulings—document precedents |
| "Feels manipulated" (Adaptive game) | Level 4 | Adaptation too visible—smooth adjustments |

**Diagnostic principle:** Start at lowest level that could cause the symptom. Work upward only if lower-level fixes don't resolve it.

---

## Iteration Documentation Template

Track changes systematically to build institutional memory.

### Iteration Record

**Date:** _______________

**Playtest context:** (Who played, how long, what version)

---

**Observation:** What actually happened?

---

**Hypothesis:** What we thought would happen vs. what did happen

---

**Diagnosis:** What level is the problem?

| Level | Could this be the cause? | Evidence |
|-------|--------------------------|----------|
| 7 (Parameters) | | |
| 6 (Presentation) | | |
| 5 (Mechanics) | | |
| 4 (Paradigm) | | |
| 3 (Temporal) | | |
| 2 (Dynamics) | | |
| 1 (Aesthetic) | | |

**Identified level:** _______________

---

**Adjustment:** What we changed

---

**Rationale:** Why this change should fix the problem

---

**Result:** Did it work?

- [ ] Fixed—move on
- [ ] Improved but not fixed—continue same direction
- [ ] Made worse—revert and try different approach
- [ ] No change—diagnosis was wrong, re-diagnose

---

**Lessons:** What did we learn for future iterations?

---

## System Functions Reference

Six functions every game must fulfill. Use when specifying Level 6.

### 1. Adjudication

How outcomes are determined and communicated.

| Option | Description | Serves |
|--------|-------------|--------|
| Transparent | Visible percentages, clear calculation | Challenge, Mastery |
| Opaque | Outcomes without visible math | Narrative, Tension |
| Delayed | Action now, outcome later | Tension, Discovery |
| Deterministic | No randomness, pure skill | Challenge |
| Probabilistic | Dice/random elements | Tension, variety |

### 2. Information Management

What players know and when.

| Option | Description | Serves |
|--------|-------------|--------|
| Full transparency | Everything visible | Mastery, optimization |
| Selective | Some visible, some hidden | Discovery, Tension |
| Minimal | Revealed through play | Discovery, Challenge |
| Pushed | Game tells you what matters | Casual players |
| Pulled | Player must seek information | Hardcore players |

### 3. Content Generation

How content is delivered.

| Option | Description | Serves |
|--------|-------------|--------|
| Dense frontloaded | Most content visible quickly | Challenge (fast learning) |
| Sparse gated | Unlocks over time | Discovery, Progression |
| Responsive | Content varies by player state | Narrative, Adaptive |
| Procedural | Generated each time | Replayability |
| Authored | Hand-crafted, fixed | Precision, narrative control |

### 4. State Persistence

What the game remembers.

| Option | Description | Serves |
|--------|-------------|--------|
| Total | Everything forever | Narrative (permanent weight) |
| Selective | Some persists, some resets | Progression + fresh challenge |
| Fading | Information decays | Realism, anti-optimization |
| None | Each session fresh | Challenge (pure skill) |

### 5. Feedback

How the game signals what's happening.

| Option | Description | Serves |
|--------|-------------|--------|
| Immediate | Instant response to action | Action games, Challenge |
| Delayed | Response after interval | Tension, contemplation |
| Punchy | Screen shake, particles, sound | Satisfaction, action feel |
| Subtle | Minimal sensory feedback | Atmosphere, realism |
| Ambient | Environmental changes | Immersion |

### 6. Cognitive Framing

How players learn and understand.

| Option | Description | Serves |
|--------|-------------|--------|
| Tutorial | Explicit instruction | Accessibility |
| Learning by doing | First levels teach | Immersion, respect for player |
| Tooltips on demand | Information when requested | Balance of help/flow |
| Contextual hints | Help appears when struggling | Casual players |
| Documentation | External reference | Hardcore, complex systems |

---

## Using This Document

**Matrices are maps, not territories.** They summarize patterns observed across many games. Your specific design may have good reasons to diverge.

**Cross-reference matrices.** A single decision often requires consulting multiple matrices. Designing resources? Check Matrix 5 (resource functions) AND Matrix 4 (player profile constraints) AND the Resource Specification Process in Chapter 7.

**When matrices conflict with your instinct, investigate.** Either your instinct is catching something the matrix misses, or the matrix is surfacing something your instinct overlooked. Both are valuable signals.

**Return to chapters for understanding.** This document provides lookup tools. The main chapters provide conceptual foundations. If a matrix entry is unclear, read the relevant chapter.

---

*This supplementary material is reference documentation. Return to the main Chapter 7 text for conceptual understanding and worked examples.*
