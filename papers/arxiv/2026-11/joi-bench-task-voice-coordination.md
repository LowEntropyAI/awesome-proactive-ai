# Joi-Bench-Task: Benchmarking Task Coordination in Full-duplex Voice Agents through Interactive Simulation

[Paper](https://arxiv.org/abs/2611.12118) · First posted 2026-11-09 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A voice agent running tools in the background still has to decide when to report results while the user keeps talking, changes plans or interrupts.

## Proactivity Signal

Every task is requested by the user. The agent must decide when to announce results from asynchronous tools, absorb mid-task changes and status questions, pause on interruptions and resume reporting without dropping anything.

## Evaluation Setup

Sixty scenarios across six domains give 140 cases; five commercial voice agents produce 700 conversations of up to 480 seconds. An LLM-and-TTS user simulator injects interventions at controlled moments (699 of 700 delivered in the intended window). Scoring passes ASR transcripts to an LLM evaluator and a second LLM reviewer. Under request changes the best result completion is 55%; after interruptions four of five agents omit at least 23% of information on average.

## Key Limitations

English only, clean audio, mock tools with fixed run times, simulated users and LLM scoring. It times reports for requests already made rather than unprompted help. No code or data link was found.

## Use For

Testing whether full-duplex voice agents keep track of what they have done, said and still owe while the user talks over them.
