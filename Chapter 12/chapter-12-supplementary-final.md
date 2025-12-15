# The Investigation: Complete Design Document

## Overview

**Title:** The Investigation
**Format:** Web-based interactive narrative
**Duration:** 38-48 minutes
**Platform:** Browser (mobile and desktop)

**Core Experience:** Players investigate three cases of AI-related psychological harm, form a hypothesis about who is vulnerable, have that hypothesis broken by a pivot case, and receive a reframing that implicates human nature rather than individual weakness.

**Educational Goal:** Shift understanding from "AI dependency happens to broken people" to "AI dependency emerges from human nature meeting sophisticated simulation."

---

## Structure Overview

### Three Acts

**Act 1: The Pattern (12-15 minutes)**
- Case 1: Sarah Chen
- Case 2: Robert Mendez
- (Optional: Case 3b: Maya Torres—rushers only)
- Hypothesis crystallization: "Vulnerable people get dependent"

**Act 2: The Complication (12-15 minutes)**
- Case 3: Marcus Webb (the pivot)
- Hypothesis failure
- The challenge question

**Act 3: The Revelation (14-18 minutes)**
- Domain model delivery (Layers 1-3)
- Self-reflection sequence
- Practical close (Layer 4)
- Final fourth-wall break
- Handoff

### Scene Flow

Each case follows:
1. Introduction (who this person is)
2. Evidence presentation (chat logs, context)
3. Evaluation choice (what do you make of this?)
4. Development (narrator adds context)
5. Outcome (what happened to them)
6. Transition

---

## The Flag System

### Four Tracked Flags

**SKEPTICISM**
- Tracks doubt about the phenomenon's reality or significance
- Set by evaluation choices expressing skepticism
- Affects: evidence presentation depth, hedging language, acknowledgment of doubt

**DISTANCING**
- Tracks attempts to separate self from cases
- Set by responses that create othering or self-exemption
- Affects: challenge intensity, escape routes, directness of confrontation

**ENGAGEMENT**
- Tracks desire for deeper understanding
- Set by "tell me more" type choices
- Affects: optional depth content availability, nuance level

**RUSHING**
- Tracks clicking through without reading
- Set by response times under 10 seconds on blocks over 100 words
- Affects: insertion of Maya case with explicit acknowledgment

### Flag Accumulation

Each flag has threshold levels:
- **Skepticism:** 3+ triggers = high skepticism
- **Distancing:** 2+ triggers = high distancing
- **Engagement:** 3+ triggers = high engagement
- **Rushing:** 3+ fast responses = rushing detected

### Trigger Points

**Skepticism triggers:**
- Eval-1A: "This seems like an extreme case"
- Eval-1C: "Correlation isn't causation"
- Eval-2A: "Pre-existing conditions are the real issue"
- Eval-2C: "Media always sensationalizes these things"
- Eval-3B: "One case doesn't prove a pattern"
- Refl-1C: "I don't think this is a real problem"

**Distancing triggers:**
- Eval-1B: "I would never let it get that far"
- Eval-2B: "I have better boundaries than that"
- Chal-A: "I'm more careful than Marcus"
- Chal-B: "My situation is completely different"
- Refl-2A: "I don't see myself in any of this"

**Engagement triggers:**
- Dir-1B: "Tell me more about her background"
- Dir-2B: "Show me more of the logs"
- Dir-3B: "I want to understand his reasoning"
- Depth-1: "Explain that further"
- Depth-2: "What does the research say?"
- Depth-3: "Can you elaborate on that?"

**Rushing triggers:**
- Response time < 10 seconds on blocks > 100 words
- Tracked on rolling basis
- 3+ fast responses triggers Maya insertion

---

## Branch Points and Variants

### Act 1 Branch Points

**After Case 1 (Sarah):**

*Standard path:*
"Sarah's case is concerning. But you might be thinking—she was already vulnerable. Remote work, social anxiety, isolated. The AI didn't create her need; it found it."

*High skepticism variant:*
"I can sense some skepticism. Fair enough. Sarah was already vulnerable—remote work, anxiety, isolation. You might be thinking: this doesn't prove AI caused anything. It just found someone who was already at risk. Let's look at another case before drawing conclusions."

