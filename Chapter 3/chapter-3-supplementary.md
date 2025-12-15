# Chapter 3 Supplementary Material: Resources Quick Reference

This supplementary material accompanies Chapter 3 (Resources). Use it as a reference during design work, after you've internalized the core concepts from the main chapter.

## What's In This Document

| Section | What You'll Find | Use When... |
|---------|------------------|-------------|
| **Resource Functions Reference** | Table of four functions (Limiter, Currency, Tracker, Meta-resource) with purposes and examples | Deciding what type of resource to create |
| **Function-Aesthetic Alignment** | Matrix showing which functions serve which aesthetics | Checking if your resource choices match your target experience |
| **Behavior Patterns Reference** | Table of five patterns (Consumable, Buffer, etc.) with cognitive load ratings | Choosing how a resource should behave mechanically |
| **Recovery Speed Effects** | How recovery rate affects player behavior and pacing | Tuning resource recovery for desired pacing |
| **Scarcity Levels Reference** | Four scarcity levels with appropriate aesthetics | Setting resource abundance/scarcity |
| **Resource-Aesthetic Configuration** | Detailed resource sets for each aesthetic (Challenge, Discovery, etc.) | Designing complete resource systems for your aesthetic |
| **Archetype-Resource Mapping** | Which resources work for which archetypes | Quick lookup when you know your archetype |
| **Resource Design Checklist** | Step-by-step validation checklist | Final review before implementation |
| **Validated Design Patterns** | Proven patterns like Separated Concerns, Dynamic Recovery | Looking for tested solutions to common problems |
| **Common Anti-Patterns** | What to avoid and how to fix it | Diagnosing resource system problems |
| **Loop Scale Resource Distribution** | Resources by temporal scale (micro/meso/macro/meta) | Designing multi-scale resource systems |

---

## Resource Functions Reference

| Function | Purpose | Core Dynamic | Examples |
|----------|---------|--------------|----------|
| **Limiter** | Constrain actions, create pressure | "Can I afford this?" | HP, action points, ammunition, time limits |
| **Currency** | Enable trade-offs, create allocation decisions | "Buy this or that?" | Gold, XP, skill points, crafting materials |
| **Tracker** | Show progress, communicate state | "How far along?" | Quest markers, map %, collection progress |
| **Meta-resource** | Span sessions, create long-term decisions | "Which permanent upgrade?" | Hades Darkness, Rogue Legacy gold |

### Function-Aesthetic Alignment

| Function | Challenge | Tension | Submission | Mastery | Discovery | Progression |
|----------|-----------|---------|------------|---------|-----------|-------------|
| Limiter | ✔✔ | ✔✔ | ✗ | ✔ | ~ | ~ |
| Currency | ✔✔ | ~ | ✔ | ✔✔ | ~ | ✔✔ |
| Tracker | ~ | ~ | ✔✔ | ~ | ✔✔ | ✔✔ |
| Meta-resource | ✔ | ~ | ✔ | ✔✔ | ✔ | ✔✔ |

Key: ✔✔ = Excellent fit, ✔ = Works well, ~ = Depends on implementation, ✗ = Usually conflicts

---

## Behavior Patterns Reference

| Pattern | Behavior | Core Dynamic | Cognitive Load |
|---------|----------|--------------|----------------|
| **Consumable** | Depletes, must replenish | "Spend now or save?" | Moderate |
| **Buffer** | Absorbs costs, protects | "How much margin?" | Low-Moderate |
| **Accumulation** | Primarily increases | "Progress through growth" | Low |
| **Composition** | Combination matters | "Curation over collection" | High |
| **Capacity** | Gates other systems | "What fits within limits?" | Moderate-High |

### Recovery Speed Effects

| Recovery | Player Behavior | Pacing Pattern | Best For |
|----------|-----------------|----------------|----------|
| **None** | Extreme conservation | Maximum tension | Horror, permadeath roguelikes |
| **Slow** | Attrition management | Strategic retreat cycles | Old-school RPGs, survival |
| **Moderate** | Episodic spending | Self-contained segments | Modern roguelikes, mission-based |
| **Fast** | Aggressive expenditure | Constant forward pressure | Action games, DOOM-style |

