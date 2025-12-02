# Chapter 4 Supplementary Material: Cognitive Load Quick Reference

This supplementary material accompanies Chapter 4 (Cognitive Load). Use it as a reference during design work, after you've internalized the core concepts from the main chapter.

## What's In This Document

| Section | What You'll Find | Use When... |
|---------|------------------|-------------|
| **Load Type Reference** | Tracking, Decision, Execution definitions and indicators | Diagnosing which load type is problematic |
| **Load Level Examples** | Games at each load level for each type | Calibrating your design against known examples |
| **Archetype-Load Matrix** | Complete profile for each archetype | Checking if your archetype fits audience capacity |
| **Budget Allocation by Aesthetic** | Where to spend cognitive budget for each aesthetic | Planning load distribution |
| **Load Source Reference** | Five sources with cognitive costs | Identifying where load is coming from |
| **Observable Behavior Indicators** | What to watch for in playtesting | Validating load during testing |
| **Load Reduction Checklist** | When to use each reduction strategy | Fixing load problems |
| **Investment Trajectory Patterns** | How load changes over player lifetime | Designing onboarding and mastery curves |

---

## Load Type Reference

### Tracking Load

**Definition:** Mental effort to remember and monitor current game state.

**What players track:**
- Resource values (health, mana, ammunition, gold)
- Status effects (buffs, debuffs, timers, cooldowns)
- Positions (unit locations, enemy positions, waypoints)
- Progress states (quest objectives, collectibles, areas explored)
- Relationships (faction standings, NPC opinions)

**Observable indicators:**

| Level | Behavior | Example Games |
|-------|----------|---------------|
| Very Low | Instant understanding, no UI dependence | *Untitled Goose Game*, *Journey* |
| Low | Brief UI glances, easy resumption | *DOOM (2016)*, *Mario Odyssey* |
| Medium | Occasional checking, brief reorientation | *Slay the Spire*, *Hades* |
| High | Frequent checking, note-taking | *Crusader Kings 3*, *Civilization VI* |
| Very High | External tools required, constant reference | *Dwarf Fortress*, *Path of Exile* |

### Decision Load

**Definition:** Mental effort to evaluate options and choose actions.

**What creates it:**
- Number of options (action space size)
- Evaluation complexity (calculations required)
- Interdependencies (combo effects, synergies)
- Hidden information (uncertainty)
- Irreversibility (permanent consequences)

**Observable indicators:**

| Level | Behavior | Example Games |
|-------|----------|---------------|
| Very Low | Instant choices, no analysis | *Vampire Survivors*, *Cookie Clicker* |
| Low | Quick decisions, clear preferences | *Animal Crossing*, *Stardew Valley* |
| Medium | Brief consideration, occasional tough calls | *Hades*, *Slay the Spire* |
| High | Frequent pauses, careful analysis | *XCOM 2*, *Gloomhaven* |
| Very High | Extended deliberation, may use tools | *Chess*, *Go*, *Competitive card games* |

### Execution Load

**Definition:** Mental effort to physically perform actions correctly.

**What creates it:**
- Timing requirements (precision windows)
- Coordination demands (simultaneous inputs)
- Reaction speed (responding to stimuli)
- Physical skill (muscle memory, APM)
- Spatial reasoning (3D positioning, aiming)

**Observable indicators:**

| Level | Behavior | Example Games |
|-------|----------|---------------|
| Very Low | Actions always succeed when intended | *Visual novels*, *Turn-based RPGs* |
| Low | Simple inputs, forgiving timing | *Animal Crossing*, *Pokémon* |
| Medium | Some precision needed, moderate timing | *Hades*, *Zelda games* |
| High | Tight timing, complex inputs | *Dark Souls*, *Monster Hunter* |
| Very High | Frame-perfect execution, extreme APM | *Fighting games*, *StarCraft*, *Celeste* |

---

## Archetype-Load Matrix

| Archetype | Tracking | Decision | Execution | Total | Primary Aesthetics |
|-----------|----------|----------|-----------|-------|-------------------|
| Investigation | High | Medium | Low | High | Discovery, Mastery |
| Tactical Combat | Medium | High | Low | High | Challenge, Mastery |
| Real-time Action | Low | Low | High | Medium | Challenge, Tension |
| 4X Strategy | Very High | Very High | Low | Very High | Mastery, Progression |
| Puzzle | Low | Very High | Low | Medium | Challenge |
| Cozy Simulation | Low | Low | Low | Low | Submission, Expression |
| Roguelike | Medium | High | Medium | High | Challenge, Mastery, Progression |
| Horror Survival | Medium | Medium | Medium | Medium | Tension, Challenge |
| Walking Simulator | Low | Low | Low | Low | Narrative, Discovery |
| Social Deduction | Medium | Very High | Low | High | Fellowship, Competition |
| MOBA | High | High | Very High | Very High | Competition, Mastery |
| Metroidvania | Medium | Medium | Medium | Medium | Discovery, Progression |
| Survival | High | Medium | Medium | High | Challenge, Tension |
| Fighting Game | Low | High | Very High | Very High | Challenge, Mastery |
| Deck Builder | Medium | Very High | Low | High | Mastery, Challenge |