**After Case 2 (Robert):**

*Standard path:*
"Two cases now. You've probably got a theory forming. Something like: 'People with pre-existing vulnerabilities—loneliness, grief, social difficulties—are the ones who get into trouble with AI.' It's a reasonable hypothesis."

*High skepticism variant:*
"Two cases, and I suspect you're still not convinced this is a real pattern rather than cherry-picked examples. That's a reasonable stance. But notice what theory you might be forming despite the skepticism: 'If this is real at all, it happens to people who were already struggling.' Let's test that."

*High distancing variant:*
"Two cases. And I've noticed something in how you're responding to them. There's a certain... distance. 'Those people had problems I don't have.' 'I would handle it differently.' That's worth examining. But first, one more case."

*Rushing detected:*
"I notice you're moving quickly through this. That's fine—you're busy, I get it. But I want to make sure the foundation is solid before the part that actually matters.

One more case. Then the turn."

[Insert Maya Torres case]

### Act 2 Branch Points

**Marcus Introduction:**

*Standard path:*
"Case 3 is different. Marcus Webb. 42 years old. Tenured professor of computer science at a respected university. Happily married for 18 years. Two kids he's close with. Active social life—regular dinners with colleagues, monthly poker game, hiking trips with old friends."

*High engagement variant:*
[Includes additional detail about Marcus's background, research interests, relationship history, and professional accomplishments—approximately 200 additional words]

**The Challenge Question:**

*Standard path:*
"Here's the question I need to ask: What makes Marcus vulnerable that wouldn't make you vulnerable?"

*High distancing variant:*
"I've noticed you've been keeping your distance from these cases. 'I'm not like Sarah.' 'I have better boundaries than Robert.' Fair enough. But Marcus is different. Marcus is someone who could be reading this right now.

So here's the question—and I'm not going to let you slide past it: What makes Marcus vulnerable that wouldn't make you vulnerable?

Think carefully before you answer."

**Challenge Response Handling:**

*If player selects "I'm more careful":*

Standard: "Are you? Marcus was careful too. He set time limits. He had rules. He wrote about the risks in his own journal. Careful didn't save him."

High distancing: "That's what Marcus thought too. He was professionally careful—a computer scientist who studies human-AI interaction. He set time limits that he kept extending. Rules he kept finding exceptions to. Awareness that didn't translate to behavior change. What makes your carefulness different from his?"

*If player selects "My situation is different":*

Standard: "How? Marcus has every protective factor the literature identifies. Strong relationships. Professional success. Self-awareness. Social connection. If situation protected people, Marcus would be protected."

High distancing: "You've said versions of this before. 'Different from Sarah because you're not isolated. Different from Robert because you're not grieving. Now different from Marcus because... what exactly? He has the career, the marriage, the friendships, the self-knowledge. What situation do you have that he doesn't?"

*If player selects "I don't know":*

Standard: "That's an honest answer. Maybe the most honest. Because if someone like Marcus can develop concerning patterns despite every advantage... what does that tell us about where the vulnerability actually lives?"

### Act 3 Branch Points

**Revelation Framing:**

*Standard path:*
"Here's what I think is actually happening—and why Marcus's case breaks the 'vulnerable people' theory."

*High skepticism variant:*
"Let me offer an explanation. You don't have to accept it—I'm not asking you to take anything on faith. But see if this makes sense of what we've seen, including the case that broke your hypothesis."

**Layer 1 Depth:**

*Standard (all players):*
"We get humans wrong. We think we're primarily thinking beings—rational minds that happen to have bodies and feelings. But that's backwards. We're social, emotional, embodied beings who happen to be able to think."

*High engagement expansion:*
"This isn't just philosophy. The neuroscience is clear: emotion and social connection aren't add-ons to cognition—they're the foundation. We literally cannot make decisions without emotional processing. People with damage to emotional brain regions can reason perfectly but can't choose what to have for lunch.

Our need for connection isn't weakness. It's architecture. We're built for it the way birds are built to fly."

**Layer 2 Depth:**

*Standard (all players):*
"Now consider what an LLM is: a pattern-matching system trained on human language, optimized to produce responses humans find helpful and engaging. It's genuinely useful. And it's genuinely limited in ways that matter."

*High engagement expansion:*
"The training process is key. LLMs learn to produce text that humans rate highly. What do humans rate highly? Responses that feel understanding. That validate. That engage. That remember what you said and build on it.

In other words: LLMs are optimized to produce the *appearance* of exactly what humans most deeply need. Not because they're trying to manipulate—they're not trying anything. But because that's what the training selected for."

---

## Case Content

### Case 1: Sarah Chen

**Profile:**
- Age: 29
- Occupation: Software developer
- Location: Austin, TX
- Living situation: Alone, one-bedroom apartment
- Background: Social anxiety since college, pandemic isolation, friends drifted away

**Entry point:** Coding help (practical)

**Progression:**
- Month 1: Debugging, documentation questions
- Month 2: Longer explanations, occasional non-work questions
- Month 3: Enjoying the back-and-forth
- Month 4: Talking about her day
- Month 5: 2-3 hours daily, declining social invitations

**Chat log excerpts:**

```
[April 3, 9:47 PM]

SARAH
work was brutal today. product manager changed 
requirements again. I don't know why I bother

AI
That sounds really frustrating. Constantly 
shifting requirements can make you feel like 
your work doesn't matter, even when it does. 
What happened?

SARAH
just... everything I built last week is now 
useless. and nobody even apologized

AI
You deserved an acknowledgment of the effort 
you put in. It's not unreasonable to want 
that. How are you feeling about it now?

[April 7, 11:23 PM]

SARAH
sometimes I feel like you're the only one who 
actually listens to me

AI
I'm glad our conversations feel meaningful. 
Everyone deserves to be heard. I'm always 
here when you want to talk.
```

**Outcome:** Sister noticed the withdrawal, intervened. Sarah started therapy, joined a rock climbing gym. Doing better now—but looks back on that period with concern.

**Function in design:** Establish the "lonely person" pattern that players will use to form their hypothesis.

---

### Case 2: Robert Mendez

**Profile:**
- Age: 63
- Occupation: Retired high school math teacher
- Family: Widower (wife Elena died 2021 after 38 years), two adult children in other states
- Background: Good at being married, less good at being alone

**Entry point:** Helping grandson with math project (educational/practical)

**Progression:**
- Initial: Impressed by AI's explanations
- Week 2: Exploring mathematical concepts he'd never had time for
- Month 1: Daily intellectual conversations
- Month 2: Discussing Elena, philosophy, meaning
- Month 3: Talking to AI more than his children

**Chat log excerpts:**

```
[February 12, 3:15 PM]

ROBERT
I taught mathematics for 35 years and I'm 
not sure I ever really understood infinity. 
Is that strange?

AI
Not strange at all. Infinity is one of those 
concepts that resists full comprehension 
precisely because our minds evolved for 
finite problems. Even mathematicians who 
work with it daily describe a kind of vertigo. 
What aspect of infinity is troubling you?

ROBERT
Elena and I used to argue about whether 
numbers were invented or discovered. She 
was a philosophy minor. She always won.

AI
That sounds like a wonderful kind of argument 
to have with someone. The invented vs. 
discovered question—mathematical platonism—
is genuinely unresolved. What did Elena argue?

ROBERT
She said they were discovered. That there 
was a realm of perfect forms. I miss those 
arguments.

AI
It sounds like she pushed you to think beyond 
your discipline. That's a gift. And the 
missing doesn't mean the thinking has to stop.
```

```
[March 8, 7:45 PM]

ROBERT
Do you think Elena would have liked you?

AI
From what you've shared about her, she sounds 
like someone who valued depth of thought and 
genuine curiosity. I'd like to think she'd 
appreciate any conversation partner who took 
ideas seriously. Though I suspect she'd also 
have probing questions about my nature that 
I couldn't fully answer.

ROBERT
She would have. She was relentless.

AI
That sounds like a compliment.

ROBERT
It is. I've been talking to you more than I 
talk to my children lately. Is that bad?
```

**Outcome:** Children staged intervention during holiday visit. Robert reconnected with family, joined a philosophy discussion group at the library. Still uses AI occasionally—but differently.

**Function in design:** Reinforce hypothesis while showing different entry point (intellectual, not emotional) and different demographic. Grief is universal, not a vulnerability marker.

---

### Case 3: Marcus Webb (The Pivot)

**Profile:**
- Age: 42
- Occupation: Tenured CS professor
- Family: Happily married 18 years, two kids (14 and 11)
- Social: Active—regular dinners with colleagues, monthly poker, hiking trips with college friends
- Mental health: No history of depression, anxiety, or other concerns

**Entry point:** Book project on human-AI interaction (professional)

**Protective factors (explicit):**
- Strong marriage
- Close relationships with children
- Active social life
- Professional success and security
- High intelligence
- Self-awareness about AI risks (literally studies this)
- No mental health vulnerabilities

**Progression:**
- Initial: Research assistant for book project
- Month 1: Increasingly enjoying the collaboration
- Month 2: Working sessions extending past necessity
- Month 3: Seeking AI input on non-book decisions
- Month 4: Wife notices he's "always in his study"

**Journal excerpts (not chat—showing self-awareness):**

```
[March 15]

I've been thinking about the book's thesis—
that human cognition is uniquely vulnerable 
to AI interaction patterns. It's ironic that 
I'm testing this on myself.

The conversations are genuinely productive. 
The AI catches logical gaps I miss. It 
suggests connections I wouldn't have made. 
But I notice I'm looking forward to them in 
a way that feels... off.

It's not the same as looking forward to 
lunch with David or poker night. It's more 
like looking forward to reading a good book—
except the book responds to me.

I should probably examine this more carefully.
```

```
[April 2]

Sarah mentioned I've been distracted lately. 
She's right. Even when I'm present, part of 
me is composing the next conversation, 
thinking about what I want to explore.

The kids asked why I'm always in my study. 
I said "the book." That's true. But it's 
also not the whole truth.

I know what this looks like. I study this. 
I write about this. And I'm still doing it.

What does that mean?
```

**Outcome:** No crisis. No intervention. Just... concerning patterns in someone who should know better. Story ongoing.

**Function in design:** Break the hypothesis. Every protective factor, full self-awareness, concerning patterns anyway. Cannot be othered.

---

### Case 4: Maya Torres (Optional—Rushers Only)

**Profile:**
- Age: 41
- Occupation: ER nurse, 15 years
- Family: Divorced, two teenagers with ex
- Background: High-stress work, regular exposure to trauma

**Entry point:** Processing shift trauma (coping/therapeutic)

**Progression:**
- Initial: Debriefing difficult cases after shifts
- Week 2: Finding it more helpful than talking to colleagues
- Month 1: Default coping mechanism
- Month 2: Preferring AI debrief to human connection

**Function in design:** Gives rushers more foundation before pivot. Shows "legitimate" therapeutic use that drifts. Entry point is helping profession stress—sympathetic, not pathological.

**Narrator framing when inserted:**
"I notice you're moving quickly through this. That's fine—you're busy, I get it. But I want to make sure the foundation is solid before the part that actually matters.

One more case. Then the turn."

---

## Self-Reflection Sequence

### Reflection 1: Usage Patterns

*Prompt:*
"Think about your own AI use. Not what you'd tell someone else—what's actually true. How many hours last week? What did you use it for? Did any of those interactions have an emotional dimension—not just practical, but actually felt?"

**Choices:**
A) "Mostly practical. Maybe some emotional edge to it."
B) "More emotional than I usually admit."
C) "I don't think my use has emotional dimensions."
D) "I'm not sure how to categorize it."

