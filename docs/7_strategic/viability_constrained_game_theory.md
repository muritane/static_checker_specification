# Viability-Constrained Game Theory  
## Strategic Interaction Under Bounded, Irreversible, Drift-Exposed Execution

---

## Status

This document defines a constraint-consistent embedding of game-theoretic reasoning within the bounded execution stack.

It does not modify:

- Execution primitives
- Structural typing discipline
- Control layer
- Cognitive layer
- Normative layer
- Governance layer

It constrains strategic analysis to remain coherent under:

- Finite resources
- Partial observability
- Irreversibility
- Irreversible abstraction
- Drift / non-stationarity
- Horizon boundedness
- Structured topology
- Consequence propagation
- Viability precedence

Game theory is not replaced.

It is typed.

---

## Dependencies

This document depends on:

- `0_core/execution_primitives.md`
- `1_structural/typing_discipline.md`
- `2_control/control_layer.md`
- `3_cognitive/cognitive_layer.md`
- `5_normative/normative_layer.md`
- `6_governance/governance_layer.md`

It extends the stack into multi-agent strategic interaction.

It introduces no new primitives.

---

# 1. Scope

This framework applies when:

- Multiple agents interact.
- Outcomes depend on joint action.
- Incentives shape behavior.
- Actions are executed under bounded resources.
- Systems must remain viable across time.

It rejects:

- Horizon-free optimality claims.
- Stationary payoff assumptions without declaration.
- Costless reversibility.
- Infinite buffer assumptions.
- Optimization claims without viability witness.

---

# 2. Typing Environment for Strategic Claims

All strategic analysis must declare:

- **E** — Information structure (who observes what, with what latency)
- **T̂** — Consequence topology (load routing, buffer location, authority)
- **H** — Declared horizon
- **R** — Resource bounds and current margins
- **V** — Explicit viability conditions

Strategic claims without `(E, T̂, H, R, V)` are under-typed.

---

# 3. Agents Under Execution Constraints

Agents are modeled as:

- Resource-bounded (E1)
- Partially informed (E2)
- Irreversible in action (E3)
- Representationally compressed (E4)
- Drift-exposed (E5)
- Horizon-limited (E6)

Agents do not possess:

- Infinite foresight
- Infinite search capacity
- Perfect payoff knowledge
- Infinite slack

Strategic reasoning must respect bounded cognition and execution cost.

---

# 4. Viability Precedes Optimization

## 4.1 Viability Definition

A multi-agent system is viable over horizon H if:

- Each participating locus retains execution capacity.
- Critical buffers remain above collapse thresholds.
- Adaptation pathways remain accessible.
- Topology does not collapse into deadlock or destruction.

Viability is structural, not moral.

---

## 4.2 Viability Gate

Let:

```
S = set of all possible joint strategies
S_v ⊆ S = strategies preserving viability over H
```

Equilibrium analysis must be restricted to `S_v`.

Strategies outside `S_v` are executionally invalid.

Optimization over non-viable strategy space is ill-typed.

---

# 5. Payoffs Under Resource and Topology Constraints

Classical payoff functions:

```
u_i : S → ℝ
```

Viability-constrained form:

```
u_i : (S_v, T̂, R, H) → ℝ
```

Payoffs must incorporate:

- Resource consumption
- Buffer depletion
- Drift exposure
- Irreversibility cost
- Topology-based load routing

Short-term gains that erode long-horizon viability must be structurally penalized.

---

# 6. Horizon Declaration

All equilibrium claims must specify:

- Evaluation horizon H
- Discount structure (if applicable)
- Drift assumptions
- Redesign availability

Stationary equilibrium claims without horizon declaration are under-typed.

An equilibrium optimal over H₁ may destroy viability over H₂.

---

# 7. Drift and Non-Stationarity

Let:

```
P_t = payoff structure at time t
```

Drift implies:

```
P_t ≠ P_(t+Δ)
```

