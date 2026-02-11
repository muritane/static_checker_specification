# Cognitive Layer  
## Representation, Traversal, and Decision Under Effective Infinity

---

## Status

This document defines the **Cognitive Layer** of the stack.

It assumes:

- `0_core/execution_primitives.md`
- `1_structural/typing_discipline.md`
- `2_control/control_layer.md`

It does not introduce new physics.
It does not introduce normative claims.

It specifies how bounded agents:

- represent possibility spaces,
- traverse effectively infinite domains,
- allocate attention,
- compress state,
- decide under partial observability,
- and cope with irreversible abstraction.

If the Execution Layer defines what must be true for systems to run,  
and the Control Layer defines how systems stabilize under disturbance,

the Cognitive Layer defines:

> How bounded agents choose what to see, explore, ignore, and commit to.

---

# 1. Scope

This layer applies when:

- the state space is too large to enumerate,
- evaluation is costly,
- attention is scarce,
- representation is compressed,
- and traversal is path-dependent.

It applies to:

- biological cognition,
- artificial agents,
- planning systems,
- research programs,
- cultural evolution,
- career trajectories,
- exploration under uncertainty.

It does not assume intelligence in the human sense.
It assumes bounded traversal under constraint.

---

# 2. Effective Infinity

A space is **effectively infinite** when:

- full enumeration exceeds resource bounds (E1),
- evaluation cost dominates search,
- drift invalidates static maps (E5),
- or halting occurs before global coverage.

Effective infinity is an executional property, not a set-theoretic one.

Under effective infinity:

- global optimization is ill-typed,
- exhaustive comparison is impossible,
- reachability replaces existence as the operative category.

---

# 3. Representation as Compression

All cognition relies on representational compression (E4a).

Representation:

- discards distinctions,
- defines equivalence classes,
- shapes what is perceptible,
- constrains what can be imagined,
- limits what can be evaluated.

Representation is:

- horizon-bound (E6),
- topology-sensitive (E7),
- drift-exposed (E5).

Representation is not neutral.
It determines reachable futures.

---

# 4. Traversal and Path Dependence

Traversal is movement through possibility space under resource bounds.

Traversal is:

- sequential,
- lossy,
- irreversible (E3),
- attention-limited (E1).

Path dependence means:

> Future discoverability depends on prior traversal.

Once a path is taken:

- alternative branches become costly,
- representation updates bias future selection,
- missed structures compound into exclusion.

Traversal commits blindness.

---

# 5. Exploration vs Exploitation

Cognitive systems alternate between:

## Exploration
- Preserve degrees of freedom.
- Expand representation.
- Probe unknown regions.
- Accept inefficiency.
- Increase model uncertainty.

## Exploitation
- Collapse degrees of freedom.
- Commit to known policies.
- Extract returns.
- Reduce variance.
- Increase specialization.

The transition is irreversible at fine granularity.

Exploration consumes viability margin.
Exploitation risks drift-induced brittleness.

Balancing them is structural, not moral.

---

# 6. Attention as Scarce Allocation

Attention is a finite resource (E1).

Attention determines:

- which signals enter representation,
- which distinctions are preserved,
- which alternatives are evaluated,
- which failures are detected.

Unattended signals are structurally invisible.

Attention allocation is itself a policy under constraint.

---

# 7. Heuristics and Bias

Heuristics are compressed policies for traversal.

They:

- reduce search cost,
- collapse distinctions,
- trade optimality for tractability.

Bias is unavoidable because:

- compression is unavoidable (E4),
- evaluation is expensive (E1),
- horizons are bounded (E6).

Bias becomes failure only when:

- drift invalidates assumptions,
- heuristics suppress redesign signals,
- representation cannot represent its own invalidation.

---

# 8. Model Uncertainty and Drift

Cognitive systems operate with provisional models.

Drift (E5) implies:

- models degrade,
- prior probabilities misalign,
- feedback shifts.

Adaptive cognition requires:

- preserved redesign pathways (Typing §10),
- ability to detect model mismatch,
- tolerance for ambiguity.

Overconfidence is often compressed uncertainty, not certainty.

---

# 9. Halting Conditions

Traversal halts due to:

- resource exhaustion (E1),
- opportunity cost,
- external interruption,
- viability constraints (E9).

Non-discovery does not imply non-existence.

It implies non-reachability within horizon.

This invalidates:

- merit narratives based purely on visibility,
- optimization claims assuming exhaustive search,
- blame attribution based on outcome absence.

---

# 10. Cognitive Load and Control Interaction

Cognition interacts with control:

- Model quality affects control stability.
- Control policies constrain exploration.
- Buffer margins affect risk tolerance.
- Over-control can suppress exploration.
- Under-control amplifies noise.

Cognition and control co-evolve.

---

# 11. Cognitive Failure Modes

## 11.1 Premature Closure

Fixing representation too early.
Collapsing latent degrees of freedom.

Result: brittleness under drift.

---

## 11.2 Endless Exploration

Never committing to closure.
Preserving too many distinctions.

Result: resource exhaustion.

---

## 11.3 Model Entrenchment

Suppressing redesign signals.
Ignoring topology changes.

Result: catastrophic misalignment.

---

## 11.4 Attention Capture

External signals hijack limited attention.
Distortion of traversal priorities.

Result: skewed reachability.

---

# 12. Agency Within Cognitive Limits

Agency remains bounded by:

- representational limits,
- attention scarcity,
- path dependence,
- topology awareness,
- horizon awareness.

Cognitive systems cannot:

- consider all alternatives,
- foresee all consequences,
- maintain infinite optionality.

Agency is always partial.

---

# 13. Cognitive Layer Boundaries

This layer does not:

- declare goals,
- enforce metrics,
- assign responsibility,
- define legitimacy.

It defines how bounded agents:

- construct world models,
- traverse possibility space,
- and commit under irreversibility.

Goal selection belongs above.
Execution physics belongs below.
Control stabilizes between them.

---

# 14. Robotics Mapping (Example)

In robotics:

- Representation → world model, SLAM map, learned policy
- Traversal → planning tree expansion
- Exploration → randomization, frontier search
- Exploitation → fixed policy execution
- Attention → sensor prioritization
- Drift → sensor degradation, terrain change
- Halting → battery depletion, task timeout

The same structural constraints apply to research programs and personal development.

---

# Summary

Cognition in bounded systems is:

- compressed representation under irreversibility,
- prioritized traversal under effective infinity,
- path-dependent commitment under drift,
- attention allocation under scarcity.

Global optimality is rarely well-typed.
Reachability dominates existence.
Traversal shapes the future more than intention.

This layer explains why.

Execution remains below.
Control regulates.
Governance redesigns.
Goals constrain from above.
