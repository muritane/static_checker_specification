# The Minimal Constraint Core

## (Execution Typing for Bounded Systems)

This is a **closed set**.
Nothing here is optional.
Nothing here is value-laden.
Anything not listed here is *derived*, *domain-specific*, or *interpretive*.

---

## 0. Scope Declaration (Global)

This constraint core applies **if and only if** all of the following are true:

* Action occurs in the world (not pure interpretation)
* Resources are finite
* Time is irreversible
* Outcomes propagate beyond the actor
* Persistence across time matters

If any of these are false, the system is **out of scope**.

---

## 1. Foundational Constraints (Physics-Level)

These constraints are **non-negotiable**.
No goal, intelligence, coordination, or ethics can remove them.

### C1 — Bounded Resources

Time, energy, attention, compute, coordination bandwidth, and material capacity are finite.

> Any claim requiring infinite context, infinite patience, or infinite negotiation is ill-typed.

---

### C2 — Partial Observability

No executor has full access to the state variables governing outcomes.

> Claims assuming full information are ill-typed under execution.

---

### C3 — Irreversibility

Execution induces state transitions that cannot, in general, be undone.

> Rollback is itself costly execution, not a default property.

---

### C4 — Unavoidable Compression

Any pipeline from world → representation → action collapses distinctions irreversibly.

> Lossless abstraction is impossible under execution.

---

### C5 — Drift / Non-Stationarity

Causal structure changes over time.

> All invariants are horizon-bounded.

---

## 2. Executability Boundary

A strict boundary exists between **interpretation** and **execution**.

* Above the boundary: meaning, intent, narrative, justification
* At the boundary: invocation, defaults, omission, interface crossing
* Below the boundary: invariants, buffers, latency, failure, load

> Interpretation does not execute.
> Execution is indifferent to intent.

Any claim that crosses this boundary without specifying how is **ill-typed**.

---

## 3. Viability Precedence

### C6 — Viability Gate

Optimization, improvement, or evaluation claims are meaningful **only if continued execution is possible over the stated horizon**.

> Optimization without a viability witness is undefined, not wrong.

---

## 4. Closure and Degrees of Freedom

### C7 — Closure Requirement

Executable systems must terminate interpretation by fixing an exact set of degrees of freedom.

For any task, DOFs must be classified as:

* **Essential** — fixed at entry
* **Optional** — delegated within bounds
* **Latent** — preserved for versioning
* **Irrelevant** — collapsed
* **Unknown** — excluded from execution

> Any system that does not declare this partition is not agency-supporting.

---

## 5. Decidability and Agency

### C8 — Decidable Boundary

Agency exists **only** at a pre-execution boundary where:

* Accept and refuse are both executable
* Refusal has bounded, declared consequences
* Constraints are explicit before entry

> If refusal exists only narratively, agency attribution is ill-typed.

Inside execution, only discretion exists — not agency.

---

## 6. Responsibility and Load

### C9 — Load Location

Disturbance introduced by execution must land somewhere in the system topology.

> If load location is invisible, responsibility attribution is unstable.

---

### C10 — Responsibility Typing

Responsibility is typeable **only** if:

* Entry was decidable
* Relevant DOFs were declared
* Outcomes depended on controllable variables
* Failure semantics were explicit
* Load routing is legible

> Responsibility follows load, not involvement, intent, or narrative.

---

## 7. Metrics and Evaluation

### C11 — Executable Metrics

A metric is valid only if it:

* Is substitutable across evaluators
* Is computable under resource bounds
* Yields determinate outcomes
* **Fails explicitly** outside its envelope

> Metrics that never fail accumulate hidden error and are ill-typed as coordination interfaces.

---

## 8. Meaning for Coordination

### C12 — Shared Meaning Constraint

Meaning becomes real-for-coordination **only** when it is:

* Externally addressable
* Substitutable across agents
* Admitted into a protocol
* Subject to failure with cost

> Meaning that cannot fail cannot coordinate.

---

## 9. Narrative Acceptance (Non-Binding Regime)

### C13 — Narrative Non-Executability

Narrative, interpretation, and expectation can coordinate **only while acceptance holds**.

They impose:

* no invariants
* no failure semantics
* no irreversible cost

> Narrative acceptance is pre-execution only and collapses under load.

---

## 10. Redesign and Horizon Safety

### C14 — Redesign Possibility

A system must preserve (or allow recovery of):

* horizon specification
* execution vs interpretation distinction
* irreversibility awareness
* refusal / interruption points
* load traceability

> Abstractions that erase their own invalidation conditions are redesign-unsafe.

---

## 11. Power (Descriptive)

### C15 — Power Definition

Power is the capacity to **reassign disturbance and buffer ownership across nodes and horizons**.

> No execution eliminates cost.
> It only displaces it.

---

## 12. Typing Outcomes

Any claim about action, evaluation, agency, or responsibility is exactly one of:

* **Well-Typed** — coherent under these constraints
* **Under-Typed** — missing required witnesses
* **Ill-Typed** — violates constraints

This is a **three-valued system** by necessity.

---

# End of Core

This is the **entire minimal set**.

Nothing can be removed without producing invisible constraints.
Nothing can be added without over-constraining upstream.
