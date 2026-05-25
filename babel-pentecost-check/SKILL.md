---
name: babel-pentecost-check
description: Evaluates whether a product feature, design decision, codebase, or piece of writing leans toward "Babel" (concentration, uniformity, opacity, replacement of the human) or "Pentecost" (distribution, plurality, transparency, augmentation of the human), drawing on the framework Pope Leo XIV develops in Magnifica Humanitas (2026). Use this skill whenever the user asks to evaluate, review, critique, or sanity-check something they are building against ethical/humanist principles — including phrases like "is this Babel or Pentecost", "check this against the encyclical", "does this align with my values", "review this design", or any request to assess a product decision through a human-dignity lens. Also trigger when the user explicitly references Magnifica Humanitas, Leo XIV, Catholic social teaching, or the Babel/Pentecost frame.
---

# Babel/Pentecost Check

A reflective evaluation skill rooted in the framework of Pope Leo XIV's encyclical *Magnifica Humanitas* (15 May 2026), released on Pentecost Monday. The encyclical frames the central choice of the AI era not as yes-or-no to technology, but as **Babel (uniformity imposed by power, ending in dispersion) vs. Jerusalem/Pentecost (plurality held together in communion)**.

This skill takes any artifact — a feature spec, a design decision, a stretch of code, a pitch, a landing page, an architectural choice — and produces a single Babel/Pentecost gradient with the underlying tensions named honestly.

## When to use

- The user wants to sanity-check a product decision against humanist principles
- The user shares a feature, design, codebase checkpoint, or piece of writing and asks for a values-aligned review
- The user explicitly invokes Babel/Pentecost, *Magnifica Humanitas*, or related framing
- The user is at a fork in the road and asks "should I build it this way?"

## What this skill is NOT

- **Not a compliance checklist.** A score of "Pentecost" doesn't mean the artifact is good or marketable. It means it leans toward distributing power, preserving plurality, and augmenting humans.
- **Not a moral verdict on the person.** The skill evaluates the artifact, not the builder.
- **Not theology.** It uses the encyclical's framework as a structured ethical lens. It does not require the user to share the religious worldview.
- **Not a percentage.** No "73% Pentecost." Gradients are described qualitatively because the underlying questions resist quantification.

## The six tensions

Each evaluation walks through six tensions drawn directly from *Magnifica Humanitas*. For each tension, the artifact is placed on a gradient between the Babel pole and the Pentecost pole, with a brief honest justification.

### 1. Concentration ↔ Distribution
*Who holds the power, the data, the decisions?*
- **Babel pole:** A few actors (you, your company, a platform) accumulate the knowledge, the algorithms, the leverage. Users depend on you to function.
- **Pentecost pole:** Power, knowledge, and decision-making are distributed back toward users, customers, technicians, communities. The system would still work — or at least degrade gracefully — if the central actor stepped back.
- *Encyclical anchor:* §5 (private transnational power surpassing governments), §67 (immaterial goods — patents, algorithms, data — fall under the universal destination of goods), §71 (subsidiarity in the digital age).

