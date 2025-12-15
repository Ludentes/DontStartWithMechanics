# Supplementary Material: Testing Design Decisions

Testing is how designs become games. Until real players engage with your system, you have only hypotheses. This document covers how to test design decisions at each level of the derivation chain, how to run effective playtests, and how to interpret results.

---

## Testing Philosophy

### Tests Are Experiments, Not Auditions

A playtest is not a performance where you hope players like your game. It's an experiment where you gather data about whether your design hypotheses are correct.

This reframe matters. If playtests are auditions, negative feedback feels like rejection. If playtests are experiments, negative feedback is valuable data. The hypothesis "players will experience tension when resources drop below 30%" can be confirmed or refuted. Both outcomes are useful.

Before each test, articulate what you're testing. "Does this work?" is too vague. "Do players check resource counts before committing to major actions?" is testable. "Do players report feeling tense during the final encounter?" is testable. Specific hypotheses yield actionable results.

### Test Early, Test Ugly

The earlier you test, the cheaper it is to change direction. Testing a paper prototype costs hours. Testing after six months of development costs months of rework.

Early tests should be ugly. Placeholder art, handwritten cards, verbal descriptions of what would eventually be animated. Polish obscures problems by making players reluctant to criticize something that looks finished. Ugly prototypes invite honest feedback.

The goal of early testing isn't to validate the final product. It's to invalidate bad directions before you invest in them.

### Test the Right Thing at the Right Time

Different development stages require different tests:

**Concept stage:** Does the core loop feel promising? Test with paper prototypes, verbal walkthroughs, or minimal implementations. You're testing whether the fundamental idea works, not whether the execution is good.

**System stage:** Do mechanics create intended dynamics? Test with functional prototypes that have real rules but placeholder content. You're testing whether the systems interact correctly.

**Parameter stage:** Are the numbers right? Test with near-complete implementations where you're tuning values. You're testing calibration, not concept.

**Polish stage:** Does the complete experience land? Test with polished builds on target audience. You're testing whether everything comes together.

Testing calibration when you haven't validated the concept wastes effort. Testing concept with a polished build makes pivoting expensive. Match test type to development stage.

---

## Testing by Chain Level

Each level of the derivation chain has different testing needs and methods.

### Testing Level 1: Aesthetic Profile

**What you're testing:** Is this the right experience for this audience?

**Methods:**

*Concept pitching:* Describe your intended experience to target players. "This is a game where you'll feel X through doing Y." Watch for enthusiasm versus polite interest. Ask: "Would you play this? What would make you more interested?"

*Comparable analysis:* Identify existing games that target similar aesthetics for similar audiences. Do those games have engaged playerbases? What do players say about them? If no comparable exists, that's either opportunity or warning sign.

*Early prototype reaction:* After minimal prototype exposure, ask players to describe what they experienced. Do their descriptions match your intended aesthetic? If you're targeting Tension and they describe "relaxing puzzle-solving," there's a mismatch.

**What you're looking for:**
- Target audience recognizes and wants the described experience
- Early prototypes evoke descriptions matching intended aesthetic
- Players in target profile engage voluntarily (not just completing a task)

**Red flags:**
- Players describe experiences very different from intent
- Target audience expresses disinterest in concept
- Players engage dutifully but don't express enthusiasm
- You're designing for an audience you can't access for testing

### Testing Level 2: Required Dynamics

**What you're testing:** Do the intended behaviors actually emerge?

**Methods:**

*Behavioral observation:* Watch players interact with your prototype. Don't guide them. Note what they actually do, not what you hope they'll do.

For each required dynamic from your derivation, check:
- Core loop behavior: Are players doing the intended repeated action?
- Peak moments: Do the intended high points occur?
- Progression: Are players learning/growing in intended ways?
- Anti-dynamics: Are the behaviors you wanted to prevent absent?

*Think-aloud protocol:* Ask players to verbalize their thinking while playing. "I'm checking my health because I'm worried about the next fight." This reveals whether players are engaging with systems as intended.

*Post-session interview:* Ask players to describe what they did and why. Compare their descriptions to your intended dynamics. Gaps between intended and actual behavior indicate design problems.

**What you're looking for:**
- Players exhibit core loop behavior without prompting
- Peak moments occur at intended frequency
- Players describe thought processes matching intended dynamics
- Anti-dynamics are absent

**Red flags:**
- Players do something other than core loop (ignore main mechanic, find exploit)
- Peak moments don't occur or occur at wrong times
- Players describe motivations you didn't intend ("I was just trying to get it over with")
- Anti-dynamics emerge (dominant strategy, safety when tension intended, etc.)

