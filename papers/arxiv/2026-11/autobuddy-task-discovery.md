# AutoBuddy: Evaluating Proactive, Always-On Agents on Task Discovery and Execution in a Simulated Workplace

[Paper](https://arxiv.org/abs/2611.12393) · First posted 2026-11-09 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

Most agent benchmarks hand the agent its task; an always-on assistant first has to notice which obligations are actually the user's.

## Proactivity Signal

With no request, the agent reads one employee's mail, chat, calendar and files, decides which open obligations belong to that person (skipping answered requests, colleagues' work and background noise), then carries out each one in the systems where it lives.

## Evaluation Setup

One generated six-month organisation yields 120 ground-truth tasks over 94 actor-days of 44 employees; 41% are business-system operations. Seventeen backbones run three times each in one reference harness. Discovery is matched against the cited request record and execution by diffing workspace state, with no LLM grader. End-to-end scores range from 0.234 to 0.698; the best backbone reaches discovery F1 0.925, and the strongest models score 0.45–0.56 on business-system tasks against 0.67–0.75 on collaboration tasks.

## Key Limitations

One synthetic organisation with LLM-written documents, one agent architecture and no real users. Discovery runs once per actor-day and every matched task is executed, so interruption timing and whether the person wanted the work done are not tested. No code or benchmark link was found.

## Use For

Testing whether an always-on agent can find the user's own pending work without being told, with false alarms penalised.
