# TimeTraveler: Temporal Strategy Planning with Time Dictionary for Streaming Video Understanding

[Paper](https://arxiv.org/abs/2611.10337) · First posted 2026-11-07 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

"Tell me when the car stops" cannot be answered now; a streaming model has to know which questions to answer from the past and which to wait for.

## Proactivity Signal

Each moment of the stream is stored as a timestamped caption. A planner routes each user question to past, present or future evidence; for future questions a small yes/no gate polls new captions and answers once the condition is met.

## Evaluation Setup

Training-free, evaluated on OVO-Bench and StreamingBench. With Qwen3-VL-8B, OVO-Bench overall rises from 51.70 to 58.02 and StreamingBench from 59.33 to 64.51. On StreamingBench Proactive Output the gate lifts accuracy from 52.40 to 62.90, while memory without the gate drops to 45.20. The planner agrees with one human annotator on 79.3% of 150 sampled queries.

## Key Limitations

The user always asks first, so this times an answer rather than choosing to help. Caption errors propagate, each query takes one route, and the gate fires on its first positive. Visual only; no real users. The code repository holds only a README.

## Use For

Routing standing streaming questions to past, present or future evidence, with an explicit wait gate.
