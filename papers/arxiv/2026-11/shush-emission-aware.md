# SHUSH: Emission-Aware Reward Design for Proactive Video Assistants

[Paper](https://arxiv.org/abs/2611.26478) · First posted 2026-11-19 · Checked 2026-11-21. Paper and accessible artifact listings reviewed; no rerun.

## Why It Matters

An interval-matching reward counts extra replies and missed opportunities rather than scoring only the first timely hit.

## Proactivity Signal

Counts unnecessary replies as errors, so a video assistant cannot improve its timing score merely by speaking more often.

## Evaluation Setup

Existing visual OmniPro and ProactiveVideoQA tests show different changes in response volume; on visual OmniPro, the reported timing F1 rises from 0.259 to 0.396 under the matched recipe.

## Key Limitations

Uses existing annotations and backbones. It is a reward and evaluation study, not an unprompted task-discovery system. ICASSP under review is not acceptance.

## Use For

Design and evaluate the component or controls needed for calibrated initiative.
