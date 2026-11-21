# ALIVE: Making Streaming Video Models Interactive

[Paper](https://arxiv.org/abs/2611.21366) · [Project](https://lijinzhao30.github.io/ALIVE/) · [Code](https://github.com/lijinzhao30/ALIVE) · [Model](https://huggingface.co/ALIVE-Team/ALIVE) · First posted 2026-11-16 · Checked 2026-11-21. Paper and accessible artifact listings reviewed; no rerun.

## Why It Matters

Contrastive supervised training and behavior-aligned RL teach response, waiting and feedback-seeking over multiple streaming turns.

## Proactivity Signal

The model can watch for a requested event, track changing instructions, and ask for a missing fact or user action before finishing.

## Evaluation Setup

FSI-Bench evaluates identifying a missing prerequisite, seeking help from the user and completing the task; the paper also reports four existing benchmarks.

## Key Limitations

These results cover monitored or delegated tasks; release of a demo and checkpoint does not imply open evaluation and training data.

## Use For

Compare how systems recognize and resolve the need for a question.