### Testing Level 3: Temporal Architecture

**What you're testing:** Do loops complete in intended times? Does pacing feel right?

**Methods:**

*Timed observation:* Time actual loop completions. How long do micro loops take? Meso loops? Compare to your targets from derivation.

*Pacing journaling:* Have players mark when they feel peaks and valleys of engagement. Compare to intended pacing pattern. Or observe directly: when do players lean forward (engaged) versus lean back (disengaged)?

*Stopping point testing:* Interrupt players at various points. Ask: "If you had to stop now, how would that feel?" Test whether your intended stopping points feel like natural breaks and whether non-stopping-points feel interruptive.

*Session length validation:* For your target player profile, do sessions actually fit intended duration? Do players want to stop when you expect, or do they want to continue/quit earlier?

**What you're looking for:**
- Actual loop durations within 20% of targets
- Engagement peaks align with intended pacing pattern
- Stopping points feel natural; non-stopping-points feel interruptive
- Session lengths match player profile expectations

**Red flags:**
- Loops take much longer or shorter than intended
- Engagement is flat when escalation intended (or spiky when steady intended)
- Players express frustration at stopping points or relief at non-stopping-points
- Players quit earlier than intended or resist stopping at intended points

### Testing Level 4: Balance Paradigm

**What you're testing:** Does the rules approach create the right feel?

**Methods:**

*Consistency testing (for Consistency paradigm):*
- Can players predict outcomes? Ask players to predict results before actions resolve. Track prediction accuracy over time.
- Do same inputs produce same outputs? Deliberately repeat situations; verify consistency.
- Are players learning patterns? Do repeat encounters go better than first encounters?

*Framework testing (for Framework paradigm):*
- Does adjudication feel fair? After GM/facilitator rulings, ask players if outcome felt appropriate.
- Is flexibility enabling narrative? Are story moments landing that wouldn't be possible with rigid rules?
- Is inconsistency causing problems? Do players express frustration at unpredictable rulings?

*Adaptive testing (for Adaptive paradigm):*
- Is adaptation invisible? Players shouldn't notice difficulty adjusting. If they do, immersion breaks.
- Is intended experience maintained? Despite player variance, does the target experience (tension level, flow state, etc.) stay consistent?
- Is adaptation responsive? Does the system adjust quickly enough to prevent extended periods outside target experience?

**What you're looking for:**
- Paradigm is achieving its purpose (learnability / narrative flexibility / maintained experience)
- Players aren't fighting the paradigm (complaining about randomness in Consistency game, feeling railroaded in Framework game, noticing rubber-banding in Adaptive game)

**Red flags:**
- Consistency paradigm: players can't learn patterns, outcomes feel random
- Framework paradigm: adjudication feels arbitrary, players distrust rulings
- Adaptive paradigm: players notice and exploit adaptation, experience still varies wildly

### Testing Level 5: Mechanical Specification

**What you're testing:** Do specific mechanics create intended dynamics? Is cognitive cost justified?

**Methods:**

*Mechanic isolation:* Test individual mechanics in isolation before testing the complete system. Does this mechanic, by itself, create its intended effect?

*Cognitive load observation:* Watch for signs of overload:
- Frequent UI/reference checking (tracking overload)
- Long pauses before decisions (decision overload)
- Execution errors, fumbling (execution overload)
- Requests to slow down or explain
- Glazed expressions, disengagement

*Mechanic contribution assessment:* For each mechanic, ask: "If we removed this, what would be lost?" If the answer is "not much," the mechanic may not justify its cognitive cost.

*Exploit hunting:* Actively try to break your mechanics. Find dominant strategies, exploits, degenerate cases. If you can find them, players will.

**What you're looking for:**
- Each mechanic creates its intended dynamic
- Players operate within cognitive budget (no overload signs)
- No dominant strategies or exploits
- Players engage with all mechanics (no ignored systems)

**Red flags:**
- Mechanic doesn't produce intended behavior
- Players exhibit cognitive overload signs
- Players find strategies that trivialize intended challenge
- Players ignore mechanics (suggests vestigial design)

### Testing Level 6: Parameters

**What you're testing:** Do specific numbers produce intended intensity and timing?

**Methods:**

*Measurable tracking:* Identify your key measurables from derivation (TTK, resource depletion rate, success rate, etc.). Track actual values during playtest. Compare to targets.

*Intensity calibration:* Ask players to rate intensity at various points (1-10 scale, or qualitative). Compare to intended intensity curve.

