Worked Example 1: Casual Mobile Roguelike

**Starting point:** Aesthetic-first with constraints. A roguelike-inspired mobile game for casual players. Light humor, pixel art. Something for commutes.

**Immediate tension:** Roguelikes are typically midcore/hardcore. Casual roguelike is deliberate subversion requiring careful derivation.

***

**Level 1: Aesthetic Profile**

Primary aesthetic: Challenge (earned triumph through skill development)
Secondary aesthetic: Progression (meta-unlocks for return motivation)

Player profile: Casual mobile

* 5-15 minute sessions
* Cognitive budget of 3±2 tracked elements
* Low complexity tolerance
* Expect interruption

Tone: Light humor means failure is amusing, not punishing. Death is punchline, not tragedy.

Success criteria:

* "I did it!" moments at least once per session
* Noticeable improvement over first 5-10 runs
* Voluntary return (not FOMO-driven)
* Clean exit possible at any moment

***

**Level 2: Required Dynamics**

Core loop: Attempt → fail/succeed → learn → retry. But compressed: learning must happen in 3-5 tries, not 50.

Peak moments: Victory over previously-lethal enemy, run completion, new personal best. Must occur every session.

Anti-dynamics: Grind (repetition without skill), confusion (unclear deaths), frustration (failure without learning), complexity overwhelm.

Humor dynamic: Death produces chuckle, not groan. Enemies are silly. Failure text is funny.

Cognitive check: 3±2 budget = health, attack capability, enemy patterns. Resource management must be minimal or automated.

***

**Level 3: Temporal Architecture**

Run (macro): 5-8 minutes. Fits casual session, allows 1-2 complete runs per play.

Floor (meso): 90-120 seconds each, 3-4 floors per run. Each floor is completable unit with progress persistence.

Encounter (micro): 15-30 seconds. Fast iteration, long enough for pattern recognition. 3-5 encounters per floor plus mini-boss.

Pacing: Escalating within run. Floor 1 easy (confidence), Floor 2 introduces challenge, Floors 3-4 where most deaths occur.

Stopping points: Between floors (good), between runs (excellent), mid-encounter (acceptable with pause).

Content scale:

* 6-8 enemy types (learnable in casual timeframe)
* 3-4 floor tilesets
* 10-15 upgrade options
* 4 bosses (one per tileset)

***

**Level 4: Balance Paradigm**

Paradigm: Consistency. Pattern learning requires deterministic enemies. Red flash always means jump.

Why not Adaptive: Would undermine Challenge aesthetic. Earned triumph requires consistent obstacles.

Archetype inheritance: Roguelike gives procedural generation, run-based structure, build variety. Not inheriting: permadeath punishment severity (light humor framing softens failure).

***

**Level 5: Mechanical Specification**

Core mechanic: Auto-attack combat with positioning. Player moves character, character auto-attacks nearest enemy. Skill expression through positioning and dodge timing.

Why auto-attack: Touch precision limited. Positioning is intuitive; combos are not.

Resources:

1. Health (Limiter): 3 HP. One hit = one damage. Hearts display.
2. Coins (Currency): Collected during run, spent between floors. Resets each run.
3. Stars (Meta-resource): Earned at run-end, spent on permanent unlocks.

Three resources. Within budget.

Recovery: No health recovery within floor. Possible between floors (uncommon). Creates tension without attrition spiral.

Upgrades: Between floors, choose 1 of 3. Stat boosts or simple abilities. No complex synergies.

Content approach: Procedural floor layouts, hand-authored enemy patterns and bosses.

***

**Level 6: Parameters**

Target measurables:

* Run completion: \~20% initially, \~60% after 10 runs
* Average run (new player): 3-4 minutes (die Floor 2-3)
* Average run (learned): 5-7 minutes (reach boss)
* Deaths per session: 2-4
* Triumph moments per session: 1-3

Combat parameters:

Target encounter: 20 seconds.

Enemies per encounter: 2-4.

Player DPS: 1 damage per attack, attack every 2 seconds = 0.5 DPS. 3 enemies × 3 HP = 9 HP ÷ 0.5 DPS = 18 seconds. ✔

Enemy damage: Player has 3 HP, should survive 2-3 floors initially. \~1 hit per 4-6 encounters. Floor 1 enemies: attack every 4 seconds, 15% hit rate. Floor 3-4: attack every 2.5 seconds, 25% hit rate.

Floor timing: 4 encounters × 20 seconds + 20 seconds traversal = 100 seconds per floor. 4 floors = 6.6 minutes per run. ✔

Boss: 15 HP, 3-phase pattern, learnable over 2-3 attempts.

Meta-progression:

* 3 stars per completion, 1 for reaching boss
* Unlock costs: 10-50 stars
* Total unlocks: 15-20
* Time to complete: 2-4 weeks casual play

***

**Content Derivation**

Enemy count: 16 encounters per run, 3-5 encounters to learn each type, want variety without overwhelming pattern-learning. 8 common enemies, 3 rare, 4 bosses = 10-12 total.

Sprites per enemy:

* Idle: 1-2 frames
* Telegraph: 2-3 frames (critical for pattern learning)
* Attack: 2-3 frames
* Hit: 1-2 frames
* Death: 3-4 frames (humor opportunity)
* Total: 9-14 frames per enemy

Bosses: 25-30 frames each (3 attack patterns, phase transitions, dramatic death)

Player character: 18-27 frames. Variants via palette swap.

Environment: 4 tilesets × 40-60 pieces = 160-240 pieces.

UI: \~70-90 sprites.

Effects: \~25-35 frames.

**Total art budget: 450-600 pieces** (with palette swaps).

Writing:

* Enemy descriptions: 300-500 words
* Death messages: 20-30 unique, 100-300 words (humor-critical)
* Upgrade text: 75-200 words
* Boss intros: 80-160 words
* Tutorial/tips: 300-750 words
* Meta flavor: 100-450 words
* **Total: \~1,000-2,400 words**

***

**What This Example Shows**

Each number traces back through the chain:

* 6.6-minute runs ← casual session windows ← player profile (Level 1)
* 3 HP ← cognitive simplicity ← casual budget (Level 1)
* 20-second encounters ← 90-second floors ← temporal architecture (Level 3)
* Enemy attack rates ← pattern learning requirements ← Challenge dynamics (Level 2)
* 10-12 enemy types ← variety ÷ mastery time ← temporal architecture (Level 3)
* 9-14 frames per enemy ← telegraph requirements ← pattern learning dynamics (Level 2)
* 20-30 death messages ← expected deaths × repetition tolerance ← Challenge aesthetic (Level 1)

The roguelike example showed Consistency paradigm with systems-heavy design. Now consider the opposite end of the spectrum.