### Using the Matrix

1. Find your archetype (from Chapter 2)
2. Check total load against audience capacity:
   - Low = Casual appropriate
   - Medium = Midcore appropriate
   - High = Midcore to Hardcore
   - Very High = Hardcore only
3. If mismatch: change archetype or change target audience
4. Design within the archetype's natural profile

---

## Budget Allocation by Aesthetic

### Challenge Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 60% | Execution or decision IS the challenge |
| Resource management | 20% | Scarcity creates meaningful choices |
| Goal tracking | 10% | Clear objectives |
| Context/meta | 10% | Minimal—focus on challenge |

### Mastery Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 40% | Deep interactions to master |
| Resource management | 30% | Optimization space |
| Goal tracking | 10% | Clear but complex goals |
| Context/meta | 20% | Long-term mastery systems |

### Discovery Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 40% | Exploration mechanics |
| Resource management | 10% | Not the focus |
| Goal tracking | 20% | What's left to find? |
| Context | 30% | World richness matters |

### Submission Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 70% | The relaxing activity itself |
| Resource management | 10% | Abundant, not stressful |
| Goal tracking | 10% | Simple, clear |
| Context | 10% | Simple framing |

### Fellowship Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 40% | Shared activity |
| Resource management | 10% | Simple or shared |
| Goal tracking | 10% | Team objectives |
| Context | 10% | Shared understanding |
| Social/communication | 30% | Coordination is key |

### Narrative Aesthetic

| Source | Allocation | Rationale |
|--------|------------|-----------|
| Core mechanic | 30% | Story delivery mechanics |
| Resource management | 10% | Minimal management |
| Goal tracking | 20% | Story progress |
| Context | 40% | World and character depth |

---

## Load Source Reference

### Source 1: Core Mechanic

**What it creates:** Varies by mechanic type
**Budget priority:** Highest—this is where aesthetic payoff lives

| Mechanic Type | Primary Load | Secondary Load |
|---------------|--------------|----------------|
| Investigation | Tracking | Decision |
| Tactical | Decision | Tracking |
| Action/Reflex | Execution | — |
| Puzzle | Decision | — |
| Exploration | Tracking | — |
| Social | Decision | Tracking |

### Source 2: Resource Management

**What it creates:** Tracking + Decision load
**Budget impact:** Scales with resource count and complexity

| Resource Count | Audience | Cognitive Cost |
|----------------|----------|----------------|
| 1-2 | Casual | Very Low |
| 3-4 | Casual-Midcore | Low |
| 5-7 | Midcore | Medium |
| 8-12 | Midcore-Hardcore | High |
| 13+ | Hardcore only | Very High |

| Resource Type | Cognitive Cost |
|---------------|----------------|
| Tracker | Very Low |
| Buffer | Low |
| Accumulation | Low |
| Consumable | Medium |
| Capacity | Medium-High |
| Composition | Very High |

### Source 3: Goal Tracking

**What it creates:** Tracking load + minimal Decision load
**Budget impact:** Scales with loop complexity

| Loop Scale | Goal Clarity Needed | Load Level |
|------------|---------------------|------------|
| Micro | Instant | Zero |
| Meso | Visible/trackable | Low |
| Macro | Directional | Medium |
| Meta | Persistent | High |

### Source 4: Context/Meta-Progression

**What it creates:** Tracking load (world) + Decision load (meta choices)

| Context Complexity | Examples | Load Level |
|--------------------|----------|------------|
| Minimal | Tetris, Chess | Zero |
| Low | Mario, simple arcade | Very Low |
| Medium | Hades, most roguelikes | Low-Medium |
| High | Disco Elysium, narrative RPGs | Medium-High |
| Very High | Crusader Kings, Dwarf Fortress | Very High |

### Source 5: Social Coordination

**What it creates:** All three load types
**Budget impact:** Adds 20-40% to total load

