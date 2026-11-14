# We Are What We Remember: Mental-State-Driven Memory for Long-Term Character Dialogue

[Paper](https://arxiv.org/abs/2611.16223) · First posted 2026-11-12 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A companion that remembers only topically similar facts misses the shared history that should shape what it brings up next.

## Proactivity Signal

Within each reply, a small trained reasoner reads persistent mental states of the character, the user and their relationship to anticipate latent needs, form an intention such as checking in about an interview, and recall the episodes that support it. The user always speaks first.

## Evaluation Setup

MemReal-Bench has 310 state-reasoning probes and 511 dialogue questions over 4,617 turns, synthesised from patterns in a month-long real-user collection. MindMem reaches 59.03% on state reasoning against 34.84% for A-Mem, and 82.58% on dialogue questions against 73.39%. Scoring uses an LLM judge that agreed with 10 human annotators on 80% of state-reasoning cases (κ 0.60).

## Key Limitations

Dialogues are synthetic and the judge is only moderately calibrated on the headline task. The "proactive intentions" shape what a reply says, not whether or when to reach out. Code and benchmark are promised upon acceptance.

## Use For

Relationship-aware memory for companions that should raise the right shared history.