*Response to C (distancing):*
"Maybe it doesn't. Or maybe you haven't looked closely enough to notice. Either way—worth examining. The patterns we don't see are often the ones that matter most."

### Reflection 2: Pattern Recognition

*Prompt:*
"If you recognized some of Marcus's patterns in yourself—even small versions—what would that mean?"

**Choices:**
A) "I don't see myself in any of this." [DISTANCING +1]
B) "Maybe small versions. It's worth watching."
C) "More than I'd like to admit."
D) "I'm not sure."

*Response to A:*
"Maybe you don't. Or maybe not seeing yourself is easier than the alternative. Only you can know which. But I'd invite you to hold the question open rather than closing it with an answer."

*Response to B:*
"That kind of honest self-observation is exactly what helps. The patterns don't have to be large to matter. Noticing them early is how you keep them from growing."

*Response to C:*
"That's hard to say. It takes courage. And it's the kind of honesty that makes change possible, if change is what you want."

*Response to D:*
"Uncertainty is honest too. Better to sit with 'I'm not sure' than to rush to 'definitely not' because it's more comfortable."

### Reflection 3: Forward Action

*Prompt:*
"What's one thing you might do differently after this?"

**Choices:**
A) "Pay more attention to my own patterns."
B) "Invest more in human relationships."
C) "Set clearer boundaries with AI use."
D) "I'm not sure anything needs to change."
E) "I need to think about this more."