Viable equilibria must either:

- Remain robust under bounded drift, or
- Declare regime boundaries and redesign triggers.

Static Nash equilibrium is insufficient without drift robustness analysis.

---

# 8. Irreversibility and Path Dependence

Strategy execution:

- Consumes resources
- Alters reachable future states
- Modifies topology
- Changes payoff surfaces

Thus:

```
Reachable(S_(t+1)) ⊂ Reachable(S_t)
```

Repeated games must be treated as trajectory processes, not reset games.

Path dependence is structural.

---

# 9. Equilibrium Classification

Under viability constraint, equilibria are classified as:

## 9.1 Viable Equilibrium
Preserves execution capacity across H under bounded drift.

## 9.2 Fragile Equilibrium
Stable under static assumptions but collapses under bounded drift.

## 9.3 Buffer-Consuming Equilibrium
Maintains local stability while eroding resource margins.

## 9.4 Ill-Typed Equilibrium
Violates execution primitives or ignores viability constraints.

Classical Nash equilibrium may fall into any category.

---

# 10. Repeated Games Under Constraint

Repeated interaction requires:

- Affordable retaliation
- Drift-tolerant cooperation detection
- Buffer capacity for punishment cycles
- Explicit horizon compatibility

Strategies such as tit-for-tat are viable only if:

- Buffer ≥ retaliation cost
- Misclassification risk is bounded
- Drift does not destroy observability

Otherwise, retaliation may be self-destructive.

---

# 11. Mechanism Design Under Viability Constraint

Mechanisms must satisfy:

1. Incentive compatibility  
2. Resource feasibility  
3. Drift tolerance  
4. Load traceability  
5. Explicit failure semantics  
6. Redesign availability  

Mechanisms producing equilibrium while eroding viability are structurally invalid.

---

# 12. Power and Load Redistribution

Strategic action can:

- Shift buffer ownership
- Reassign disturbance
- Compress or extend horizons
- Modify topology

Power does not eliminate cost.

It redistributes it.

Equilibrium analysis must specify:

- Who absorbs disturbance
- Where buffers saturate
- What failure mode emerges

---

# 13. Metrics in Strategic Systems

Metrics must:

- Be computable under resource bounds
- Fail explicitly outside envelope
- Remain robust under drift

Goodhart dynamics arise when:

- Metrics become optimization targets
- Failure semantics are suppressed
- Proxy-target alignment drifts

Equilibria based on invalid metrics are fragile.

---

# 14. Organizational Example Typing

## Promotion Systems

Require declaration of:

- Retention buffer
- Cultural drift exposure
- Horizon (multi-year)
- Load redistribution topology

Zero-sum competition may be locally rational but buffer-consuming.

---

## Firing Policies

Bottom-decile policies must model:

- Trust buffer
- Sabotage incentives
- Hiring pipeline capacity
- Reputation drift

If trust buffer is viability-critical, such equilibrium may be invalid.

---

## Metric Optimization

Conversion maximization without fraud topology modeling:

- Violates consequence propagation awareness
- Produces unstable equilibrium
- Erodes long-horizon viability

---

# 15. What This Framework Does Not Do

It does not:

- Guarantee cooperation
- Eliminate conflict
- Replace classical equilibrium analysis
- Remove incentive tensions
- Override execution physics

It constrains strategic reasoning to remain execution-coherent.

---

# 16. Summary

Viability-Constrained Game Theory asserts:

1. Strategy search must occur within viability-preserving action space.
2. Optimization is undefined without survival margin.
3. Drift invalidates stationary equilibrium assumptions.
4. Irreversibility makes trajectory modeling essential.
5. Power redistributes cost but does not remove it.
6. Metrics must fail explicitly to remain valid.
7. All equilibria are horizon-bound.

Game theory predicts behavior within rules.

This framework ensures:

The rules do not destroy the system that plays the game.

---
