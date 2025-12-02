# Chapter 6 Supplementary Material: Balance Quick Reference

This supplementary material accompanies Chapter 6 (Balance). Use it as a reference during design work, after you've internalized the core concepts from the main chapter.

## What's In This Document

| Section | What You'll Find | Use When... |
|---------|------------------|-------------|
| **The Five-Level Framework** | Quick reference for the balance derivation process | Starting balance work on a new system |
| **Aesthetic-Dynamic Pairs** | Required dynamics for each aesthetic with example failures | Identifying what dynamics you need |
| **Paradigm Reference** | Three paradigms with requirements, failures, and LLM integration | Choosing your balance approach |
| **Paradigm Selection Flowchart** | Decision tree for paradigm choice | Quick paradigm selection |
| **Measurable Targets by Dynamic** | Specific targets for each dynamic type | Setting measurable goals |
| **Parameter Derivation Worksheet** | Step-by-step calculation template | Deriving specific numbers |
| **Iteration Diagnostic Checklist** | Problem → Cause → Solution mappings | Troubleshooting balance issues |
| **LLM Integration Patterns** | How each paradigm uses LLM | Designing LLM-enhanced balance |

---

## The Five-Level Framework

| Level | Question | Output |
|-------|----------|--------|
| 1. Aesthetic | What experience are you creating? | Target aesthetic (from Chapter 1) |
| 2. Dynamics | What behaviors create that experience? | Required dynamics list |
| 3. Paradigm | What approach creates those behaviors? | Consistency / Framework / Adaptive |
| 4. Measurables | How do you verify it's working? | 3-5 quantifiable targets |
| 5. Parameters | What specific numbers achieve it? | Actual values for your game |

**The derivation flows downward. Validation flows upward.**

---

## Aesthetic-Dynamic Pairs

### Challenge Aesthetic

**Required Dynamics:**
- Pattern learning (observe, hypothesize, test, refine)
- Skill expression (expert execution demonstrably better than novice)
- Failure recovery (death followed by immediate retry with gained knowledge)
- Mastery progression (clear improvement curve)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Pattern learning | Random attack patterns | Frustration, not challenge |
| Skill expression | Outcomes luck-based | Gambling, not mastery |
| Failure recovery | Long respawn times | Punishment, not learning |
| Mastery progression | Flat difficulty | Boredom after initial learning |

### Tension Aesthetic