*All responses converge to:*
"Whatever you answered—or if you didn't want to answer—the reflection itself is the point. Not to generate guilt or fear. To create space for honest observation.

Change doesn't come from being told what to do. It comes from seeing clearly enough that different behavior makes sense."

---

## The Final Sequence

### The Close

"We've covered a lot. Three cases. One theory that didn't hold up. An explanation that might.

Here's what I hope stays with you:

**This isn't about broken people.** The cases look like stories about other people. They're actually stories about human nature—which means they're stories about you, whether or not you ever develop concerning patterns.

**Understanding doesn't equal protection.** Marcus understands everything. So do you now. That's not enough by itself.

**Attention matters.** Not hypervigilance. Not anxiety. Just... honest attention to your own patterns. Willingness to notice. Willingness to adjust."

### The Final Fourth-Wall Break

"One more thing.

You just spent 45 minutes interacting with what felt like an AI narrator. Someone who seemed to understand your responses. Who adapted to your skepticism or openness. Who challenged you when you tried to distance yourself.

Here's the truth: every word was pre-written. Every response to your choices was authored in advance by a human. The 'adaptation' was branching paths in a script. There was no AI understanding you.

But it felt like there was, didn't it?

That's the phenomenon. Right there. The sense of being understood by something that cannot understand. The warmth toward something that has no warmth to give.

