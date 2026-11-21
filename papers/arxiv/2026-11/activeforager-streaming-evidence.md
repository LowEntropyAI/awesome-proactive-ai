# Look Closer, Look Back, or Wait for Agentic Streaming Video Understanding

[Paper](https://arxiv.org/abs/2611.24267) · [Code](https://github.com/TiezMind/ActiveForager) · First posted 2026-11-18 · Checked 2026-11-21. Paper and accessible artifact listings reviewed; no rerun.

## Why It Matters

A four-way evidence policy keeps the current frame window separate from verified evidence retrieved from history.

## Proactivity Signal

For an existing video question, the agent chooses whether to answer, zoom in, recall an earlier event, or wait for new evidence.

## Evaluation Setup

Benchmarks include OVO-Bench and zero-shot Video-Holmes; the paper compares frozen and trained routing against simple-window baselines.

## Key Limitations

Evidence gathering is conditioned on an explicit question. Released manifests depend on separately obtained media; fine-tuned weights were not verified.

## Use For

Compare the conditions that trigger intervention with those that justify waiting.
