# Duopra: From Full-Duplex Conversation to Full-Duplex Agency

[Paper](https://arxiv.org/abs/2611.25773) · [Project](https://cychen2003.github.io/duopra/) · [Code](https://github.com/cyChen2003/duopra) · [Model](https://huggingface.co/Chechen123/Duopra) · [Dataset](https://github.com/DanielLin94144/Full-Duplex-Bench/tree/main/v3) · First posted 2026-11-19 · Checked 2026-11-21. Paper and accessible artifact listings reviewed; no rerun.

## Why It Matters

A full-duplex interface learns when to initiate self-contained backend requests or call tools directly as spoken requests evolve.

## Proactivity Signal

Starts a tool call when the spoken request is sufficiently specified and revises the arguments if the user corrects them.

## Evaluation Setup

The paper evaluates timely execution and speech behavior with Full-Duplex-Bench v3 and v1; it compares direct and delegated execution.

## Key Limitations

An explicit task is supplied. The checkpoint is gated even though the repository and released benchmark files are public.

## Use For

Compare the conditions that trigger intervention with those that justify waiting.