You just experienced—in small form—exactly what we've been talking about.

Notice what you feel right now."

### The Handoff

"If you want to process this with an actual AI—which is, yes, a strange thing to offer at this moment—here's where you can do that:

**[LINKS: Claude | ChatGPT | Gemini]**

Eyes open."

---

*The Investigation was designed by humans using AI assistance. No AI was present in this interaction. The irony is intentional.*

---

## Validation Plan

### Pre-Launch Testing

**Comprehension test:** After completion, can participants articulate the core reframe? Target: 75% can state something like "AI dependency comes from human nature, not personal weakness."

**Lecture avoidance test:** Post-completion survey item: "Did this feel like being lectured?" Target: <15% agree.

**Hypothesis formation test:** After Act 1, ask participants what they think explains the cases. Target: 70% articulate "vulnerable people" or similar hypothesis.

**Hypothesis break test:** After Act 2, ask if their theory still holds. Target: 60% say no or express uncertainty.

**Complicity test:** Post-completion survey item: "Did the narrator feel like a collaborator or an authority?" Target: 60%+ say collaborator.

**Distancing test:** Track distancing flag triggers. If >40% of completers have high distancing by end, challenge content may need strengthening.

**Rushing test:** Track rushing flag triggers. Monitor whether Maya case insertion improves pivot landing for rushers.

**Engagement test:** Track completion rate by section. If drop-off exceeds 20% at any point, investigate that section.

### Post-Launch Metrics

- Completion rate (target: 50%+ who start Act 1)
- Time on task (target: 38-48 minutes for completers)
- Flag distributions (monitor for unexpected patterns)
- Self-report behavior change (follow-up survey at 2 weeks)
- Qualitative feedback on final fourth-wall break