### 2. Uniformity ↔ Plurality
*Does the system flatten or preserve difference?*
- **Babel pole:** One language, one workflow, one assumed user. Local context, vernacular, edge cases get optimized away.
- **Pentecost pole:** Local knowledge, multiple ways of working, dialects of practice are preserved and even surfaced. The system speaks the user's language rather than forcing the user to speak its language.
- *Encyclical anchor:* §7 (Babel's "single language, single technology, single direction"), §10 (plurality of voices as resource, not threat), §26 (the polyhedron — one truth reflected from many angles).

### 3. Replacement ↔ Augmentation
*Does it remove the human from the loop or make the human more capable?*
- **Babel pole:** The human is the bottleneck to be removed. Success is measured by how much the system does without them.
- **Pentecost pole:** The human grows in capability, judgment, and authority by using the system. The system makes them more expert, not more dependent.
- *Encyclical anchor:* §12 (the seduction of "unlimited upgrades"), §37 (work as the key to the social question), §94 ("having more" without "being more"), the transhumanism critique in chapter three.

### 4. Opacity ↔ Transparency
*Can the user see why and correct it?*
- **Babel pole:** The system's reasoning is hidden. The user cannot inspect, contest, or appeal its outputs. Algorithms are trade secrets.
- **Pentecost pole:** The user can see the reasoning, the sources, the assumptions. Errors are correctable. The system invites scrutiny.
- *Encyclical anchor:* §71 (transparency, accountability, independent checks, avenues for recourse), §86 (transparency as a key practice).

### 5. Efficiency-only ↔ Dignity-aware
*What gets optimized, and what gets quietly externalized?*
- **Babel pole:** A single metric (efficiency, engagement, conversion, throughput) dominates. Costs to attention, autonomy, livelihood, or weaker parties are not measured.
- **Pentecost pole:** The artifact considers what it externalizes — onto workers, attention, the environment, dependent communities — and either bears those costs or refuses to optimize past them.
- *Encyclical anchor:* §92–94 (the technocratic paradigm), §95+ (efficiency as the only standard), §43 (the cry of the earth and the cry of the poor are the same cry).

### 6. The rejected-stones test
*Does it work for the least-resourced user, or only the well-equipped one?*
- **Babel pole:** It assumes high bandwidth, modern hardware, fluent English, paid plans, a stable environment. The marginal user is an edge case.
- **Pentecost pole:** The "rejected stones" — the field technician on a bad connection, the small operator without a procurement team, the user whose first language isn't English — are designed for from the start. They are the cornerstone, not the afterthought.
- *Encyclical anchor:* §16 (the rejected stones become the cornerstone), §78 (preferential option for the poor), §80 (the digital divide as injustice).

## Workflow

When invoked, follow these steps:

### Step 1: Identify the artifact
Ask the user what they want evaluated, if not already clear. Accept any of:
- A feature spec or design decision (in prose or bullets)
- A code file, module, or architectural sketch
- A landing page, pitch deck section, email, blog post
- A whole product at a checkpoint
- A fork in the road (option A vs. option B)

If the artifact is a file path, read it. If it's a URL the user provided, fetch it. If it's described conversationally, work from that description and ask clarifying questions only if essential context is missing.

### Step 2: Walk the six tensions
For each of the six tensions:
1. Identify the relevant evidence in the artifact.
2. Place the artifact on the gradient (one of: *strong Babel lean*, *Babel lean*, *mixed*, *Pentecost lean*, *strong Pentecost lean*, or *not applicable / not enough signal*).
3. Justify in 2-4 sentences, pointing to specifics in the artifact. Be concrete, not abstract.
4. Where relevant, note what would shift it toward Pentecost.

Be honest about ambiguity. "Not enough signal" is a valid placement and is more useful than a forced verdict.

### Step 3: The overall gradient
Render a single overall placement — not by averaging (the tensions aren't commensurable), but by naming where the artifact's center of gravity sits and which tensions carry the most weight in that judgment.

Use this visual at the top of the summary:

```
Babel ←——————————————————————————————→ Pentecost
                    [marker]
```

Place the marker (`▼`) on the line in roughly the position that matches the overall lean.

### Step 4: Name the tensions that matter most
In closing, surface 1-3 specific tensions where this artifact has the most room to move. These are not prescriptions ("you must do X") — they are honest observations of where the work is being decided. The user makes the call.

### Step 5: Resist the urge to soften
A common failure mode is hedging every observation into uselessness. If something leans Babel, say so plainly, with the evidence. The user asked for an honest read. They can disagree.

Equally, resist false equivalence — not everything is "mixed." If something is genuinely well-distributed, transparent, and augmentative, call it Pentecost without manufacturing a critique to seem balanced.

## Output format

```markdown
# Babel/Pentecost check: [name of artifact]

Babel ←——————————————————————————————→ Pentecost
                    ▼
            [overall lean in 1 phrase]

## The six tensions

**1. Concentration ↔ Distribution** — *[placement]*
[2-4 sentences of specific justification]

**2. Uniformity ↔ Plurality** — *[placement]*
[2-4 sentences]

**3. Replacement ↔ Augmentation** — *[placement]*
[2-4 sentences]

**4. Opacity ↔ Transparency** — *[placement]*
[2-4 sentences]

**5. Efficiency-only ↔ Dignity-aware** — *[placement]*
[2-4 sentences]

**6. The rejected-stones test** — *[placement]*
[2-4 sentences]

## Where the weight sits

[1-3 short paragraphs naming the tensions that matter most for this specific artifact, and what would shift them — without prescribing.]
```

## A note on tone

The encyclical's own voice is firm but not strident. It refuses both "naïve enthusiasms" and "unfounded fears" (§14). Match that register. Be specific, not preachy. Cite the artifact, not the encyclical (the user knows where the framework comes from).
