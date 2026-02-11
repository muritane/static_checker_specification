# Exploration vs Execution

## Regime Separation Under Finite Resources and Irreversible Commitment

---

## Status

This document belongs to the **Cognitive Layer**.

It assumes:

* Measurable execution primitives (E1–E8)
* Structural Typing Discipline
* Control Layer
* Cognitive Layer

It introduces no new primitives.

It formalizes the structural distinction between:

* **Exploratory regimes** (non-binding computation)
* **Execution regimes** (resource-committing state transition)

The purpose is to prevent type confusion between:

* Representational search
* Load-bearing physical execution

Constraint discipline activates only when execution begins.

---

# 1. Definitions

## 1.1 Exploration

Exploration is computation that:

* Does not modify external topology,
* Does not commit irreversible state transitions outside the computing locus,
* Does not reassign load across shared nodes,
* Consumes only local resource vector components.

Formally:

Let exploration state be:

$$
\hat{x}(t)
$$

Exploration is confined to internal state transitions:

$$
\hat{x}(t+1) = F(\hat{x}(t))
$$

Without modifying:

$$
x_{external}(t)
$$

Exploration consumes:

* Local computation
* Local memory
* Local time
* Local energy

But does not alter global resource distribution or topology.

---

## 1.2 Execution

Execution is a state transition that:

1. Alters physical or shared topology,
2. Consumes shared resource components,
3. Produces externally observable load redistribution,
4. Is subject to irreversibility (E3).

Formally, execution occurs when:

$$
x(t+1) = f(x(t), u(t))
$$

Where:

* $x(t$ includes shared system state,
* $u(t)$ commits actuation.

Execution activates:

* Conservation (E8),
* Drift exposure (E5),
* Resource constraints (E1),
* Typing safety predicates.

---

# 2. Executability Boundary

The executability boundary is crossed when:

At least one of the following holds:

1. Resource vector $R$ outside local sandbox is modified.
2. Shared topology $G$ is altered.
3. External state $x_{external}$ changes.
4. Irreversible actuation is committed.
5. Contractual or interface invocation occurs.

Before crossing boundary:

* Typing discipline applies loosely.
* Safety predicates are inactive.
* Load routing is unchanged.

After crossing boundary:

* Typing discipline is mandatory.
* Control constraints apply.
* Resource and state thresholds must be respected.

---

# 3. Effective Infinity

Let decision space:

$$
A = {a_1, ..., a_N}
$$

Where:

$$
N \gg \frac{C_{total}}{C_{eval}}
$$

i.e., number of possible configurations far exceeds feasible evaluation capacity over $H$.

A space is effectively infinite if:

$$
\text{Exhaustive evaluation infeasible within } (R, H)
$$

Effective infinity is computational, not set-theoretic.

Exploration samples subset:

$$
A_{sampled} \subset A
$$

With:

$$
|A_{sampled}| \ll |A|
$$

Non-discovery does not imply non-existence.

It implies infeasibility under resource constraint.

---

# 4. Regime Properties

## 4.1 Exploration Regime

Properties:

* No shared resource modification.
* No topology alteration.
* Reversible within sandbox (subject to local E3).
* No external safety predicate activation.
* No governance enforcement required.

Exploration may:

* Evaluate inconsistent models.
* Simulate unstable trajectories.
* Consider norm violations.
* Traverse infeasible regions.

Exploration is computational search under local resource constraints.

---

## 4.2 Execution Regime

Properties:

* Shared resource consumption.
* State constraints active.
* Drift exposure begins.
* Irreversibility applies.
* Disturbance propagates.
* Responsibility becomes typeable.

Execution is load-bearing.

Execution is structurally constrained.

---

# 5. Sandbox Condition

Exploration remains non-binding only if sandbox condition holds:

1. Resource use is isolated.
2. State modifications are internal.
3. No irreversible external actuation.
4. No shared topology update.
5. No contract enforcement triggered.

If sandbox condition fails, exploration transitions to execution.

---

# 6. Transition Rule

Transition occurs when proposal becomes actuation.

Formally:

Exploration variable $a$ becomes execution input $u(t)$.

$$
a \rightarrow u(t)
$$

At that moment:

* Constraint functions $g_i(x)$ become active.
* Resource thresholds $r_j(t) \ge \tau_j$ apply.
* Drift exposure accumulates.
* Disturbance propagation begins.

Transition is irreversible in general.

---

# 7. Multi-Agent Implications

In shared topology:

Exploration is typically local to a node.

Execution modifies global graph:

$$
G_{t+1} \neq G_t
$$

A single actuation may:

* Redistribute load.
* Trigger cascading failures.
* Alter buffer ownership.
* Modify authority structure.

Therefore:

Exploration may be plural.
Execution must respect shared constraints.

---

# 8. Error Modes

Failure to separate regimes produces two classes of error:

---

## 8.1 Over-Constraining Exploration

Applying execution-level constraints to sandbox search.

Effects:

* Reduced innovation.
* Premature closure.
* Suppressed model updating.

---

## 8.2 Under-Constraining Execution

Treating execution as symbolic exploration.

Effects:

* Hidden load accumulation.
* Untracked resource depletion.
* Metric drift.
* Governance failure.

---

# 9. Redesign and Safe Deployment

Exploratory models may:

* Simulate,
* Emulate,
* Prototype.

Deployment occurs when:

$$
\hat{x}(t) \rightarrow x(t)
$$

Governance must:

* Declare transition explicitly.
* Specify horizon $H$.
* Declare safety predicates.
* Assign responsibility.

Implicit deployment is ill-typed.

---

# 10. Interaction with Typing Layer

Typing discipline activates fully only in execution regime.

Exploration claims may be:

* Under-typed
* Internally inconsistent
* Speculative

Execution claims must be:

* Well-typed under declared environment
* Safety-bounded
* Horizon-explicit

Optimization claims apply only in execution regime.

---

# 11. Summary

Under finite resources and irreversibility:

Two structurally distinct regimes exist:

Exploration:

* Internal computation
* No shared load
* No topology modification
* Reversible within sandbox
* Search under effective infinity

Execution:

* Shared resource consumption
* Irreversible state transition
* Disturbance propagation
* Constraint activation
* Responsibility attribution

Constraint discipline applies at the executability boundary.

Regime separation preserves:

* Computational freedom upstream
* Structural coherence downstream

Both regimes are necessary.
They are not interchangeable.
