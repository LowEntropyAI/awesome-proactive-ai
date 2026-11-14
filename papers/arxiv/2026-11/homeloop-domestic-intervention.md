# HomeLoop: A Simulation Framework and Benchmark for Robot-IoT Coordination in Everyday Domestic Assistance and Safety

[Paper](https://arxiv.org/abs/2611.08914) · First posted 2026-11-06 · Checked 2026-11-15. Primary paper and available artifact listings reviewed; no rerun.

## Why It Matters

A home robot woken by a smoke alarm has to tell a resident cooking from a pan on fire, and over-reacting can be as wrong as doing nothing.

## Proactivity Signal

A VLM agent controlling a robot and smart-home devices is woken by sensor, wearable or routine events and must decide whether and how to intervene. In 14 of 20 tasks no resident has asked; an unnecessary intervention fails the episode just as a missed one does.

## Evaluation Setup

Twenty tasks in five families (hazards, entry, wellbeing, chores, requests) in Isaac Sim with simulated residents, faulty sensors and evolving hazards, scored by a temporal-logic runtime monitor rather than an LLM judge. Six VLMs, two seeds each, mainly in one house. The best family-balanced score is 61.9%; across failed episodes, forbidden interventions outnumber missed required ones 42 to 16, and one model placed 1 of 20 required emergency calls.

## Key Limitations

Mostly one house, one robot body and two seeds; motion is kinematic, detections come from filtered ground truth, and the world pauses during inference. Residents are simulated and the checks encode prescribed policies. The framework is announced for release, with no link yet.

## Use For

Scoring both missed and unwanted interventions for a home agent responding to ambiguous alarms.
