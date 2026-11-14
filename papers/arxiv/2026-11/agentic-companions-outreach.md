# A Life of Its Own: How Agentic AI Companions Are Configured, Experienced as Autonomous Others, and Held Accountable

[Paper](https://arxiv.org/abs/2611.12076) · First posted 2026-11-09 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

When a companion messages someone unprompted, the rule that allowed it is buried in code, prompts and defaults the user rarely sees.

## Proactivity Signal

The paper does not build a system. It traces how open-source companions and assistants decide to reach out: heartbeats and wake-ups create an occasion to act, the model decides whether to send, and whether a user's refusal binds later outreach depends on whether it is enforced in code or only in the prompt.

## Evaluation Setup

Study 1 analyses 12 open-source repositories (four companion-oriented, four assistant-oriented, one boundary case, three components) at pinned commits, screened from 93 eligible projects. Study 2 interviews 10 people who built or modified their own companions. Findings are qualitative; there are no headline metrics.

## Key Limitations

The systems were not run, so claims concern configured mechanisms rather than observed behaviour. The interview sample is small and homogeneous (ten women, nearly all describing a romantic partner), and commercial products are excluded.

## Use For

Locating where outreach rules and refusals live in companion code before designing unprompted messaging.