**Required Dynamics:**
- Resource pressure (forced into hard choices by scarcity)
- Threat awareness (constant vigilance, can't fully relax)
- Close calls (near-death moments creating adrenaline)
- Risk evaluation (continuous danger-vs-reward calculations)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Resource pressure | Abundant resources | Relaxation, not tension |
| Threat awareness | Predictable safe zones | Complacency |
| Close calls | Either too easy or instant death | Boredom or frustration |
| Risk evaluation | No meaningful risk/reward choices | Mechanical play |

### Discovery Aesthetic

**Required Dynamics:**
- Information gathering (actively seeking clues)
- Theory formation (connecting dots, forming hypotheses)
- Revelation moments ("aha!" experiences when understanding clicks)
- Systematic exploration (investigating methodically)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Information gathering | All info immediately visible | Comprehension, not discovery |
| Theory formation | Clues don't connect logically | Confusion |
| Revelation moments | Solutions given, not discovered | Observation, not participation |
| Systematic exploration | Random success | Luck, not investigation |

### Mastery Aesthetic

**Required Dynamics:**
- System optimization (experimenting to find synergies)
- Strategic depth (multiple viable approaches with trade-offs)
- Build experimentation (theory-crafting and testing combinations)
- Expert differentiation (deep knowledge provides significant advantage)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| System optimization | No synergies to find | Shallow execution |
| Strategic depth | One obviously optimal strategy | No meaningful choices |
| Build experimentation | Respec costly or impossible | Fear of experimentation |
| Expert differentiation | Low skill ceiling | No long-term engagement |

### Narrative Aesthetic

**Required Dynamics:**
- Character engagement (emotional investment in fates)
- Consequence tracking (remembering and anticipating outcomes)
- Dramatic tension (experiencing story beats emotionally)
- Agency expression (choices feel like they matter)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Character engagement | Flat characters | Indifference |
| Consequence tracking | Choices don't persist | Meaninglessness |
| Dramatic tension | Even pacing throughout | Monotony |
| Agency expression | Choices don't affect outcomes | Observation, not participation |

### Submission Aesthetic

**Required Dynamics:**
- Flow state (actions become automatic)
- Rhythmic engagement (steady, predictable pacing)
- Stress reduction (low pressure, minimal consequences)
- Meditative execution (satisfying repetitive actions)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Flow state | Frequent interruptions | Frustration |
| Rhythmic engagement | Irregular pacing | Anxiety |
| Stress reduction | High stakes, severe punishment | Tension, not submission |
| Meditative execution | Actions feel like work | Chore, not relaxation |

### Fellowship Aesthetic

**Required Dynamics:**
- Cooperation patterns (meaningful coordination)
- Role specialization (unique contributions)
- Shared stakes (outcomes affect the group)
- Communication loops (regular discussion and planning)

**Example Failures:**

| Missing Dynamic | Cause | Result |
|-----------------|-------|--------|
| Cooperation patterns | Solo success easy | Parallel play, not fellowship |
| Role specialization | Everyone does everything | No interdependence |
| Shared stakes | Individual outcomes only | Competition, not cooperation |
| Communication loops | No need to discuss | Silent play |

---

## Paradigm Reference

### Consistency Balance

**Core Mechanism:** Rules produce identical outcomes for identical situations.

**Dynamics Created:** Pattern learning, skill expression, mastery curves, strategic depth.

**Primary Aesthetics:** Challenge, Mastery.

**Requirements:**
- Repeatability (same situations recur)
- Clarity (players perceive rules and outcomes)
- Fast iteration (quick death/retry)
- Fair feedback (understand why failed)
- Skill-based (execution/decision > chance)

**Failure Modes:**
- Rules too complex to learn
- Situations never repeat
- Randomness too high
- Feedback unclear

**Temporal Fit:** Fast micro loops, episodic or escalating pacing.

**LLM Integration:** Presentation layer only. LLM narrates outcomes but doesn't determine them. Temperature 0 for consistency.

### Framework Balance

**Core Mechanism:** GM adjudicates using position/effect framework.

**Dynamics Created:** Social negotiation, creative problem-solving, dramatic pacing, agency expression.

**Primary Aesthetics:** Narrative, Discovery, Fellowship.

**Requirements:**
- GM skill (competent, engaged)
- Social contract (trust in fairness)
- Fiction-first (narrative > mechanics)
- Flexibility (systems support adaptation)
- Consequence design (failure = interesting, not just loss)

**Failure Modes:**
- No skilled GM available
- Players want mechanical mastery
- Challenge precision required
- Complexity exceeds GM capacity

**Temporal Fit:** Variable pacing, episodic and emergent patterns.

**LLM Integration:** Adjudication role. LLM serves as GM for solo play. Must maintain fiction consistency.

### Adaptive Balance

**Core Mechanism:** System adjusts difficulty based on player performance.

**Dynamics Created:** Flow state, sustained pressure, tension maintenance, stress reduction.

**Primary Aesthetics:** Tension, Submission.

**Requirements:**
- Performance tracking (accurate measurement)
- Invisible adjustment (players don't notice)
- Appropriate metrics (track experience quality)
- Constraint bounds (reasonable limits)
- Responsiveness (adjusts quickly)

**Failure Modes:**
- Adaptation too obvious
- Wrong metrics tracked
- Undermines learning
- Removes skill expression

**Temporal Fit:** Steady-state pacing, maintains consistent intensity.

**LLM Integration:** Interpretation role. LLM assesses player state holistically from language and behavior.

---

## Paradigm Selection Flowchart

```
START: What aesthetic are you targeting?

├── Challenge or Mastery?
│   └── → CONSISTENCY
│       └── Need pattern learning and skill expression
│
├── Tension?
│   ├── Want maintained pressure regardless of skill?
│   │   └── → ADAPTIVE
│   └── Want learnable threat patterns?
│       └── → CONSISTENCY + resource economy
│
├── Narrative or Discovery?
│   └── → FRAMEWORK
│       └── Need agency expression and flexible adjudication
│
├── Submission?
│   ├── Want difficulty matching to player?
│   │   └── → ADAPTIVE
│   └── Want simple, predictable systems?
│       └── → CONSISTENCY (forgiving)
│
└── Fellowship?
    ├── Want social negotiation?
    │   └── → FRAMEWORK
    └── Want mechanical interdependence?
        └── → CONSISTENCY (cooperative)
```

**LLM Consideration:**
- Heavy LLM adjudication → Framework
- LLM enhancement of Challenge → Consistency + LLM presentation
- LLM-interpreted difficulty → Adaptive + LLM interpretation

---

## Measurable Targets by Dynamic

### Pattern Learning (Challenge)

| Measurable | Target | Range |
|------------|--------|-------|
| TTK improvement (attempt 1→10) | 40% reduction | ±10% |
| Prediction accuracy (by attempt 5) | 70% | ±10% |
| Expert vs. trained gap | 50% faster | ±15% |
| Retry willingness | >80% immediate retry | — |
| Error reduction (attempt 1→10) | 60% fewer mistakes | ±15% |

### Resource Pressure (Tension)

| Measurable | Target | Range |
|------------|--------|-------|
| Average health | 40% | ±10% |
| Average key resource | 35% | ±10% |
| Close calls per 10 min | 2-3 | — |
| Resource decisions per session | 5-8 | — |
| Time in danger zone | 15-25% | — |

### System Optimization (Mastery)

| Measurable | Target | Range |
|------------|--------|-------|
| Viable strategies | 5-10 within 20% power | — |
| Expert efficiency gap | 30% better than casual | ±10% |
| Build diversity (no single >X%) | 40% max | — |
| Optimization ceiling | 20+ hours before plateau | — |
| Experimentation rate | 3+ new builds tried | — |

### Information Gathering (Discovery)

| Measurable | Target | Range |
|------------|--------|-------|
| Clue discovery rate | 60-80% | — |
| False theories per investigation | 2-3 | — |
| Correct revelation timing | Attempt 3-4 | — |
| Systematic search evidence | >70% show method | — |
| "Aha!" report rate | >70% | — |

### Social Negotiation (Framework)

| Measurable | Target | Range |
|------------|--------|-------|
| Negotiation moments per session | 4-6 | — |
| Creative proposals per session | 3-5 | — |
| Framework consistency | >80% similar rulings | — |
| Agency perception | >80% feel choices matter | — |
| Player-initiated proposals | >50% of actions | — |

### Flow State (Submission/Adaptive)

| Measurable | Target | Range |
|------------|--------|-------|
| Difficulty match ("just right") | >70% | — |
| Session extension beyond target | Common | — |
| Stress indicators | Decreasing | — |
| "Zone" state reports | >60% | — |
| Interruption frustration | Low | — |

---

## Parameter Derivation Worksheet

### Step 1: Gather Constraints

| Constraint Source | Value | Notes |
|-------------------|-------|-------|
| Target TTK (from temporal) | ___ seconds | Meso loop duration |
| Player action frequency | ___ per second | How often can player act? |
| Hit rate (trained player) | ___% | Realistic success rate |
| Hit rate (novice) | ___% | First attempt rate |
| Hit rate (expert) | ___% | Optimized rate |

### Step 2: Calculate Required Hits

```
Target TTK × Action frequency × Hit rate = Total hits needed
___ sec × ___ actions/sec × ___% = ___ hits
```

### Step 3: Derive HP from Damage

```
If player damage = ___ per hit
Then target HP = hits needed × damage per hit
HP = ___ × ___ = ___
```

### Step 4: Verify Against Profiles

| Profile | Hit Rate | Hits in Target TTK | Damage Dealt | Result |
|---------|----------|-------------------|--------------|--------|
| Novice | ___% | ___ | ___ | Dies (expected) |
| Trained | ___% | ___ | ___ | Wins at target TTK |
| Expert | ___% | ___ | ___ | Wins faster |

### Step 5: Add Supporting Parameters

| Parameter | Value | Derivation |
|-----------|-------|------------|
| Telegraph timing | ___ sec | Reaction time + decision buffer |
| Respawn time | ___ sec | From temporal (Challenge <10s) |
| Attack patterns | ___ count | Enough variety, not overwhelming |

---

## Iteration Diagnostic Checklist

### TTK Problems

| Symptom | Likely Cause | Solution |
|---------|--------------|----------|
| TTK too short | HP too low OR damage too high | Increase HP 20% first |
| TTK too long | HP too high OR damage too low | Decrease HP 20% first |
| TTK inconsistent | High variance mechanics | Reduce randomness |
| TTK doesn't improve | Pattern learning failing | Check telegraphs, consistency |

### Dynamic Problems

| Symptom | Likely Cause | Solution |
|---------|--------------|----------|
| No pattern learning | Attacks not predictable | Add/clarify telegraphs |
| No skill expression | Outcomes too random | Increase skill weight |
| No resource pressure | Resources too abundant | Reduce spawn rates |
| No close calls | Difficulty wrong | Adjust toward 40% health average |
| No agency feeling | Choices don't matter | Add meaningful consequences |

### Paradigm Problems

| Symptom | Likely Cause | Solution |
|---------|--------------|----------|
| "Feels random" (Consistency) | Hidden randomness | Make rules transparent |
| "Feels arbitrary" (Framework) | Inconsistent rulings | Document precedents |
| "Feels manipulated" (Adaptive) | Adaptation too visible | Smooth adjustments |
| "Can't learn" (Consistency) | Complexity too high | Simplify or chunk rules |
| "No creativity" (Framework) | Too prescriptive | Open scene framing |

---

## LLM Integration Patterns by Paradigm

### Consistency + LLM

**Role:** Presentation layer

**What LLM Does:**
- Narrates mechanical outcomes
- Describes combat aesthetically
- Provides flavor without changing results

**What LLM Doesn't Do:**
- Determine success/failure
- Modify damage or effects
- Make adjudication decisions

**Implementation:**
```
Mechanical layer: Player deals 90 damage (deterministic)
LLM layer: "Your blade finds the gap in the beast's scales, 
           drawing a spray of dark ichor" (generated)
```

**Temperature:** 0 or very low for consistency

### Framework + LLM

**Role:** Adjudication (GM substitute)

**What LLM Does:**
- Evaluates player proposals
- Assigns position/effect
- Maintains fictional consistency
- Generates consequences

**What LLM Doesn't Do:**
- Break established fiction
- Contradict previous rulings
- Ignore player agency

**Implementation:**
```
Player: "Can I swing from the chandelier to reach the balcony?"
LLM: Evaluates fictional positioning, assigns Risky/Standard,
     generates outcome maintaining world consistency
```

**Critical Constraint:** Must track and respect established facts

### Adaptive + LLM

**Role:** Interpretation layer

**What LLM Does:**
- Assesses player state from language
- Detects frustration, boredom, engagement
- Suggests narrative adaptations
- Interprets holistic signals

**What LLM Doesn't Do:**
- Replace all metrics (combine with behavioral)
- Make adjustment decisions alone
- Adapt so much that challenge disappears

**Implementation:**
```
Behavioral: Player died 3 times
LLM interpretation: Player messages show curiosity, not frustration
Decision: Maintain difficulty, player is engaged in learning
```

**Key Insight:** LLM enables narrative adaptation (NPC offers help) rather than just parameter tweaking (reduce enemy HP)

---

*This supplementary material is reference documentation. Return to the main Chapter 6 text for conceptual understanding and worked examples.*