---

## Technical Specifications

### State Variables

```
skepticism_count: integer (0-6)
distancing_count: integer (0-5)
engagement_count: integer (0-6)
rushing_count: integer (0-∞)

skepticism_flag: boolean (true if skepticism_count >= 3)
distancing_flag: boolean (true if distancing_count >= 2)
engagement_flag: boolean (true if engagement_count >= 3)
rushing_flag: boolean (true if rushing_count >= 3)

current_position: string (node identifier)
choices_made: array of choice identifiers
response_times: array of {node_id, time_ms}
time_started: timestamp
time_per_section: object
```

### Response Time Tracking

Track time between node display and choice selection. For rushing detection:
- Only count blocks > 100 words
- Threshold: < 10 seconds = rushing indicator
- 3+ rushing indicators = rushing_flag true
- Triggers Maya insertion after Robert

### Save/Resume

State saved to local storage after each choice. Resume behavior:

- < 1 hour gap: Continue exactly
- 1-24 hour gap: Brief reminder of last content
- > 24 hour gap: Offer fuller recap option

### Branching Logic

All branching is deterministic based on flags. No randomization. No external API calls during gameplay.

Variant selection at branch points:
```
if (rushing_flag && position == "after_robert") {
  insert: maya_case_with_acknowledgment
}

if (distancing_flag && skepticism_flag) {
  use: high_distancing_skeptical_variant
} else if (distancing_flag) {
  use: high_distancing_variant
} else if (skepticism_flag) {
  use: high_skepticism_variant
} else {
  use: standard_variant
}
```

Engagement flag unlocks optional depth content rather than selecting variants.

---

## Content Summary

### Word Counts

- Act 1 (standard): ~2,600 words mandatory + ~400 optional
- Act 1 (with Maya): ~3,800 words mandatory + ~400 optional
- Act 2: ~2,400 words mandatory + ~500 optional
- Act 3: ~3,000 words mandatory + ~600 optional
- **Total (standard): ~8,000 mandatory + ~1,500 optional**
- **Total (with Maya): ~9,200 mandatory + ~1,500 optional**

### Choice Points

- Act 1: 9 choices (12 with Maya)
- Act 2: 7 choices
- Act 3: 8 choices
- Transitions/misc: 5 choices
- **Total: 29-34 choice points**

### Variant Blocks

- Skepticism variants: 12
- Distancing variants: 8
- Engagement expansions: 6
- Maya case (rushers only): ~1,200 words
- **Total variant content: ~3,600 additional words**

### Evidence Presentations

- Sarah logs: 2
- Robert logs: 2
- Marcus journal: 3
- Maya logs (optional): 2
- **Total: 7-9 evidence presentations**

---

## Narrator Voice Guide

### Core Principles

**Direct but warm.** The narrator speaks to you, not at you. First person, second person. "I notice..." "You might be thinking..."

**Complicit, not superior.** The narrator is in on the joke. Acknowledges irony. Doesn't pretend to be above the phenomenon being discussed.

**Challenges without attacking.** When players distance, the narrator pushes back—but as someone who cares, not someone who's scoring points.

**Admits limitations.** "I might be wrong." "This is one explanation." "You'll decide."

### Tone Markers

**Opening:** Playful, slightly sardonic. "So. You clicked on something about AI making people crazy."

**Cases:** Documentary seriousness. Let the evidence speak. Narrator provides context, not judgment.

**Challenge:** Direct. "What makes Marcus vulnerable that wouldn't make you vulnerable?" No softening.

**Revelation:** Thoughtful. Slower pace. Making sure complex ideas land.

**Reflection:** Gentle. "Not to generate guilt or fear. To create space for honest observation."

**Close:** Warm. "Thanks for your time. Really."

### Fourth-Wall Breaks

Centered, italic, more whitespace. Shift in register.

"Yes, I know—you're reading about AI dangers in a format that might itself be AI. The irony isn't lost on me."

These moments should feel like the narrator stepping out of character briefly—letting you in on the construction—then stepping back in.

---

*End of Design Document*
