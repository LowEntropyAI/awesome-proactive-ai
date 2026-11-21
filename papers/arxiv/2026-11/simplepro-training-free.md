# SimplePro: A Simple Baseline for Proactive Video Understanding

[Paper](https://arxiv.org/abs/2611.23954) · First posted 2026-11-18 · Checked 2026-11-21. Paper and accessible artifact listings reviewed; no rerun.

## Why It Matters

Explicit reporting rules, bounded visual history and response history give a training-free baseline for streaming response timing.

## Proactivity Signal

A frozen VLM uses recent frames and prior answers to decide whether new evidence warrants an update; a filter suppresses repeats.

## Evaluation Setup

The paper evaluates multiple backbone sizes on OVO-Bench, StreamingBench-PO and ProactiveVideoQA.

## Key Limitations

The task supplies reporting instructions; this does not establish open-ended intent discovery. The work does not train new weights.

## Use For

Compare the conditions that trigger intervention with those that justify waiting.
