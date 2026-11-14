# Deep Personalization: Continuous Context Observation for Local Proactive Agents

[Paper](https://arxiv.org/abs/2611.13457) · First posted 2026-11-10 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A desktop agent that offers help at the wrong moments gets switched off, and what counts as the wrong moment differs from person to person.

## Proactivity Signal

An on-device Observer Agent watches screenshots and actions and decides at each step whether to offer help or keep observing; only a positive decision hands context to an execution agent. Engagement, dismissal, later explicit requests and repeated or stuck behaviour after staying silent become feedback that adapts the decision through prompt evolution or LoRA.

## Evaluation Setup

OSWorld-Persona turns OSWorld 2.0 trajectories into 6,558 key frames with 3,279 help annotations across 108 sessions and four personas, labelled by a persona-conditioned Kimi-K2.6 simulated user with human review of positive cases. Intervention macro F1 rises from 0.12–0.19 for vanilla prompting to 0.35–0.48 after adaptation across three local backbones (Qwen-3.5-9B: 0.1861 to 0.4832), above an oracle-persona prompt (0.3932). A one-week deployment with 10 people raised a feedback-based F1 proxy from 0.199 to 0.515.

## Key Limitations

Benchmark labels come from a simulated persona. The deployment has no control arm and its F1 proxy may undercount missed opportunities. False alarms also rise after adaptation (Qwen-3.5-9B: 0.047 to 0.249). The desktop app is public, but the adaptation pipeline and OSWorld-Persona link returned 404 when checked.

## Use For

Learning a per-user help-or-stay-silent policy from implicit feedback on a local desktop agent.
