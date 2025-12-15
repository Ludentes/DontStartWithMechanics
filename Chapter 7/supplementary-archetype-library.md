# Supplementary Material: Archetype Library

Archetypes are recurring structural patterns in game design—recognizable configurations of temporal architecture, mechanics, and player expectations. Choosing an archetype means inheriting a set of design commitments that have been tested across many games. You can then modify, subvert, or faithfully execute those commitments based on your specific aesthetic goals.

This library covers common archetypes across mediums. For each archetype, we document:

- **Core identity:** What makes this archetype recognizable
- **Temporal commitments:** Loop structure, pacing, session expectations
- **Mechanical expectations:** What players expect the game to include
- **Aesthetic affinities:** Which aesthetics the archetype naturally serves
- **Cognitive profile:** Typical investment level and load distribution
- **Modification notes:** Common ways designers adapt the archetype

Archetypes are starting points, not prisons. Understanding what an archetype commits you to helps you decide what to keep and what to change.

---

## Video Game Archetypes

### Roguelike / Roguelite

**Core identity:** Run-based play with permadeath (or significant run-end consequences), procedural generation, and emergent variety through system interactions.

**Temporal commitments:**
- Macro loop: The "run" (20-90 minutes typically)
- Meso loop: Floor/level/zone completion (5-15 minutes)
- Micro loop: Individual encounters or rooms (seconds to minutes)
- Meta loop (roguelite): Cross-run progression, unlocks
- Pacing: Escalating within run; each run is complete arc
- Stopping points: Between runs (natural); between floors (acceptable)

**Mechanical expectations:**
- Permadeath or run-ending failure state
- Procedural level/encounter generation
- Build variety (different each run)
- Resource management within run
- Escalating difficulty across run
- Some randomness in available options

**Aesthetic affinities:**
- Primary: Challenge (earned success through skill development)
- Secondary: Mastery (system optimization), Discovery (emergent combinations), Tension (risk/reward decisions)

**Cognitive profile:**
- Typically midcore to hardcore
- High decision load (build choices, resource allocation)
- Moderate tracking load (current build state, floor progress)
- Variable execution load (depends on action vs. turn-based)

**Modification notes:**
- "Roguelite" adds meta-progression, softening permadeath's sting but potentially undermining Challenge purity
- Can compress runs for casual audience (10-20 minute runs)
- Can emphasize different secondaries: Narrative roguelikes (Hades), Mastery roguelikes (Slay the Spire), Discovery roguelikes (Noita)

---

### Puzzle Game (Daily/Session)

**Core identity:** Discrete challenges with solutions, minimal or no meta-progression, focus on the solving moment.

**Temporal commitments:**
- Meso loop: Single puzzle (1-15 minutes depending on complexity)
- Micro loop: Individual moves or observations (seconds)
- Macro loop: Often absent; session is one or few puzzles
- Meta loop: Optional progression through difficulty tiers
- Pacing: Each puzzle is complete arc; no inter-puzzle tension required
- Stopping points: After each puzzle (very clean)

**Mechanical expectations:**
- Clear success/failure state
- Deterministic systems (same input → same output)
- No or minimal randomness in puzzle state
- Often: undo or reset capability
- Often: hint system for accessibility

**Aesthetic affinities:**
- Primary: Challenge (solving is triumph) or Mastery (elegant solutions)
- Secondary: Completion (finishing all puzzles), Discovery (understanding the logic)

