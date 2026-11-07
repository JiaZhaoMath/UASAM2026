---
speaker: Md Obaidul Haque
role: student
campus: The University of Alabama
campus_short: UA
title: LLM-Driven Behavioral Heterogeneity in Networked SEIR(S) Models with GAM Distillation
slot: 2:10–2:30 p.m.
source: ../../abstracts/ua_haque_student.md
---

Human behavior has a large impact on epidemic dynamics, yet classical compartmental models usually treat individuals as homogeneous and their protective behavior as absent or fixed. We develop a hybrid networked SEIR framework in which a large language model (LLM) provides each agent’s behavioral decisions. Agent profiles, epidemic conditions, social influence, and policy signals are encoded as natural-language prompts, and the LLM returns a willingness-to-comply score that sets the agent’s self-protection level. Single-factor experiments show distinct, demographically structured infection burdens across age, occupation, and income groups, which no-protection, heuristic, and fixed-mean baselines fail to reproduce. We then reformulate the model as an SEIRS continuous-time Markov chain driven by independent Poisson clocks with waning immunity. Because querying the LLM for every decision is slow and costly, we replace it with a distilled, interpretable generalized additive model (GAM) trained on current-state inputs. In preliminary validation, the GAM surrogate reproduces the LLM-driven epidemic trajectories. It enables faster simulations at no API cost, opening a path to large-population studies of LLM-driven behavior.
