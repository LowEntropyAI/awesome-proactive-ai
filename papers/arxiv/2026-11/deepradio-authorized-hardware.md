# DeepRadio: A Human-Agent Workspace for Physical Radio Development

[Paper](https://arxiv.org/abs/2611.09418) · First posted 2026-11-06 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

An agent that builds radio systems can push a software decision straight onto transmitting hardware unless it knows when to stop and hand control back.

## Proactivity Signal

The agent places its own checkpoints: it asks for missing parameters, and before consequential actions it applies a Deny / Confirm / Propose / Allow policy. Hardware and RF operations need an approved plan, flowgraph edits arrive as editable patches, and only local reversible actions run automatically.

## Evaluation Setup

Seven atomic software-defined-radio tasks, ten runs each by one experienced operator, completed 67 of 70 runs with every constraint satisfied. In a within-subject study with 20 participants on one task, 19 reached a verified physical deployment with DeepRadio against 10 with Codex in GNU Radio Companion (exact McNemar p = .004); median time to verified success was 14.6 against 34.2 minutes.

## Key Limitations

Users initiate every turn, so the initiative studied is when to return control, not whether to offer help. One user-study task, mostly student participants, perceived rather than calibrated confidence, and a descriptive time comparison. Code is promised after publication.

## Use For

An authorization ladder for agents whose actions reach physical hardware.