*A/B testing:* When uncertain between parameter values, test both with different player groups. Compare outcomes.

*Edge case testing:* Test with parameter values at extremes of your expected range. Verify the system degrades gracefully (or breaks in expected ways).

**What you're looking for:**
- Actual measurables within acceptable range of targets
- Player-reported intensity matches intended curve
- Parameters are robust (small changes don't break experience)
- Edge cases are handled appropriately

**Red flags:**
- Measurables significantly off target
- Players report wrong intensity (boring when exciting intended, or stressful when relaxed intended)
- Parameters are fragile (small changes break experience)
- Edge cases produce degenerate outcomes

---

## Running Playtests

### Before the Playtest

**Define your hypotheses.** What specific questions are you trying to answer? Write them down. Limit to 3-5 questions per playtest; more than that and you won't be able to track everything.

**Prepare your prototype.** Whatever fidelity is appropriate for your development stage. Ensure it's functional enough to test your hypotheses. Don't waste tester time on broken builds.

**Prepare observation tools.** Note-taking template, timer, recording device (with consent), survey questions. Know what data you're collecting before you start.

**Recruit appropriate testers.** Target audience members are ideal but not always available. At minimum, understand how your testers differ from target audience and account for it in interpretation.

**Set expectations.** Tell testers what you need from them. "I want you to play normally and think aloud." "I want you to try to break this." "I'll be asking questions but won't help if you get stuck." Clear expectations improve data quality.

### During the Playtest

**Observe, don't guide.** Resist the urge to help, explain, or correct. When players struggle, that's data. When they misunderstand, that's data. Interventions contaminate results.

**Take notes on behavior, not just outcomes.** "Player won encounter" is less useful than "Player checked resources three times before engaging, used defensive ability early, nearly died, clutch victory."

**Note timestamps for key moments.** When did engagement peak? When did confusion occur? Timestamps let you correlate events with specific game states.

**Save interpretation for later.** During the playtest, record what happened. Don't analyze yet. Analysis during observation biases what you notice.

**If you must intervene, note it.** Sometimes you have to explain something or fix a bug. When you do, mark it. That session's data is now partially compromised; account for it in analysis.

### After the Playtest

**Debrief while memory is fresh.** Ask survey questions, conduct interviews, or have players complete feedback forms immediately. Memory degrades quickly.

**Good debrief questions:**
- "Describe what you just experienced." (Open-ended, no leading)
- "What were you trying to do when [specific moment]?" (Clarifies observed behavior)
- "Was there a point where you felt [target emotion]?" (Tests aesthetic delivery)
- "What was confusing?" (Identifies clarity problems)
- "If you were going to play again, what would you do differently?" (Reveals learning and engagement)
- "Would you play this again? Why or why not?" (Tests overall appeal)

**Avoid leading questions.** "Did you feel tense during the boss fight?" leads the witness. "How did you feel during the boss fight?" does not.

**Compile data before interpreting.** Gather all notes, timestamps, survey responses, recordings. Then analyze systematically. Premature conclusions bias interpretation.

### Interpreting Results

**Compare to hypotheses.** For each question you defined before the playtest, what answer did you get? Confirmed? Refuted? Inconclusive?

**Distinguish between types of problems:**

*Clarity problems:* Players didn't understand what to do. Fix: Better tutorial, UI, feedback, or rules explanation. Usually Level 5 or 6 fixes.

*Calibration problems:* Players understood but values were wrong. Too easy, too hard, too slow, too fast. Fix: Parameter tuning. Level 6 fixes.

*Mechanical problems:* The mechanic itself doesn't create the intended dynamic. Fix: Change or replace mechanic. Level 5 fix.

*Structural problems:* The overall structure doesn't support the experience. Fix: Restructure temporal architecture or reconceive dynamics. Level 3 or 2 fixes.

*Targeting problems:* The experience isn't right for this audience, or this audience doesn't want this experience. Fix: Change audience or change aesthetic target. Level 1 fix.

**Sample size awareness.** One playtest is an anecdote, not data. Patterns across multiple playtests are more reliable. Be cautious about over-interpreting single sessions.

**Account for tester-audience mismatch.** If your tester is more experienced than target audience, easy might be "too easy for them but right for target." If less experienced, hard might be "too hard for them but right for target."

---

## Testing Formats

Different formats serve different purposes.

### Solo Testing (Designer Plays)

**Good for:**
- Verifying basic functionality
- Finding obvious breaks
- Rapid iteration on parameters
- Checking if something is possible at all

**Limited for:**
- Aesthetic delivery (you can't experience your own game fresh)
- Learning curve assessment (you already know everything)
- Blind spot detection (you'll unconsciously avoid broken areas)

**When to use:** Early and often, but never as sole validation.

### Internal Testing (Team/Friends)

**Good for:**
- Finding problems before embarrassing yourself with external testers
- Testing with high engagement (friends want to help)
- Rapid feedback cycles
- Exploratory testing (actively trying to break things)

**Limited for:**
- Target audience validation (unless team/friends are target audience)
- Fresh-eyes perspective (they've heard you talk about the game)
- Honest negative feedback (social pressure to be nice)

**When to use:** After solo testing, before external testing. Use friends for stress-testing, not validation.

### External Testing (Target Audience)

**Good for:**
- Actual aesthetic validation
- Learning curve assessment
- Fresh perspective
- Honest feedback (no social relationship to protect)

**Limited for:**
- Rapid iteration (recruiting takes time)
- Early concept testing (may burn target audience on unfinished work)
- Deep system testing (external testers give less time)

**When to use:** When you have specific hypotheses that require target audience validation. Don't burn external testers on tests you could do internally.

### Blind Testing (No Designer Present)

**Good for:**
- Tutorial and onboarding validation (can they learn without you?)
- Real-world conditions simulation
- Eliminating designer influence on play

**Limited for:**
- Understanding why problems occurred
- Catching in-the-moment reactions
- Flexibility to explore unexpected findings

**When to use:** When you need to validate that the game teaches itself. Essential for any game without human facilitation.

### Recorded Testing

**Good for:**
- Detailed behavioral analysis
- Catching things you missed live
- Showing team members who weren't present
- Before/after comparison across iterations

**Limited for:**
- Real-time response
- Tester comfort (some people behave differently on camera)

**When to use:** When you need detailed data and tester consents. Good complement to live observation, not replacement.

---

## Testing Cadence

### How Often to Test

**Concept phase:** Test whenever you have a new concept worth validating. Days to weeks between tests.

**System phase:** Test after each significant mechanical change. Days between tests.

**Parameter phase:** Test constantly. Multiple tests per day during intensive tuning.

**Polish phase:** Test each major milestone. Weekly or per-milestone.

### When to Stop Testing and Ship

Testing can continue forever. At some point, you ship. Signals that you're ready:

- Core aesthetic lands reliably (players report intended experience)
- Major problems are resolved (no critical breaks)
- Iteration returns diminish (changes produce smaller improvements)
- Target audience wants to play again (engagement validated)

You'll never achieve perfection. The goal is "good enough for audience to enjoy while you continue improving."

---

## Common Testing Mistakes

**Testing too late.** Waiting until the game is "ready" means every problem is expensive to fix. Test ugly prototypes early.

**Testing without hypotheses.** "Let's see what people think" produces vague feedback. "Let's test whether the resource pressure creates tension" produces actionable data.

**Helping stuck players.** When a player is stuck, you learn something. When you help them, you learn nothing except that you can help.

**Defensive interpretation.** "They didn't get it because they're not the target audience" might be true, or might be excuse-making. Be honest about what results mean.

**Over-weighting vocal feedback.** One player's strong opinion isn't necessarily representative. Look for patterns across testers.

**Under-weighting behavior.** What players say matters less than what they do. If they say it's fun but stop playing early, believe the behavior.

**Testing with wrong audience.** Hardcore testers will find your casual game boring. Casual testers will find your hardcore game overwhelming. Match tester to target.

**Fixing everything at once.** If a playtest reveals five problems, don't change five things. Change one, retest. Otherwise you won't know which change helped.

**Ignoring good results.** When something works, understand why. That's as valuable as understanding failures.

---

## Testing Checklist

Before each playtest:
- [ ] Hypotheses written (3-5 specific questions)
- [ ] Prototype ready (functional for hypotheses being tested)
- [ ] Observation tools prepared (notes, timer, surveys)
- [ ] Testers recruited (appropriate for test type)
- [ ] Expectations set (testers know what you need)

During each playtest:
- [ ] Observe without guiding
- [ ] Note behaviors, not just outcomes
- [ ] Timestamp key moments
- [ ] Mark any interventions

After each playtest:
- [ ] Debrief immediately
- [ ] Compile all data
- [ ] Compare to hypotheses
- [ ] Categorize problems by level
- [ ] Plan next iteration

After iteration:
- [ ] Document what changed and why
- [ ] Predict what should be different in next test
- [ ] Test the change specifically
