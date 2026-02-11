# Constraint Architecture for Bounded Execution

A layered constraint framework for modeling systems that:

* Execute physical state transitions,
* Operate under finite resources,
* Experience irreversible change,
* Evolve under drift,
* Interact across structured topology,
* And adapt under governance.

This repository defines a structured stack for analyzing:

* What must be physically true for execution,
* When claims about execution are structurally coherent,
* How systems regulate trajectories under disturbance,
* How bounded agents search and commit,
* How norms restrict admissible trajectories,
* How authority modifies constraints,
* How strategic interaction unfolds under resource limits.

This is not a moral doctrine.

It is a constraint-theoretic execution framework.

---

# Core Principle

All reasoning about action must respect:

1. Finite measurable resource vectors.
2. Information capacity limits.
3. Physical irreversibility.
4. Lossy representation and actuation.
5. Parameter drift.
6. Finite evaluation horizon.
7. Structured topology.
8. Conservation-governed consequence propagation.

Everything above the Core must reduce to these measurable constraints.

---

# Architecture Overview

The system is layered.

Lower layers constrain higher ones.

```
docs/
  0_core/
    execution_primitives.md
  1_structural/
    typing_discipline.md
  2_control/
    control_layer.md
  3_cognitive/
    cognitive_layer.md
    exploration_vs_execution.md
  4_domain/
    robotics.md
    personal_domain.md
  5_normative/
    normative_layer.md
  6_governance/
    governance_layer.md
  7_strategic/
    viability_constrained_game_theory.md
```

Each layer:

* Declares its assumptions,
* Defines measurable objects,
* Specifies typing conditions,
* Preserves lower-layer invariants,
* Remains horizon-bound.

---

# Layer Summary

## 0 — Core (Execution Primitives)

Defines measurable physical and informational constraints:

* Finite resource vectors (time, energy, bandwidth, etc.)
* Information channel limits
* Thermodynamic irreversibility
* Representational compression
* Parameter drift
* Finite horizon
* Structured topology
* Conservation and consequence propagation

No goals.
No norms.
No viability axiom.

Only measurable constraints.

---

## 1 — Structural Typing Discipline

Defines when execution claims are coherent.

All claims must declare:

* Topology
* Horizon
* Resource bounds
* Disturbance bounds
* Drift assumptions

Introduces:

* Trajectory safety predicate (formerly viability)
* Executability boundary
* Degree-of-freedom partition
* Agency typing rule
* Responsibility typing rule
* Metric validity constraints

Typing determines structural admissibility.

It does not determine truth or morality.

---

## 2 — Control

Defines closed-loop regulation under:

* Bounded disturbance,
* Finite resources,
* Drift exposure,
* Explicit state and resource constraints.

Stability means:

* State and resource thresholds remain satisfied over horizon H.

Control preserves constraint satisfaction.
It does not select goals.

---

## 3 — Cognitive

Defines bounded search and representation under:

* Finite compute,
* Limited information,
* Irreversibility,
* Effective infinity (computational infeasibility of exhaustive search).

Exploration and execution are formally separated.

Cognition shapes trajectory selection but cannot escape physical limits.

---

## 4 — Domain Instantiations

Applies the stack to concrete domains.

### Robotics

* Energy measured in joules.
* Latency measured in seconds.
* Topology explicit (ROS graphs, power networks).
* Drift observable (sensor degradation, wear).
* Failure physically measurable.

### Personal Domain

* Finite lifespan.
* Finite energy and cognitive bandwidth.
* Embedded social topology.
* Irreversible commitments.
* Drift through aging and environmental change.

The stack becomes embodied and measurable.

---

## 5 — Normative Layer

Defines additional admissibility constraints over trajectories.

Norms are constraint functions:

$$
\Omega_H \rightarrow \Omega_H^N
$$

They restrict what is permitted among physically possible trajectories.

Norms:

* Are horizon-bound,
* Require enforcement topology,
* Do not override physics.

Optimization occurs only within normative constraints.

---

## 6 — Governance Layer

Defines authority over constraint modification.

Governance specifies:

* Who may change constraints,
* How changes propagate,
* How enforcement operates,
* How versioning and redesign occur.

Governance cannot suspend physical laws.

It manages meta-constraints.

---

## 7 — Strategic Layer

Embeds game-theoretic reasoning within bounded execution.

Strategic analysis must:

* Declare horizon,
* Respect resource floors,
* Model drift,
* Restrict to safety-preserving strategies,
* Account for irreversibility and topology.

Equilibria are classified as:

* Safety-preserving,
* Drift-fragile,
* Buffer-consuming,
* Ill-typed.

Game theory remains intact but typed against physical constraint.

---

# Design Invariants

Across all layers:

1. Physics is non-negotiable.
2. All evaluation is horizon-bound.
3. Resource vectors are finite and measurable.
4. Irreversibility reduces reachable state space.
5. Drift invalidates stationary assumptions.
6. Disturbance propagates through topology.
7. Optimization does not precede safety.
8. Constraint changes must be versioned.
9. Load redistribution must be traceable.

---

# What This Repository Is Not

It is not:

* A moral doctrine,
* A political manifesto,
* A productivity system,
* A universal metaphysics,
* A replacement for formal control theory,
* A replacement for formal game theory.

It is a structural constraint framework for systems that execute under load.

---

# How to Use

When analyzing any system:

1. Declare topology $G$.
2. Declare finite horizon $H$.
3. Specify resource vectors $R$.
4. Declare disturbance bound $D$.
5. Specify drift model $\Theta$.
6. Define state and resource thresholds.
7. Apply typing discipline.
8. Only then evaluate optimization or strategy.

If a layer is skipped, claims may be under-typed.

---

# Extension Policy

* New physical primitives require revision of Core.
* New typing rules require Structural update.
* New domains belong in `4_domain/`.
* New strategic models belong in `7_strategic/`.
* Norm updates require governance revision.
* All constraint changes must declare horizon and resource impact.

Core primitives change only if physical law changes.

---

# Summary

This architecture separates:

* Physical constraint,
* Structural coherence,
* Trajectory regulation,
* Bounded search,
* Normative admissibility,
* Constraint authority,
* Strategic interaction.

Each layer is explicit.

Each layer is horizon-bound.

Each layer is resource-aware.

Execution is physical.

Constraint discipline ensures reasoning remains coherent within that fact.
