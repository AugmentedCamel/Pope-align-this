# Babel/Pentecost Check

A Claude skill that evaluates whether a product feature, design decision, codebase, or piece of writing leans toward **Babel** (concentration, uniformity, opacity, replacement of the human) or **Pentecost** (distribution, plurality, transparency, augmentation of the human).

Drawn from the framework Pope Leo XIV develops in [*Magnifica Humanitas*](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) (15 May 2026), the first papal encyclical on safeguarding the human person in the age of artificial intelligence.

> *"The primary choice is not between a 'yes' or 'no' to technology, but rather between constructing Babel or rebuilding Jerusalem; between a power that claims to dominate the heavens and a people who work together in the presence of God to rebuild the walls of fraternal coexistence."*
> — *Magnifica Humanitas* §9

## Why this exists

The encyclical was released to the public on Pentecost Monday — the feast that liturgically resolves Babel. In Genesis 11, God scatters humanity because their tower-building was prideful and self-sufficient. In Acts 2, the Spirit descends and the apostles speak in many tongues — but everyone *understands*. Babel = one language imposed, ending in dispersion. Pentecost = many languages preserved, ending in communion.

The encyclical's core claim: technology is never neutral. It takes on the characteristics of those who design, finance, regulate, and use it. The question of the AI era is not whether to build, but **what kind of city we are building**.

This skill turns that question into something checkable. It walks an artifact through six tensions and produces a single Babel/Pentecost gradient with the underlying trade-offs named honestly.

## The six tensions

1. **Concentration ↔ Distribution** — Who holds the power, data, and decisions?
2. **Uniformity ↔ Plurality** — Does the system flatten or preserve local context?
3. **Replacement ↔ Augmentation** — Does it remove the human from the loop or make the human more capable?
4. **Opacity ↔ Transparency** — Can the user see why and correct it?
5. **Efficiency-only ↔ Dignity-aware** — What gets quietly externalized?
6. **The rejected-stones test** — Does it work for the least-resourced user, or only the well-equipped one?

Each tension is anchored in specific passages of the encyclical. Full references are in [`babel-pentecost-check/references/encyclical-anchors.md`](babel-pentecost-check/references/encyclical-anchors.md).

## What it produces

For any artifact, the skill renders:

```
Babel ←——————————————————————————————→ Pentecost
                    ▼
            [overall lean in one phrase]
```

…followed by a placement on each of the six tensions, 2–4 sentences of specific justification per tension, and a closing paragraph naming where the artifact's center of gravity sits.

It does **not** produce a percentage score. The underlying questions resist quantification, and false precision is its own kind of Babel.

## What this skill is NOT

- **Not a compliance checklist.** A "Pentecost" lean doesn't mean the artifact is good or marketable — it means it leans toward distributing power, preserving plurality, and augmenting humans.
- **Not a moral verdict on the builder.** It evaluates the artifact, not the person.
- **Not theology.** It uses the encyclical's framework as a structured ethical lens. It does not require the user to share the religious worldview.

## Installation

### Claude Code

```bash
claude skill install path/to/babel-pentecost-check.skill
```

Or clone this repo and install the folder directly:

```bash
git clone https://github.com/AugmentedCamel/Pope-align-this.git
claude skill install ./Pope-align-this/babel-pentecost-check
```

### Usage

Once installed, the skill triggers automatically when you ask Claude to evaluate a feature, design decision, or piece of writing against humanist principles. Examples:

- *"Check this pricing model against Babel/Pentecost."*
- *"Run the encyclical check on this landing page."*
- *"Is this design Babel or Pentecost?"*
- *"Review this architectural choice against Magnifica Humanitas."*

## References

- **Encyclical:** [*Magnifica Humanitas* — Pope Leo XIV (15 May 2026)](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html)
- **Papal tweet on release:** [@Pontifex (25 May 2026)](https://x.com/Pontifex/status/2058888313029685400)

## About this skill

This is my two cents to humanity — a small, concrete attempt to make the encyclical's framework usable by builders. The questions it asks are not new; the encyclical itself stands on 135 years of Catholic social teaching going back to *Rerum Novarum* (1891). What this skill adds is just a thin runtime: a way to put your work in front of those questions before you ship it, while there is still time to choose.

If it helps even one product decision tilt away from Babel, it has done its job.

— Mika Meel ([mikameel](https://github.com/mikameel))

## License

MIT. Use it, fork it, improve it. The framework belongs to no one and to everyone — that is rather the point.
