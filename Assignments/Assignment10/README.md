# Assignment 10 — Reinforcement Learning in Healthcare: Personalized Insulin Dosing

**Course:** ITAI 4375 — AI in Healthcare  
**Date:** March 30, 2026  

---

## Problem

Managing blood glucose in hospitalized diabetic patients is a high-stakes, continuous decision problem. Conventional sliding scale insulin protocols are static and fail to adapt to individual patient physiology. This paper investigated how reinforcement learning (RL) — an AI paradigm built around sequential decision-making — can be applied to personalize insulin dosing in intensive care unit patients.

## Approach

I developed a detailed system design for an RL-based insulin dosing agent, covering:

- **State space:** Patient observations including continuous glucose monitor readings, prior dosing history, and dietary intake
- **Action space:** Selection of insulin dose to maintain glucose between 70–180 mg/dL (the target "Time in Range")
- **Reward function:** Positive reinforcement for readings within the target zone; heavy penalties for hypoglycemic episodes below 70 mg/dL, which carry the highest clinical risk
- **Safety constraints:** Offline training on retrospective datasets and mandatory clinician oversight before any live deployment

I also reviewed published findings showing that one RL-driven model achieved a 73% Time in Range score, outperforming conventional sliding scale protocols, and examined the central challenge of keeping patients safe while the algorithm is still learning.

## Results & Key Findings

RL is well-suited to insulin dosing because the problem has the core structure RL is designed for: repeated decisions whose effects accumulate over time, clear feedback (glucose readings), and a well-defined goal (maximize time in safe range while minimizing dangerous lows). The published evidence supports feasibility, but clinical deployment at scale remains challenging due to the patient safety risks inherent in any trial-and-error learning process in a medical setting.

## What I Learned

This was the most technically advanced assignment of the course, and it pushed me to deeply understand how RL differs from other ML approaches. The key insight I took away: RL is not just about making one good prediction — it's about making a sequence of decisions that remain safe and effective over time, even as the environment (the patient's physiology) changes. That temporal dimension makes RL uniquely suited to — and uniquely dangerous in — clinical applications.
