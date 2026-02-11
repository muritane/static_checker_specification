# Execution Primitives  
## Ontological Constraints for Bounded Systems Under Load

---

## Status

This document defines the **minimal execution ontology** required for reasoning about systems that:

- act,
- consume resources,
- propagate effects,
- and persist across time.

It contains **no typing rules**,  
no agency claims,  
no responsibility attribution,  
no optimization criteria,  
no moral commitments.

It specifies only what must be structurally true  
for execution to exist at all.

Everything in higher layers (agency, metrics, governance, redesign, typing)  
is derived from these primitives.

If any primitive here is invalidated,  
the entire stack above must be reconsidered.

---

## 0. Scope

This ontology applies **if and only if** all of the following hold:

- Action produces real state transitions.
- Resources are finite.
- Time is not freely reversible.
- Effects can propagate beyond the acting locus.
- Persistence across time matters.

Systems outside these conditions (purely symbolic, timeless, consequence-free) are out of scope.

---

# Core Execution Primitives

These constraints are **non-negotiable under current physical understanding**.

They are not normative.
They are not optional.
They are not preferences.

They are structural features of execution in bounded systems.

---

## E1 — Bounded Resources

All executors operate under finite limits in:

- time,
- energy,
- material capacity,
- computation,
- memory,
- attention,
- coordination bandwidth.

No system can:

- evaluate infinite alternatives,
- maintain infinite context,
- negotiate without bound,
- or delay decision indefinitely without cost.

> Infinite slack is incompatible with execution.

---

## E2 — Partial Observability

No executor has complete access to all state variables governing outcomes.

Observation is:

- filtered,
- delayed,
- lossy,
- and model-dependent.

Perfect state access is unattainable in bounded systems.

> Any representation of the world is necessarily incomplete.

---

## E3 — Irreversibility

Execution induces state transitions that cannot, in general, be undone.

Rollback, reversal, and repair:

- are themselves executions,
- consume additional resources,
- introduce new state transitions,
- and do not restore prior informational symmetry.

Time asymmetry is structural.

> Execution destroys alternative futures.

---

## E4 — Irreversible Abstraction

Execution requires lossy collapse of distinctions.

This occurs in two distinct but related forms:

### E4a — Representational Loss

Representations cannot preserve all distinctions present in the world.

Models are compressions.

They discard structure to become tractable.

---

### E4b — Actuation Loss

Action selection maps many possible world states to a single executed transition.

Alternative branches are collapsed.

Future options are eliminated.

---

These two losses may coincide or diverge depending on system design,  
but at least one must occur for execution to proceed under bounded resources.

> Lossless execution is impossible.

---

## E5 — Drift / Non-Stationarity

Causal structure changes over time.

- Environments shift.
- Dependencies reconfigure.
- Latencies vary.
- Couplings strengthen or weaken.
- Resource margins erode.

No invariant is globally permanent.

All invariants are regime- and horizon-bounded.

> Stability is always conditional.

---

## E6 — Horizon Boundedness

All execution unfolds over a temporal horizon.

Evaluation, viability, and stability are meaningful only relative to:

- a time window,
- or an operational lifespan.

Claims that do not specify a horizon are underspecified for execution.

Horizons may be implicit,  
but they must be recoverable for coherence.

> Horizon-free validity does not exist in bounded systems.

---

## E7 — Topological Distinction

Execution implies at least one distinguishable locus where:

- state transitions occur,
- disturbance can accumulate,
- resource depletion can manifest,
- and constraints can bind.

Even if representation, executor, and affected state are colocated,  
they must be distinguishable in principle for execution to be meaningful.

Without topology:

- load has nowhere to land,
- cost has nowhere to accumulate,
- disturbance has no path.

> Execution implies structure.

---

## E8 — Consequence Propagation

Disturbance introduced by execution propagates through structure.

Propagation may involve:

- latency,
- buffering,
- amplification,
- attenuation,
- fan-out,
- or masking.

Propagation is governed by topology, not intent.

Effects may be:

- delayed,
- displaced,
- accumulated,
- or redistributed.

But they do not vanish.

> No disturbance is annihilated; it is transformed or relocated.

---

## E9 — Viability as Structural Condition

A system is viable if and only if it preserves:

- the capacity to continue executing,
- the capacity to sense sufficiently for adaptation,
- and the capacity to act meaningfully within its horizon.

Viability does not imply:

- success,
- growth,
- optimality,
- moral goodness.

It implies non-collapse.

> Optimization presupposes viability.

---

# What This Layer Does Not Contain

This ontology does not include:

- agency
- responsibility
- metrics
- evaluation
- legitimacy
- governance
- meaning
- narrative
- optimization
- fairness
- authority
- redesign policies
- value judgments

Those belong to higher layers.

This layer only specifies what must be true for execution to exist.

---

# Minimality Claim

This set is minimal in the following sense:

- Removing any primitive makes bounded execution unintelligible.
- Adding domain-specific constraints here prematurely over-specifies the ontology.
- All higher-order reasoning must reduce to these primitives without contradiction.

If future physical knowledge invalidates any primitive,
the entire architecture above must be revised.

---

# Summary

Execution in bounded systems requires:

- finite resources,
- partial observability,
- irreversible time,
- lossy abstraction,
- non-stationary causality,
- horizon-bounded validity,
- structured topology,
- consequence propagation,
- and structural viability.

Everything else is layered on top.

This document defines the ground layer.

Nothing below this.
