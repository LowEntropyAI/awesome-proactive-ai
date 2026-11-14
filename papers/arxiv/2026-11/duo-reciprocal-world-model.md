# Duo: A Reciprocal World Model for Full-Duplex Interaction

[Paper](https://arxiv.org/abs/2611.15131) · First posted 2026-11-11 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A real-time audiovisual partner has to decide when to speak while it keeps watching and listening, not only what to say.

## Proactivity Signal

Every 0.71-second chunk, an intent module chooses to speak with text or wait, and a realization model renders matching audio and video. Training rebalances the two actions so the model does not collapse into waiting forever.

## Evaluation Setup

Human evaluation of 30 real-time duplex cases against six binary criteria: 168 of 180 checks passed (93.3%), with content responsiveness weakest at 22 of 30. There are no baselines, and the timing of speak-or-wait decisions is not measured.

## Key Limitations

The authors call it preliminary; response timing and longer sessions still need evaluation. Rater identity and number are not reported. Speak-or-wait happens inside a conversation the user drives, and "proactive inquiry" appears only as a data-generation setting. Inference code and weights are public; training code and data are not.

## Use For

An open full-duplex audiovisual backbone with an explicit speak-or-wait token.
