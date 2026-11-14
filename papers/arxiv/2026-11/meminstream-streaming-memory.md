# MemInStream: Memorizing or Merely Recognizing? Rethinking Streaming Video Memory Evaluation

[Paper](https://arxiv.org/abs/2611.15640) · First posted 2026-11-11 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A streaming assistant that helps unprompted needs to remember what it saw, but existing accuracy scores cannot tell forgetting from never seeing.

## Proactivity Signal

No user-facing decision. Each question is tied to annotated evidence intervals and kept only if models can answer from the evidence yet fail from text alone or from recent frames, so the score isolates memory.

## Evaluation Setup

3,799 multiple-choice questions with 8,217 evidence intervals across 17 tasks, filtered by two proprietary models and then human-reviewed. Five offline models and nine online streaming methods were evaluated. The best online method scores 37.06% on state tracking and 37.34% on multi-evidence integration; Gemini-3.8-Flash drops from 90.6% when the evidence is in its window to 21.8% when it is not.

## Key Limitations

Questions and some evidence are model-generated, and filtering depends on two specific proprietary models. It measures memory, not whether or when to help. The authors note it does not capture very long streams.

## Use For

Checking whether a streaming assistant's memory, rather than recent frames or language priors, supports its answers.
