# Structural Typing Discipline

## A Static Coherence System for Execution Claims Under Physical Constraint

---

## Status

This document defines the **Typing Layer** built on top of the measurable execution primitives (E1–E8).

It does not introduce new physics.
It does not introduce norms.
It does not select goals.

It specifies when claims about execution are:

* Well-typed
* Under-typed
* Ill-typed

with respect to bounded physical systems.

If the Core defines what must be physically true for execution to exist,
this document defines what must be structurally true for statements about such systems to be coherent.

---

# 0. Dependency

This layer assumes the measurable primitives:

* E1 — Finite Resource Vectors
* E2 — Information Capacity Limits
* E3 — Irreversibility
* E4 — Lossy Representation and Actuation
* E5 — Drift
* E6 — Horizon Boundedness
* E7 — Structured Topology
* E8 — Conservation and Consequence Propagation

If any primitive changes, typing guarantees must be re-evaluated.

---

# 1. Typing Environment

All execution-relevant claims must be typed relative to an explicit or inferable environment:

$$
\mathcal{T} = (E, G, H, R, \Theta)
$$

Where:

* **$E$** — Information structure

  * Channel capacities (bits/s)
  * Latency (s)
  * Noise model

* **$G$** — Topology graph

  * Nodes $V$
  * Edges $E$
  * Load routing structure

* **$H$** — Finite evaluation horizon (seconds, cycles, episodes)

* **$R$** — Resource vectors for relevant loci

  * Energy (J)
  * Time (s)
  * Memory (bytes)
  * Compute (FLOPs/s)
  * Financial or domain-specific resources

* **$\Theta$** — Drift model

  * Parameter evolution $\theta(t)$
  * Drift bounds over $H$

Claims that omit necessary components of $\mathcal{T}$ are **Under-Typed**.

---

# 2. Claim Categories

Every execution-relevant claim must belong to one of the following types:

1. **Execution Claim**

   * Asserts that a state transition occurs.
   * Must specify affected loci in topology.

2. **Trajectory Claim**

   * Asserts behavior over time interval $[0, H]$.

3. **Optimization Claim**

   * Asserts improvement relative to metric.

4. **Safety / Viability Claim**

   * Asserts preservation of execution capacity over $H$.

5. **Agency Claim**

   * Asserts decision boundary prior to execution.

6. **Responsibility Claim**

   * Attributes load or outcome to locus in topology.

7. **Metric Claim**

   * Defines evaluative function over trajectories.

8. **Governance Claim**

   * Modifies constraints or typing environment.

Type confusion results in ill-typed discourse.

---

# 3. Interpretation vs Execution Boundary

There exists a strict boundary between:

## Interpretation (Non-Binding)

* Narrative
* Meaning
* Hypothesis
* Preference
* Intention
* Value declaration

These do not modify topology or resource vectors.

## Execution (Binding)

Execution occurs when:

* Resource vector R changes,
* State transition occurs,
* Load propagates through G,
* Contract or interface is invoked,
* Irreversible action is taken.

Crossing the boundary activates physical constraints (E1–E8).

A claim that moves from interpretation to execution without specifying:

* Affected nodes,
* Resource consumption,
* Horizon,

is ill-typed.

---

# 4. Trajectory Safety Predicate (Derived Viability)

Viability is not primitive.

It is a trajectory predicate:

$$
V(H) := \forall t \in [0,H], r_i(t) \ge \tau_i
$$

Where:

* $r_i(t)$ are resource components,
* $\tau_i$ are declared collapse thresholds.

A system is trajectory-safe over $H$ if:

* Resource floors are not breached,
* Irreversible collapse states are not entered,
* Information channels remain functional.

All optimization claims must declare a trajectory safety predicate.

Optimization without declared safety thresholds is ill-typed.

---

# 5. Optimization Typing Rule

An optimization claim:

$$
\Delta M > 0
$$

is well-typed only if:

1. Metric $M$ is defined and computable under $R$.
2. Horizon $H$ is declared.
3. Drift model $\Theta$ is specified or bounded.
4. Safety predicate $V(H)$ is declared.

Otherwise the claim is Under-Typed.

If optimization violates declared safety predicate, it is Ill-Typed.

---

# 6. Degree-of-Freedom (DOF) Partition

Executable participation requires explicit DOF partitioning:

For a given decision boundary:

* **Essential DOFs** — Fixed prior to execution.
* **Delegated DOFs** — Adjustable within bounds.
* **Latent DOFs** — Reserved for redesign.
* **Collapsed DOFs** — Intentionally eliminated.
* **Unknown DOFs** — Not modeled.

Failure to partition DOFs results in invisible constraint surfaces.

Invisible constraints cause misattributed responsibility.

---

# 7. Agency Typing

Agency exists only at pre-execution decision boundaries.

A boundary is agency-typed if:

1. Acceptance and refusal are executable.
2. Consequences of refusal are bounded.
3. DOFs are declared.
4. Horizon scope is explicit.

If refusal leads to unbounded collapse, agency claim is ill-typed.

Inside execution, only discretion exists — not agency.

---

# 8. Responsibility Typing

Responsibility attribution must follow topology.

A responsibility claim is well-typed only if:

1. The locus controls relevant DOFs.
2. Load routing through $G$ is traceable.
3. Outcome depends causally on locus-controlled variables.
4. Horizon is aligned.

Intent, status, proximity, or narrative involvement are insufficient.

Responsibility follows load accumulation under E7 and E8.

---

# 9. Metric Validity

A metric $M$ is valid only if:

1. It is computable under $R$.
2. It is horizon-bound.
3. It is reproducible under declared $E$.
4. It fails explicitly outside its domain.

A metric that never fails accumulates unmodeled drift.

Implicit reinterpretation of metric failure is structural decay.

---

# 10. Drift Sensitivity Rule

All trajectory and optimization claims must specify one of:

* Drift bound over $H$,
* Stationarity assumption,
* Regime boundary.

Failure to declare drift exposure makes long-horizon claims under-typed.

---

# 11. Redesign Safety

A system remains redesign-safe only if:

* DOFs remain partially latent.
* Safety predicate is observable.
* Collapse thresholds are explicit.
* Horizon can be revised.
* Interface contracts are versioned.

A representation that cannot represent its own invalidation is ill-typed.

---

# 12. Power (Descriptive Typing)

Power is defined as:

> Capacity to modify $R$, $G$, $H$, or DOF partitions.

Power claims must specify:

* Which resource vectors are affected,
* Which nodes absorb load,
* Which horizon is altered.

Power does not eliminate cost.

It redistributes load.

---

# 13. Three-Valued Typing Outcome

Every claim is exactly one of:

## Well-Typed

Structurally coherent under declared $\mathcal{T}$.

## Under-Typed

Missing necessary declarations or witnesses.

## Ill-Typed

Violates execution primitives or internal consistency.

Truth is orthogonal to typing.

Typing concerns structural admissibility under physical constraint.

---

# 14. What This Layer Does Not Do

This discipline does not:

* Determine moral correctness.
* Guarantee success.
* Select goals.
* Eliminate conflict.
* Enforce norms.

It determines only:

Whether a claim about bounded execution is structurally coherent.

---

# 15. Summary

Given measurable physical primitives (E1–E8), this typing discipline:

* Forces explicit horizons,
* Requires topology declaration,
* Binds optimization to trajectory safety,
* Prevents false agency claims,
* Grounds responsibility in load routing,
* Requires metrics to fail explicitly,
* Makes drift visible.

It is a static coherence system for execution discourse.

All higher layers must type-check against it.