---

## Scarcity Levels Reference

| Level | Description | Player Experience | Appropriate Aesthetics |
|-------|-------------|-------------------|------------------------|
| **Extreme** | Always running out | Constant anxiety, desperation | Tension, Horror |
| **Strategic** | Meaningful trade-offs | Careful planning required | Challenge, Mastery |
| **Comfortable** | Usually enough | Light optimization | Discovery, Narrative |
| **Abundant** | Always enough | No resource stress | Submission, Cozy |

---

## Resource-Aesthetic Configuration

### Challenge Aesthetic

**Resource requirements:**
- Strategic scarcity (not extreme, not abundant)
- Multiple competing demands (opportunity cost)
- Consequences for poor management

**Typical resource set:**
- 2-3 Limiters (HP, action points, time)
- 1-2 Currencies (upgrade choices)
- Usually NOT Trackers (tracking doesn't create challenge)

**Example - XCOM 2:**
- Action points: 2 per turn, choose move vs. shoot vs. ability
- Soldier health: Injury consequences, manage risk
- Resources: Limited materials, must prioritize equipment

### Discovery Aesthetic

**Resource requirements:**
- Trackers showing what's been found
- Light resource management (don't distract)
- Currencies only if unlocking new areas

**Typical resource set:**
- 1-3 Trackers (completion %, collectibles)
- 0-1 Limiters (mild, like stamina)
- 1 Currency if needed for gates

**Example - Outer Wilds:**
- Knowledge tracker (ship log)
- NO resource management
- Pure Discovery, resources would distract

### Tension Aesthetic

**Resource requirements:**
- Strategic to extreme scarcity
- Constant worry about running out
- Consequences feel threatening

**Typical resource set:**
- 2-3 scarce Limiters (ammunition, health, sanity)
- Light or no Currencies
- Trackers for investigation progress (if horror-investigation)

**Example - Resident Evil:**
- Ammunition: Always insufficient
- Health items: Scarce, must ration
- Inventory: Tight capacity forces choices

### Submission Aesthetic

**Resource requirements:**
- Abundant or auto-managing
- No harsh penalties
- Trackers for satisfaction, not stress

**Typical resource set:**
- 1-2 generous Limiters (if any)
- 1-3 Trackers (collection, completion)
- 0-1 abundant Currency

**Example - Animal Crossing:**
- Bells: Abundant, can buy what you want
- Collection trackers: Fish, bugs, fossils
- No scarcity-driven decisions

### Mastery Aesthetic

**Resource requirements:**
- Complex systems with interactions
- Composition resources (build optimization)
- Deep optimization potential

**Typical resource set:**
- 4-6 resources (higher complexity appropriate)
- Composition resources essential
- Currencies for progression
- Limiters for optimization challenges

**Example - Slay the Spire:**
- Deck: Core composition puzzle
- Energy: Constrains plays per turn
- Relics: Build modifiers
- Gold: Acquisition choices

### Narrative Aesthetic

**Resource requirements:**
- Minimal tracking (don't distract from story)
- Resources that tell story when present
- Avoid optimization gameplay

**Typical resource set:**
- 0-2 Trackers (relationship, story progress)
- 0-1 Light Limiter (if creates narrative tension)
- NO complex management

**Example - Disco Elysium:**
- Health/Morale: Extremely generous
- Skill points: Minimal (level-up only)
- Resources nearly invisible, story primary

### Fellowship Aesthetic

**Resource requirements:**
- Shared resources (creates cooperation) OR simple individual (avoids bookkeeping)
- Clear, easy-to-communicate state

**Typical resource set (shared):**
- 2-3 shared Limiters (party pool)
- 1-2 shared Currencies

**Typical resource set (individual):**
- 1-2 simple individual Limiters
- Avoid individual Composition (too much load during social play)

---

## Archetype-Resource Mapping

| Archetype | Primary Functions | Scarcity Level | Key Resources |
|-----------|-------------------|----------------|---------------|
| **Horror Investigation** | Limiter + Tracker | Extreme-Strategic | Ammunition, sanity, evidence |
| **Mystery Investigation** | Tracker | Comfortable | Clues, theories, relationships |
| **Tactical Combat** | Limiter + Currency | Strategic | Action points, equipment, abilities |
| **Roguelike** | All (multi-scale) | Varies by scale | Micro/meso/macro/meta resources |
| **Cozy Simulation** | Tracker + Currency | Abundant | Collections, currency, progress |
| **4X Strategy** | Limiter + Currency + Composition | Strategic | Yields, units, tech, diplomacy |
| **Survival** | Limiter | Strategic-Extreme | Health, hunger, materials |

---

## Resource Design Checklist

### Initial Design

- [ ] Primary aesthetic identified (Chapter 1)
- [ ] Archetype chosen (Chapter 2)
- [ ] Required functions determined (Limiter? Currency? Tracker? Meta?)
- [ ] Behavior patterns selected (Consumable? Buffer? Accumulation? Composition? Capacity?)

### Configuration

- [ ] Scarcity level matches aesthetic
- [ ] Recovery speed creates intended pacing
- [ ] Multiple competing demands exist (opportunity cost)
- [ ] Resources don't create false choices

### Validation

- [ ] Cognitive load appropriate for audience
- [ ] Total resource count manageable (2-4 casual, 4-6 hardcore)
- [ ] Each resource passes "remove and test" check
- [ ] Configuration coherent (all resources serve same aesthetic)

---

## Validated Design Patterns

### Separated Concerns (Blades in the Dark)

**Pattern:** Separate fast-recovering buffer from slow-recovering consequences
- Stress (fast) vs. Harm (slow)
- Creates agency: choose which to suffer
- Adds depth without excessive complexity

### Dynamic Recovery (Left 4 Dead AI Director)

**Pattern:** Adjust resource availability based on performance
- Struggling players get more pickups
- Skilled players get less support
- Maintains appropriate challenge level

### Opportunity Cost Economy (Civilization gold)

**Pattern:** Single currency, multiple valuable uses
- Can't afford everything, must prioritize
- Creates decisions without tracking complexity
- More engaging than multiple currencies

### Risk/Reward Accumulation (Dark Souls souls)

**Pattern:** Valuable currency that can be lost
- Creates greed-driven overextension
- Loss feels like player's fault
- Generates memorable moments

### Regenerating Capacity (Slay the Spire potions)

**Pattern:** Limited slots force using old to get new
- Can't hoard indefinitely
- Encourages tactical use
- Prevents "save for boss" problem

---

## Common Anti-Patterns

| Anti-Pattern | Problem | Solution |
|--------------|---------|----------|
| Too many resources | Cognitive overload | Remove lowest-value resources |
| Single-use resources | Calculation, not strategy | Add competing demands |
| Broken economy | Abundance removes decisions | Reduce acquisition or add sinks |
| Progress-blocking scarcity | Frustration, not challenge | Add fallback acquisition paths |
| Hidden resource state | Can't make informed decisions | Show resource information clearly |
| Incoherent scarcity | Tense game with abundant resources | Match scarcity to aesthetic |

---

## Loop Scale Resource Distribution

| Scale | Duration | Resource Types | Recovery |
|-------|----------|----------------|----------|
| **Micro** | Seconds-minutes | Cooldowns, energy, per-action | Per-action or instant |
| **Meso** | Minutes-30min | HP per encounter, spell slots | Per-encounter or rest |
| **Macro** | Session-run | XP, campaign resources | Per-session or run completion |
| **Meta** | Between sessions | Permanent unlocks, collection | Persistent |

**Example - Hades resource architecture:**
- Micro: Health per room (fast visibility)
- Meso: Boons per run (build composition)
- Macro: Darkness per run (currency for meta)
- Meta: Mirror talents, unlocked weapons (permanent)

---

*This supplementary material is reference documentation. Return to the main Chapter 3 text for conceptual understanding and narrative examples.*
