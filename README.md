# Policy-Superposition

Policy Superposition for ARC-AGI 3

[PDF](https://iamjasonfeng.github.io/Policy-Superposition/policy_superposition_preliminary_report.pdf)

Abstract

This paper presents a preliminary evaluation of Policy Superposition, a lightweight test-time control
method I co-developed with OpenAI Codex for interactive language-model agents. Instead of committing
early to one interpretation of an unfamiliar environment, the agent maintains multiple candidate policies in
persistent memory, revises them using real action outcomes, and decides when the evidence justifies
selecting one. All candidates share one real trajectory and are updated inside ordinary action calls; the
method adds no auxiliary model calls, search tree, environment fork, rollback, voting procedure, or
external hypothesis manager. I evaluated the method on all 25 public ARC-AGI-3 games using DeepSeek
V4 Flash and the Tufa Labs Duck harness. A matched baseline scored 6.01%, while Policy Superposition
scored 11.02%, an increase of 83.4%. The treatment completed 52 levels across 24 games, compared with
42 levels across 21 games for the baseline, while using slightly fewer actions. Because this result comes
from one stochastic paired evaluation with important confounds, I present it as promising preliminary
evidence rather than a settled performance estimate.