**Cognitive profile:**
- Highly variable (casual Wordle to hardcore Stephen's Sausage Roll)
- Decision load dominates
- Low tracking load (state visible)
- Minimal execution load

**Modification notes:**
- Daily format creates social/competitive layer (Wordle)
- Meta-progression can add Progression aesthetic but may undermine puzzle purity
- Narrative wrapper can add Narrative aesthetic without changing core loop (The Witness)

---

### 4X Strategy

**Core identity:** Empire building through explore, expand, exploit, exterminate. Long-term strategic planning, complex system interactions, world domination fantasy.

**Temporal commitments:**
- Macro loop: Full game/campaign (many hours, often 4-20+)
- Meso loop: Era or major objective (1-3 hours)
- Micro loop: Individual turn or decision (minutes)
- Meta loop: Often absent or minimal (each game is standalone)
- Pacing: Very long escalation; early exploration → mid expansion → late conflict
- Stopping points: Between turns (acceptable); between sessions requires save system

**Mechanical expectations:**
- Multiple interlocking systems (economy, military, research, diplomacy)
- Map-based territorial control
- Technology/advancement trees
- AI or human opponents
- Victory conditions (multiple paths)
- Deep decision trees with long-term consequences

**Aesthetic affinities:**
- Primary: Mastery (system optimization), Challenge (strategic competition)
- Secondary: Discovery (map exploration), Expression (empire building choices), Completion (victory achievement)

**Cognitive profile:**
- Hardcore
- Very high tracking load (many systems, long-term state)
- Very high decision load (complex, consequential choices)
- Low execution load (turn-based)

**Modification notes:**
- Can streamline for midcore (fewer systems, shorter games)
- Real-time variants (RTS) shift execution load dramatically
- Asymmetric factions add Discovery and replayability
- Narrative campaigns add Narrative aesthetic

---

### Idle / Incremental

**Core identity:** Numbers go up. Progression continues even without active play. Optimization of accumulation systems.

**Temporal commitments:**
- Macro loop: Prestige/reset cycle (hours to days)
- Meso loop: Upgrade milestone (minutes to hours)
- Micro loop: Click or automation tick (seconds)
- Meta loop: Cross-prestige progression
- Pacing: Steady accumulation punctuated by prestige decisions
- Stopping points: Anywhere (game continues without you)

**Mechanical expectations:**
- Exponential growth systems
- Automation (reduce active play over time)
- Prestige/reset mechanics (trade progress for multipliers)
- Multiple currencies/resources
- Upgrade paths with diminishing returns prompting prestige

**Aesthetic affinities:**
- Primary: Progression (watching numbers grow), Completion (milestone achievement)
- Secondary: Mastery (optimal prestige timing), Submission (low-stress engagement)

**Cognitive profile:**
- Casual to midcore
- Low tracking load (game tracks for you)
- Low-moderate decision load (when to prestige, what to upgrade)
- Minimal execution load

**Modification notes:**
- Can add narrative wrapper (Universal Paperclips)
- Can add strategic depth for midcore (Realm Grinder)
- Mobile-native design allows session flexibility
- Ethical considerations around engagement manipulation

---

### Metroidvania

**Core identity:** Exploration-focused action with ability-gated progression. Interconnected world that opens as player gains capabilities.

**Temporal commitments:**
- Macro loop: Full game completion (5-20 hours)
- Meso loop: Area/boss completion or ability acquisition (30-90 minutes)
- Micro loop: Combat encounter or platforming sequence (seconds to minutes)
- Meta loop: Often absent; completion-focused
- Pacing: Gated exploration creates natural rhythm; boss fights as peaks
- Stopping points: After boss defeats, after ability acquisition, at save points

**Mechanical expectations:**
- Interconnected world map
- Ability-gated areas (need double jump to reach X)
- Backtracking with new abilities opens new paths
- Combat system (usually action-based)
- Boss fights as progression gates
- Map/tracking system for explored areas

**Aesthetic affinities:**
- Primary: Discovery (world exploration, secret finding)
- Secondary: Challenge (combat, bosses), Mastery (ability optimization), Completion (100% map)

**Cognitive profile:**
- Midcore
- Moderate tracking load (map awareness, ability inventory)
- Moderate decision load (exploration choices, build choices)
- Moderate-high execution load (action combat)

**Modification notes:**
- Can emphasize different pillars: combat-heavy (Hollow Knight) vs. exploration-heavy (Outer Wilds adjacent)
- Difficulty options expand audience
- Hint systems for accessibility without ruining Discovery

---

### Battle Royale

**Core identity:** Many players enter, one (or one team) wins. Shrinking play area forces confrontation. High stakes, permadeath per match.

**Temporal commitments:**
- Macro loop: Single match (15-30 minutes)
- Meso loop: Zone/circle phase (3-5 minutes)
- Micro loop: Individual engagement (seconds to minutes)
- Meta loop: Ranking, unlocks, seasonal progression
- Pacing: Escalating pressure as zone shrinks; tension builds to final confrontation
- Stopping points: Between matches (very clean)

**Mechanical expectations:**
- Large player count (20-100)
- Shrinking safe zone
- Looting/scavenging for equipment
- Permadeath within match
- Spectating after death (optional)
- Matchmaking system

**Aesthetic affinities:**
- Primary: Tension (survival pressure), Competition (last one standing)
- Secondary: Challenge (combat skill), Discovery (map knowledge)

**Cognitive profile:**
- Midcore to hardcore
- High tracking load (zone, enemy positions, inventory)
- High decision load (positioning, engagement choices)
- High execution load (shooter or action combat)

**Modification notes:**
- Team variants change social dynamics
- Respawn mechanics (Apex) soften permadeath
- Extraction variants (Tarkov-adjacent) modify risk/reward structure
- Can adapt to non-shooter genres (Tetris 99, auto-battlers)

---

### Cozy / Life Sim

**Core identity:** Low-stakes, pleasant engagement with world-building, collection, or daily routine activities. Relaxation over challenge.

**Temporal commitments:**
- Macro loop: Long-term world/farm/town development (tens of hours)
- Meso loop: In-game day or activity cycle (15-60 minutes)
- Micro loop: Individual task (planting, fishing, crafting) (seconds to minutes)
- Meta loop: Often real-time connected (daily events, seasons)
- Pacing: Steady-state or gentle escalation; no pressure
- Stopping points: End of in-game day is natural; can stop almost anywhere

**Mechanical expectations:**
- Collection/completion systems
- Crafting or building
- NPC relationships
- Daily/seasonal cycles (real or accelerated)
- Low or no failure states
- Customization/expression options

**Aesthetic affinities:**
- Primary: Submission (relaxation), Expression (customization)
- Secondary: Completion (collections), Progression (farm/town growth), Fellowship (NPC relationships)

**Cognitive profile:**
- Casual to midcore
- Low-moderate tracking load (collections, relationships)
- Low decision load (no wrong choices)
- Low execution load

**Modification notes:**
- Can add optional challenge layers (combat in Stardew Valley)
- Real-time mechanics create routine but may pressure players
- Social features can add Fellowship
- Narrative can add emotional depth (Spiritfarer)

---

## Tabletop RPG Archetypes

### Campaign (Long-form)

**Core identity:** Extended narrative across many sessions with persistent characters, world, and consequences. Collaborative storytelling over months or years.

**Temporal commitments:**
- Macro loop: Campaign arc (months to years, 10-100+ sessions)
- Meso loop: Story arc or adventure (3-10 sessions)
- Micro loop: Scene or encounter (minutes to an hour)
- Session: 2-5 hours typically
- Pacing: Narrative pacing across arcs; sessions need internal satisfaction
- Stopping points: End of session; ideally end of scene, not mid-combat

**Mechanical expectations:**
- Character persistence and advancement
- World persistence (actions have consequences)
- GM (usually) managing narrative and adjudication
- Combat or conflict resolution system
- Character sheet tracking capabilities, resources, relationships

**Aesthetic affinities:**
- Primary: Narrative (story investment), Fellowship (shared experience)
- Secondary: Expression (character building), Challenge (combat/obstacles), Discovery (world/plot)

**Cognitive profile:**
- Midcore to hardcore (session length demands)
- Tracking load varies by system (D&D high, PbtA lower)
- Decision load moderate (character choices)
- Execution load low (no real-time elements)

**Modification notes:**
- System choice dramatically affects cognitive load and aesthetic emphasis
- "West Marches" variant allows variable attendance
- Episodic structure (see below) can adapt to scheduling constraints

---

### One-Shot

**Core identity:** Complete experience in single session. Characters and situation are contained; no continuation expected.

**Temporal commitments:**
- Macro loop: Entire session (2-5 hours)
- Meso loop: Acts or major scenes (30-60 minutes)
- Micro loop: Individual scenes or encounters (10-30 minutes)
- Pacing: Compressed narrative arc; must reach satisfying conclusion
- Stopping points: Only at end (by definition)

**Mechanical expectations:**
- Pre-generated or quickly generated characters
- Contained scenario with clear objective
- Streamlined rules (no time for lookup)
- Minimal bookkeeping
- Clear endpoint

**Aesthetic affinities:**
- Primary: Variable (depends on one-shot type)
- Common: Narrative (contained story), Challenge (heist, dungeon), Tension (horror)

**Cognitive profile:**
- Variable, but system should be accessible
- Low tracking load (short duration)
- Decision load concentrated (fewer but weightier choices)
- Execution load low

**Modification notes:**
- Excellent for convention play, new player introduction
- Can test campaign concepts
- Horror and mystery genres suit one-shot structure well
- Pre-generated characters with built-in relationships accelerate engagement

---

### Episodic Campaign

**Core identity:** Ongoing world and characters, but each session is designed as complete unit. Accommodates irregular attendance and scheduling.

**Temporal commitments:**
- Macro loop: Overall campaign (indefinite)
- Meso loop: Single session (2-4 hours) designed as complete episode
- Micro loop: Scenes within episode
- Pacing: Each session has beginning, middle, end; ongoing threads connect sessions
- Stopping points: End of each session (designed for this)

**Mechanical expectations:**
- Character persistence (but flexible attendance)
- Session-contained objectives
- "Previously on..." and "Next time..." framing
- Minimal cliffhangers that depend on specific players
- Downtime systems for between-session advancement

**Aesthetic affinities:**
- Similar to campaign but with session-level completion needs
- Completion becomes more prominent (each session resolves something)

**Cognitive profile:**
- Midcore (can accommodate casual with right system)
- Lower between-session memory burden
- Session tracking self-contained

**Modification notes:**
- Ideal for busy adult groups
- Blades in the Dark's "score" structure is designed for this
- Requires GM skill in pacing to complete arcs in session

---

### GM-less / Story Game

**Core identity:** Collaborative narrative without traditional GM role. Rules distribute narrative authority among all players.

**Temporal commitments:**
- Variable; often one-shot or short campaign
- Meso loop: Scenes or acts as defined by game
- Micro loop: Individual narrative beats or card plays
- Pacing: Defined by game structure (act structure, token economy, etc.)
- Stopping points: Defined by game (act breaks, resource depletion)

**Mechanical expectations:**
- Distributed narrative authority
- Scene framing rules
- Conflict resolution without GM adjudication
- Often: prompts or constraints guiding narrative
- Often: explicit safety tools

**Aesthetic affinities:**
- Primary: Narrative (collaborative storytelling), Expression (character authorship)
- Secondary: Fellowship (shared creation), Discovery (emergent story)

**Cognitive profile:**
- Variable; often accessible
- Social/creative load replaces tracking load
- Decision load around narrative choices
- Requires player comfort with narrative authority

**Modification notes:**
- Excellent for groups without willing GM
- Different games offer very different structures (Fiasco vs. Microscope vs. Wanderhome)
- Some require specific player counts
- May not satisfy players seeking Challenge or tactical play

---

## Board Game Archetypes

### Euro / Strategy

**Core identity:** Resource conversion, optimization, and engine building. Low direct conflict; competition through efficiency. Clear rules, deterministic systems.

**Temporal commitments:**
- Macro loop: Full game (60-180 minutes typically)
- Meso loop: Round or era (10-30 minutes)
- Micro loop: Individual turn or action (1-5 minutes)
- Pacing: Build toward scoring/endgame; often accelerating engine speeds
- Stopping points: Between rounds (acceptable); game designed to complete in session

**Mechanical expectations:**
- Resource management and conversion
- Action selection or worker placement
- Victory points as win condition
- Limited randomness (or mitigatable randomness)
- Multiple viable strategies
- Scales with player count

**Aesthetic affinities:**
- Primary: Mastery (optimization), Challenge (competition through efficiency)
- Secondary: Completion (game end), Expression (strategy choice)

**Cognitive profile:**
- Midcore to hardcore
- High tracking load (resources, options, opponents' positions)
- High decision load (optimization calculations)
- Low execution load (turn-based, no dexterity)

**Modification notes:**
- Complexity range is wide (gateway to heavy)
- Solo modes increasingly common
- Theme integration varies (pure euro to thematic euro)

---

### Party Game

**Core identity:** Social interaction, humor, and accessibility prioritized over strategic depth. Large groups, quick rounds, minimal learning curve.

**Temporal commitments:**
- Macro loop: Full game (15-60 minutes)
- Meso loop: Round (2-10 minutes)
- Micro loop: Individual turn or response (seconds to a minute)
- Pacing: Fast, energetic; maintains group energy
- Stopping points: Between rounds; can often end early without issue

**Mechanical expectations:**
- Simple rules (explain in 2 minutes)
- Social interaction as core mechanic
- Often: judging, voting, or performance
- Scales to large groups (6+)
- Low stakes; losing isn't painful

**Aesthetic affinities:**
- Primary: Fellowship (social bonding), Submission (low-stress fun)
- Secondary: Expression (creativity, performance), Competition (light)

**Cognitive profile:**
- Casual
- Minimal tracking load
- Low decision load (intuitive choices)
- Social load primary

**Modification notes:**
- Often inappropriate for small groups
- Cultural/group fit matters (humor is subjective)
- Can wear thin with repeated play (variety needed)

---

### Cooperative

**Core identity:** All players work together against the game system. Shared victory or defeat.

**Temporal commitments:**
- Macro loop: Full game (45-120 minutes typically)
- Meso loop: Round or phase (5-15 minutes)
- Micro loop: Individual turn or decision (1-3 minutes)
- Pacing: Often escalating threat; crisis builds to climax
- Stopping points: Between rounds (acceptable); often designed for single session

**Mechanical expectations:**
- Shared win/loss condition
- Game system as opponent (deck, board state, timer)
- Role differentiation (asymmetric player powers)
- Communication mechanics (sometimes limited)
- Escalating difficulty or threat
- Difficulty settings

**Aesthetic affinities:**
- Primary: Fellowship (teamwork), Challenge (overcoming the game)
- Secondary: Tension (shared peril), Narrative (many are themed)

**Cognitive profile:**
- Midcore typically
- Shared tracking load (distributed among players)
- Collective decision-making
- "Quarterbacking" risk (one player dominates)

**Modification notes:**
- Communication limits (Hanabi) prevent quarterbacking
- Traitor variants add hidden information and Tension
- Difficulty tuning is critical for repeat play
- Legacy/campaign variants add Progression

---

### Deckbuilder

**Core identity:** Players construct their deck during play through acquisition mechanics. Engine building through card synergies.

**Temporal commitments:**
- Macro loop: Full game (30-90 minutes)
- Meso loop: Deck cycle (variable; speeds up as deck thins/optimizes)
- Micro loop: Individual turn (1-3 minutes)
- Pacing: Build phase → optimization → payoff as engine comes online
- Stopping points: Between turns; designed for single session

**Mechanical expectations:**
- Starting deck of basic cards
- Market/supply for acquisition
- Deck cycling (shuffle discard when deck empty)
- Trash/thin mechanics (remove weak cards)
- Card synergies and combos
- Victory condition (points, objectives, etc.)

**Aesthetic affinities:**
- Primary: Mastery (engine optimization), Discovery (finding combos)
- Secondary: Challenge (competition), Expression (build choices)

**Cognitive profile:**
- Midcore
- Moderate tracking load (deck composition, market state)
- High decision load (acquisition, play order)
- Low execution load

**Modification notes:**
- Cooperative variants exist (Aeon's End)
- Campaign/legacy variants add Progression
- Can hybridize with other archetypes (deckbuilding roguelike)

---

## Using the Archetype Library

**When starting with an archetype:**

1. Review the archetype's commitments (temporal, mechanical, cognitive)
2. Check alignment with your aesthetic goals (does this archetype naturally serve your target aesthetic?)
3. Identify what you're keeping vs. modifying
4. Document your modifications and why

**When starting without an archetype:**

1. Design through the derivation chain
2. As your design emerges, compare to archetypes
3. If you're converging on an archetype, decide whether to embrace it (inherit tested patterns) or diverge intentionally (subvert expectations)

**Common archetype modifications:**

- **Compression:** Shorten loops for more casual audience (roguelike runs from 60 to 20 minutes)
- **Expansion:** Add meta-loop for engagement (roguelite meta-progression)
- **Hybridization:** Combine archetypes (deckbuilding + roguelike)
- **Aesthetic shift:** Use archetype structure but target different aesthetic (cozy roguelike, narrative idle game)
- **Subversion:** Intentionally break archetype expectations (permadeath game with death as progression)

**Archetype as communication:**

Archetypes help communicate your design. "Roguelike with cozy aesthetic" instantly conveys a set of expectations and an intentional subversion. This helps team alignment, marketing, and player expectation-setting.

But archetype labels are promises. If you call something a roguelike, players expect permadeath and procedural generation. Unmet expectations damage trust. Label accurately, or clearly communicate your divergence.