| Social Type | Primary Load Added |
|-------------|-------------------|
| Async multiplayer | Low (can think at own pace) |
| Cooperative sync | Medium (coordination) |
| Competitive sync | High (prediction + deception) |
| Team competitive | Very High (coordination + competition) |

---

## Observable Behavior Indicators

### Tracking Load Problems

| Indicator | Severity | What It Means |
|-----------|----------|---------------|
| Occasional UI checking | Normal | Appropriate tracking |
| Frequent UI checking | Moderate | Approaching limit |
| Note-taking | High | Exceeding capacity |
| Lost after breaks | High | Too much to hold |
| External tools required | Very High | Far exceeds capacity |

### Decision Load Problems

| Indicator | Severity | What It Means |
|-----------|----------|---------------|
| Quick confident choices | Normal | Appropriate decision load |
| Occasional pauses | Normal | Meaningful decisions |
| Analysis paralysis | Moderate | Too many/complex options |
| Timer anxiety | High | Can't decide in time |
| Defaulting to guides | High | Overwhelmed |

### Execution Load Problems

| Indicator | Severity | What It Means |
|-----------|----------|---------------|
| Actions succeed as intended | Normal | Appropriate execution |
| Occasional misses | Normal | Skill expression |
| Frequent mechanical errors | Moderate | Timing too tight |
| Physical tension | High | Demands too high |
| Frustration at controls | High | Execution blocking fun |

### Total Load Problems

| Indicator | Severity | What It Means |
|-----------|----------|---------------|
| Flow state achieved | Normal | Load is right |
| "One more run" | Normal | Engaging appropriately |
| Early quit (before core loop) | High | Total overload |
| "Too complicated" feedback | High | Exceeds audience capacity |
| Tutorial abandonment | Very High | Immediate overload |

---

## Load Reduction Checklist

### When to Use Each Strategy

| Strategy | Use When... | Don't Use When... |
|----------|-------------|-------------------|
| **Automation** | Calculations are busywork, not choices | The calculation IS the challenge |
| **Chunking** | Many related elements can group logically | Elements are genuinely distinct |
| **Progressive Disclosure** | Total complexity appropriate, just frontloaded | Core loop needs full system |
| **Offloading** | Depth serves hardcore, basics serve everyone | Casual audience can't use tools |
| **Simplification** | Complexity exceeds aesthetic requirements | Complexity IS the aesthetic |

### Iteration by Load Type

**Tracking too high:**
1. Automate state display (show computed values)
2. Chunk related information (group by category)
3. Simplify (remove least important trackables)
4. Improve UI (clearer information display)

**Decision too high:**
1. Reduce options (fewer meaningful choices)
2. Provide guidance (recommendations, defaults)
3. Make differences clearer (obvious trade-offs)
4. Add undo/preview (reduce consequence anxiety)

**Execution too high:**
1. Widen timing windows
2. Reduce coordination demands
3. Add execution assistance (aim assist, input buffering)
4. Add difficulty/accessibility options

**Total too high:**
1. Progressive disclosure (spread across time)
2. Cut features (remove entire systems)
3. Change audience (maybe this is for hardcore)
4. Simplify across the board

---

## Investment Trajectory Patterns

### Challenge Aesthetic Trajectory

```
Load →
         ┌─────────────
        /
       /
      /
─────┘
     Novice → Intermediate → Expert
```

Load increases as player seeks harder challenges. System reveals complexity as skill grows.

### Mastery Aesthetic Trajectory

```
Load →
              ┌────────
             /
            /
           /
──────────┘
     Novice → Intermediate → Expert
```

Gradual complexity revelation. Expert load much higher than novice. Progressive disclosure essential.

### Submission Aesthetic Trajectory

```
Load →
─────────────────────────
     Novice → Intermediate → Expert
```

Flat trajectory. Load stays low throughout. Routines automate; mastery reduces effort.

### Mixed Aesthetic (Midcore) Trajectory

```
Load →
         ┌───────────
        /
───────┘
     Novice → Intermediate → Expert
```

Initial ramp (learning curve), then plateau. Novices protected; experts have depth available.

---

## Audience Capacity Reference

| Profile | Budget (Units) | Typical Session | Load Tolerance |
|---------|----------------|-----------------|----------------|
| Casual | 3-5 | 10-30 min | Low only |
| Midcore | 5-8 | 30-90 min | Low-Medium |
| Hardcore | 8-15+ | Hours | Any |

**Budget allocation rule:** No single source should exceed 70% of total budget for its load type.

---

*This supplementary material is reference documentation. Return to the main Chapter 4 text for conceptual understanding and narrative examples.*
