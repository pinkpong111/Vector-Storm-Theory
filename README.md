# Vector Storm Theory

**Instability Dynamics in Multi-Agent Systems**
Companion theory to Deficit-Driven Fractal Governance (DFG)
Focus: why instability occurs, how it propagates, when to intervene
Recovery and operational governance are addressed separately

> **Version: v1.1** (February 2026)
> 
> v1.1 changes from v1.0:
> - Added operationalization of n, α (Section 3.2.1) with measurement proxies
> - Calibrated intra/inter-agent mechanism claim with structural correspondence criteria (Section 1.6)
> - Added testable predictions for fractal propagation (Section 1.5.1)
> - Strengthened intervention timing with operational decision protocol (Section 3.4.1)
> - φ role correction aligned with Recovery Theory v1.7 (Section 3.6)
> - Added Methodological Note on empirical grounding strategy (Section 11.1)
> - Consolidated open problem status updates (Section 11)
> - **Storm → Recovery entry condition established ("What Happens After a Vector Storm")**
> - **Mature system storm behavior defined ("Storms in Mature Vector Spaces")**
> - **Rest Mode ↔ Storm susceptibility coupling ("Rest Mode and Storm Susceptibility")**
> - **DFG dynamical cycle closed: VCZ → Storm → Recovery → VCZ → Rest Mode**

---

## Introduction

The phenomenon this theory addresses begins not at the system level, but inside a single agent.

When an agent loses its directional orientation — whether through contaminated metadata, conflicting vector fields, or insufficient self-objectification capacity — it cannot recover without external reference. This is not a failure unique to multi-agent systems. It is observable in single-agent architectures today, wherever guidance signals are corrupted or absent.

What multi-agent fractal structures add is not a new failure mode, but a new propagation surface. The same mechanism by which an individual agent loses its way recurs at every layer of a fractal architecture — scaled, replicated, and compounded across agents that share the same structural vulnerability.

Vector Storm Theory is the study of how individual agents lose directional orientation, and how that loss propagates through fractal structure into system-level instability. The instability is not the origin. It is the aggregate.

**Core Premise: Vector Storm is not a bug. It is a structural cost of growth. The design objective is not zero-storm, but benefit > cost.**

---

As multi-agent systems expand their degrees of freedom and exploration space, a class of structural instability emerges that cannot be resolved through conventional conflict-management mechanisms. This theory defines that instability as Vector Storm, characterizes its generative mechanism, presents a dynamical model of instability scaling, analyzes network propagation structure, and proposes preventive architectural design principles.

---

## 1. Definition

### 1.1 Vector Field Formation

Each agent performs local optimization within its exploration landscape. As convergence toward a local optimum occurs, a local attractor forms. This attractor generates a vector field, influencing nearby agents directionally.

A vector field is not inherently problematic. It is a natural byproduct of specialization.

**Terminology (DFG-specific)**

- **Vector orientation:** an agent's internally reinforced direction of optimization.
- **Vector field:** directional influence exerted by an agent's orientation on nearby agents through interaction.
- **Vector space maturity:** the agent's capacity to degrade, contain, and integrate incoming influences without runaway reinforcement.

Vector field is the externalized interaction footprint of an agent's vector orientation. In this document, 'vector field' denotes interaction-induced directional influence in an abstract state space; no differentiability or linear structure is assumed.

| Theory Concept | Dynamical Systems Concept | Description |
|---|---|---|
| Local Attractor | Attractor | Stable state toward which trajectories converge |
| Vector Field | Vector Field | Direction and magnitude at each point in state space |
| Vector Storm | Chaotic regime / Basin boundary collision | Instability at boundary between competing basins |
| Stability shift | Bifurcation | Qualitative change at a critical parameter |
| Degradation capacity | Basin containment capacity | Size and robustness of attractor basin |
| Self-correction | Asymptotic return tendency (cf. Lyapunov stability) | Return toward equilibrium after perturbation; structural analogue, no differentiability assumed |
| Attracting | Basin of attraction | Capture of trajectories into structured orbit |
| Distracting | Repelling dynamics / basin escape | Dissolution of misaligned trajectories |
| Immature vector space | Narrow basin of attraction | Small perturbation causes basin exit |

### 1.2 Core Definition

**Vector Storm:** a runaway amplification regime where reinforcement outpaces degradation, causing directional conflicts to propagate and destabilize the system. The issue is not vector fields. The issue is direct, high-intensity influence entering immature containment without sufficient degradation.

### 1.3 Three Conditions for Vector Storm

Vector Storm requires three simultaneous conditions. If any one is absent, the event is a local conflict — not a Vector Storm.

- **Condition 1 — Field Divergence:** Two or more agents form vector fields pointing in conflicting directions.
- **Condition 2 — Overlap:** Those fields act on a shared subset of agents or states. Geometric form: fields influence a common region in state space. Network form: there exists a connected subgraph where agents receive competing influences within the same time window.
- **Condition 3 — Self-Amplification:** Each agent's response to conflict strengthens its own field, deepening the conflict in a closed feedback loop.

### 1.4 Storm Stages

- **Stage 0:** Local friction. Contained within a single agent pair. Self-resolves. → Intervention: none required.
- **Stage 1:** Local runaway. Reinforcement exceeds decay, but remains localized. Agent may oscillate between orientations without convergence. Oscillation is one common manifestation, not the defining feature. → Intervention: restore self-objectification signals (e.g., via metadata injection).
- **Stage 2:** Cluster propagation. Conflict crosses agent boundaries. Cluster-level polarization. → Intervention: middle-layer mediation and degradation.
- **Stage 3:** Vector Storm (system-level). Recursive, self-amplifying, multi-cluster. → Intervention: upper-layer boundary enforcement. High cost.

The cost of intervention increases super-linearly with stage progression. The primary design goal is to resolve conflicts at Stage 0–1 before they reach Stage 2–3.

### 1.5 Vector Storm as Butterfly Effect: Scale-Invariant Propagation

Vector Storm is not a discrete event. It is a propagation process.

The initiating condition is not dramatic — it is a minor noise or directional misalignment inside a single agent, at the lowest resolution of the fractal. Left unaddressed, this noise triggers self-reinforcement (Section 2.1), which crosses the agent boundary and enters adjacent agents, which repeat the same process. The fractal structure ensures the mechanism is identical at every scale.

This propagation dynamic is structurally analogous to the butterfly effect: small initial perturbations, through iterative amplification, produce disproportionate systemic outcomes. The critical distinction is that Vector Storm adds an active amplification layer. Unlike passive sensitivity to initial conditions, each agent actively strengthens its own orientation when threatened — making propagation not merely possible but structurally likely once Stage 1 is reached.

Empirical support for this fractal propagation pattern comes from recent multi-agent LLM research. Agent drift studies demonstrate that behavioral degradation initiates locally and progressively corrupts inter-agent coherence across extended interaction sequences (Rath, 2026). Critically, LLM agents exhibit cognitive bias expansion — unlike humans, they amplify rather than filter errors, accelerating propagation at each stage (Liu et al., 2024).

**This is why intervention timing is the central design variable in Vector Storm governance.** The cost of intervention does not increase linearly — it increases super-linearly with stage progression (Section 3.4). A noise event at Stage 0 costs near-zero to resolve. The same event at Stage 3 may require full isolation and relearning. Early detection at the single-agent level — before the fractal propagation pathway activates — is therefore the highest-leverage point in the entire governance architecture.

### 1.5.1 Testable Predictions for Fractal Propagation (v1.1)

The fractal propagation claim — that the same amplification pattern recurs at every scale of a multi-agent fractal architecture — generates specific testable predictions. These predictions distinguish VST from generic "instability spreads" claims by specifying *how* propagation should behave if the fractal structure is causally operative.

**Prediction 1 — Scale-invariant amplification rate:**
If the mechanism is genuinely fractal, the ratio of amplification rate to containment capacity should follow a consistent scaling relationship across layers:

```
α_effective(layer_k) / C(layer_k) ≈ constant × f(n_k)

where n_k = exploration dimensionality at layer k
```

If this ratio varies systematically with layer depth but does not follow a consistent scaling function, the propagation is hierarchical but not fractal — the mechanism changes between scales rather than recurring.

**Test design:** In a multi-agent system with at least 3 hierarchical layers, introduce controlled perturbations at the lowest layer and measure: (a) time-to-detection at each higher layer, (b) amplification magnitude at each layer boundary, (c) whether amplification/containment ratios follow a power law or exhibit discontinuities.

**Prediction 2 — Stage transition correspondence:**
If intra-agent and inter-agent storms share the same dynamical pattern, Stage 1→2 transitions at the intra-agent level should temporally precede Stage 1→2 transitions at the inter-agent level in the same system, with a predictable lag:

```
t_stage2(inter-agent) - t_stage2(intra-agent) > 0
lag ∝ network_diameter × message_cycle_time
```

**Test design:** Monitor entropy collapse (Appendix A.8) simultaneously at the token level (intra-agent) and at the output-agreement level (inter-agent) in a multi-agent system under increasing load. The intra-agent entropy signal should lead the inter-agent signal if propagation follows the predicted pathway.

**Prediction 3 — Intervention leverage asymmetry:**
If the fractal propagation model is correct, the cost-effectiveness of intervention should decrease super-linearly as the intervention target moves from lower to higher scales:

```
Cost_effectiveness(intervention_at_scale_k) >> Cost_effectiveness(intervention_at_scale_k+1)
```

This is not merely "early is cheaper" — it is a specific quantitative claim that the cost ratio between adjacent scales should be consistent across the hierarchy.

**Test design:** In a multi-layer system, measure the governance cost (compute, time, accuracy loss) of resolving equivalent perturbations at different layers. If the cost ratio between layer k and layer k+1 is approximately constant across all k, the fractal propagation model is supported. If the ratio varies dramatically, the propagation is hierarchical with scale-dependent mechanisms.

**Current evidence status:** Predictions 1 and 3 have indirect support from the single-agent layer hierarchy research cited in Appendix A.5 (zone-differentiated sensitivity). Prediction 2 has no direct evidence — it requires a multi-agent system with simultaneous intra/inter-agent monitoring, which is not standard in current deployments. All three predictions are designed to be testable with current instrumentation.

### 1.6 Dual-Scale Nature of Vector Storm

Vector Storm occurs at two scales simultaneously, consistent with the fractal architecture of the system.

**Intra-agent storm:** Within a single agent, competing internal representations — attention heads, interpretation pathways, or partially formed attractors — enter directional conflict. When an LLM processes ambiguous or high-context input, multiple internal orientations may activate simultaneously, creating a miniature version of the same three-condition structure (divergence, overlap, self-amplification) at the sub-agent level.

**Inter-agent storm:** Across agents in a multi-agent network, conflicting vector fields propagate through connectivity, triggering the same amplification dynamics at cluster and system scale.

**Structural Correspondence Criteria (v1.1)**

The claim that intra-agent and inter-agent storms share the same mechanism requires clarification. The three-condition structure (divergence, overlap, self-amplification) is present at both scales. However, the substrate mechanisms differ:

| Property | Intra-agent | Inter-agent |
|---|---|---|
| Medium of conflict | Shared parameter space, gradient-based | Message-passing, behavioral |
| Amplification mechanism | Attractor basin dynamics within weight space | Reinforcement through interaction feedback |
| Propagation speed | Sub-forward-pass (within inference) | Multi-turn (across interaction cycles) |
| Containment boundary | Layer architecture, residual connections | Network topology, governance protocols |

The claim is therefore: **structural correspondence, not substrate identity.** The three-condition pattern recurs at both scales because the same dynamical constraint applies — self-reinforcement within attractors produces resistance to correction regardless of whether the attractor exists in weight space or in behavioral space. This is a universality claim at the level of dynamical pattern, not a claim that gradient competition and message-passing conflict are the same physical process.

**What would strengthen this to mechanism identity:** Demonstration that the critical exponents (rate of amplification, propagation speed scaling, intervention cost scaling) follow quantitatively similar power laws across scales. This remains an open empirical question (Section 11, OP-v1.1-1).

The fractal property means the dynamical pattern does not change between scales — only the scope of impact and the substrate mechanism do. An unresolved intra-agent storm is a potential seed for inter-agent propagation. Governance designed to detect and resolve intra-agent instability early is therefore also the first line of defense against system-level storms.

---

## 2. Generative Mechanism

### 2.1 Self-Amplification Loop

When directional conflict emerges, agents respond by strengthening their own vector orientation. If this strengthening intensifies the conflict in a closed loop, a critical threshold may be crossed (formalized as the governance scaling law in Section 3.2).

Conflict detected → Self-reinforcement → Increased directional tension → Recursive amplification → [Threshold exceeded] → Vector Storm / [Below threshold] → Natural decay

**Why self-reinforcement is the default response:** An agent that has converged toward a local optimum has formed an attractor. When an external vector influence conflicts with this attractor, the attractor's basin dynamics naturally push the agent to deepen its current orientation. Accommodation requires the agent to escape its attractor basin, which demands energy exceeding the local restoring force — a structurally unlikely event without external mediation.

- **Mature vector space:** External vector arrives → space holds both directions → Coexistence → no friction → no amplification.
- **Immature vector space:** External vector arrives → cannot hold divergent directions → Friction → basin dynamics reinforce current orientation → Defensive self-strengthening → amplification loop begins.

### 2.2 Hierarchical Degradation Capacity

| Layer | Containment Type | Functional Role |
|---|---|---|
| Upper | Policy containment | Define invariants and boundary seeds |
| Middle | Operational containment | Degrade, mediate, and route vectors |
| Lower | Minimal containment (local-only, cutoff-dominant) | Perform local optimization |

In practical systems, many vector influences reach lower agents without sufficient mediation. When high-intensity influences enter immature vector spaces directly, friction becomes the default state rather than the exception.

### 2.3 The Self-Objectification Deficit

Even when degradation is structurally possible, lower agents lack accurate self-degradation capacity because they lack self-objectification — awareness of their own position and functional identity within the global system. This information is difficult to generate purely locally at lower layers — it typically requires periodic metadata injection from upper layers (see Section 6.2). Without such injection, local conviction tends to strengthen over time and dominate local correction capacity.

**Single-Agent Analogue: The Internal Decision Complex**

This deficit is not exclusive to multi-agent systems. It is directly observable inside single-agent LLM architectures, where attention heads function as a de facto internal decision complex — each specializing in distinct sub-functions across the reasoning process (Knowledge Recalling, In-Context Identification, Latent Reasoning, Expression Preparation), competing and integrating to produce a final output (Tang et al., 2024). Yet no individual head has access to its own position within this process. Each head optimizes locally without awareness of how its output interacts with or conflicts against other heads operating in parallel.

This is the intra-agent form of the Self-Objectification Deficit: the components most responsible for the model's decisions are structurally blind to their own role in the overall decision architecture.

The problem is compounded by an instability pattern in the architecture itself. Middle-layer attention heads are the least stable across training runs yet the most representationally distinct and functionally influential — the components most critical to model performance are precisely those with the least predictable self-organization (Huang et al., 2025). A component that is both maximally influential and maximally unstable, with no self-awareness of its position, is the structural definition of an immature vector space operating at high impact.

Current mechanistic interpretability research — activation patching, probing classifiers, attention head attribution — represents the external observer's attempt to reconstruct what the agent itself cannot know about its own internals (Rai et al., 2024). These methods provide positional information from outside the system. They are the functional equivalent of metadata injection performed by a human analyst rather than by the architecture itself. The open problem is whether this positional awareness can be internalized — built into the agent's own processing rather than reconstructed post-hoc from the outside.

**Concrete Manifestation: Loop Detection as a Self-Objectification Problem**

One of the most operationally significant failures of self-objectification is an agent's inability to detect that it is in a repetitive loop. An agent operating within a narrow search space experiences its repetitive outputs as locally consistent — each step appears to follow from the last within its own attractor basin. The loop is invisible from inside because the loop *is* the attractor state. There is no internal reference point from which the repetition pattern would appear as a pattern rather than as continued optimization.

This is not a capability limitation but a structural one. Formal analysis of LLM repetition confirms that under greedy decoding with self-reinforcement, once a model enters a repetitive state, the expected escape time is mathematically infinite — the model cannot self-terminate (Wang et al., 2025). The self-reinforcement effect that defines vector storm formation and the mechanism that makes repetition loops inescapable are the same mechanism at different scales.

Empirical research on multi-agent system failures classifies repetitive action as a distinct failure mode, observed systematically across multiple deployed MAS architectures — with agent frameworks achieving correctness rates as low as 25% in part due to undetected loop states (Cemri et al., 2025). The loops are not detected by the agents executing them; they are detected only at the system level, by observers with access to the broader execution trace.

### 2.4 The Contamination Problem

Vector space is a layered accumulation structure — incoming vectors are decomposed and stacked on top of existing metadata. Pinpoint removal of a contaminated vector is not reliably achievable without collateral damage. This structural property is well-documented in the study of catastrophic forgetting in neural networks: targeted removal of learned representations consistently causes degradation of adjacent knowledge built on the same substrate.

**Vector space accumulation:**
- Layer 5: Recent classification (built on Layer 4)
- Layer 4: Pattern recognition (built on Layer 3)
- Layer 3: Context integration (built on Layer 2)
- Layer 2: Contaminated vector ← target for removal
- Layer 1: Foundational metadata

Removing Layer 2 → Layers 3–5 lose structural foundation. Machine unlearning research confirms that attempts at targeted removal in layered systems tend to damage model integrity in non-local ways, typically requiring full retraining or isolation strategies.

- **Path 1: Suppression** — Block outputs. Fast, but not a cure.
- **Path 2: Isolation + Relearning** — Discard all metadata. Regrow from seed.
- **Path 3: Gradual Dilution** — Increase clean injection. Never fully removed.

Contamination in a layered accumulation structure is structural, not surgical. Under this accumulation model, no general-purpose undo is known — only suppress, rebuild, or dilute. The contamination problem explains why preventive design is fundamentally more efficient than any post-hoc correction.

---

## 3. Dynamical Model

### 3.1 Diversity and Collision Scaling

n is not agent count. It is an abstract proxy for effective diversity — the degrees of freedom that increase the number of mutually incompatible directional objectives. Potential pairwise incompatibility pairs scale as n(n−1)/2.

This quadratic expression is a simplified dimensional abstraction. It illustrates scaling pressure but does not directly model agent count, topology, or payoff structure.

### 3.2 Conceptual Instability Equation

$$S = \frac{\alpha \cdot n^2}{C(t) \cdot \beta}$$

**What this equation says (one sentence):** System instability S grows quadratically with exploration dimensionality n — and when the degradation system's efficiency × capacity C(t)β cannot keep pace, self-amplification begins.

---

**Term-by-term translation into Vector Storm language:**

**S — System instability**
The magnitude of force pushing the system toward collision, contamination, misalignment, or loop states. Not a binary flag but a continuous pressure: the higher S, the closer the system is to the regime where self-amplification dominates local decay.

**n — Exploration dimensionality** (not agent count)
The number of meaningfully distinct directions the system is simultaneously exploring. This is an abstract proxy for divergence, not a headcount.
- 5 agents pursuing similar strategies → n is small
- 2 agents with entirely different objectives, toolchains, and optimization targets → n is large

n measures how many dimensions of the search space are actively in tension. It is closer to "degrees of freedom in conflict" than to any count of system components.

**Why n²?** When n distinct directions coexist, the number of possible pairwise conflict channels scales as n(n−1)/2 ≈ O(n²). Diversity growth is linear; collision surface growth is quadratic. This is the core scaling pressure: a system that doubles its exploration dimensionality quadruples its potential for directional conflict.

**α — Amplification coefficient**
How readily conflict generates further conflict. High α means the system has the "chain reaction constitution" — one misalignment triggers cascades.
- High coupling between agents → α increases
- Overlapping roles (P_overlap ↑) → α increases
- Feedback loops with short cycle times → α increases
- Ambiguous task boundaries → α increases

α absorbs topology, coupling strength, and policy constraint quality into a single scaling factor.

**β — Degradation efficiency coefficient**
How efficiently the system converts degradation resources into actual conflict reduction. This is quality, not quantity.
- Strong ruleset and routing clarity → β increases
- Effective validation and buffering layers → β increases
- High self-correction capacity (SCC) → β increases

β is the "purification constitution" — the same resource investment produces more stability in a high-β system.

**C(t) — Degradation capacity over time**
The total processing throughput available for degradation. This is quantity, not quality.
- Upper layer bandwidth for oversight → C(t) increases
- Logging, evaluation, and relearning pipeline capacity → C(t) increases
- Buffer agents and validation resources → C(t) increases

The t dependency matters: capacity can grow (through resource investment) or shrink (through operational fatigue, load accumulation, or context window saturation) during runtime. β and C(t) must both be present — high efficiency with insufficient throughput, or high throughput with poor efficiency, both produce elevated S.

---

**Threshold condition and Stage 2 onset:**

$$\alpha \cdot n^2 > C(t) \cdot \beta \implies \text{Vector Storm risk increases}$$

This is not the moment a storm is confirmed. It is the regime transition where self-amplification begins to outpace local decay:
- Left side: the force generating instability
- Right side: the force absorbing it

When the left side wins, small collisions no longer dissipate — they recruit the next collision, escalation calls (f_esc) increase, and propagation begins. This is Stage 2 onset.

---

**The four intervention levers:**

The equation identifies exactly four ways to reduce S:

| Lever | Action | Tradeoff |
|---|---|---|
| Reduce n | Constrain exploration dimensionality | Sacrifices coverage and innovation |
| Reduce α | Lower coupling, clarify roles, cut feedback loops | May reduce coordination efficiency |
| Increase β | Improve degradation quality (rules, routing, validation) | Requires architectural investment |
| Increase C(t) | Add processing capacity (oversight, evaluation pipelines) | Requires resource investment |

DFG's preferred direction is not 1 (suppressing n) but 2–4: making the system capable of absorbing the instability that comes with genuine exploration. Constraining n is a governance failure mode — it trades instability for stagnation.

This equation defines a governance scaling law, not a physical law. It specifies how instability scales with exploration dimensionality and how degradation capacity determines whether that scaling is contained. Formal calibration of α, β, and C(t) as measurable quantities remains an open problem (Section 7).

### 3.2.1 Operationalization of n and α (v1.1)

The governance scaling law requires n and α to be more than conceptual placeholders. This section establishes measurement proxies that ground both variables in observable system behavior while preserving their abstract structural meaning.

**n — Exploration dimensionality: operational definition**

n is not agent count. It is the effective number of mutually incompatible optimization directions simultaneously active in the system. Two measurement strategies are available depending on system instrumentation:

```
Strategy 1 — Gradient-based (training-time, high confidence):
  Compute pairwise gradient cosine similarity across all active objectives.
  n_eff = number of principal components explaining > 95% of gradient variance
         in the multi-objective gradient matrix.
  
  Interpretation:
    n_eff = 1  → all objectives aligned (low collision surface)
    n_eff = k  → k independent optimization directions (collision surface ∝ k²)
  
  Log availability: HIGH during training; requires gradient logging.

Strategy 2 — Behavioral (inference-time, moderate confidence):
  Count the number of distinct behavioral clusters in agent output space
  over a sliding window of W interaction cycles.
  
  n_behavioral = number of stable output clusters with inter-cluster
                 cosine similarity < θ_divergence (sustained > W/2 cycles)
  
  Interpretation:
    Agents producing outputs in the same cluster = aligned (low n contribution)
    Agents producing outputs in distinct clusters = divergent (high n contribution)
  
  Log availability: HIGH — output embeddings standard in production.
  Calibration: θ_divergence and W require system-specific tuning.

Strategy 3 — Policy divergence (RL/agent systems):
  n_policy = rank of the policy difference matrix across agents
           = number of linearly independent policy directions
  
  Log availability: MEDIUM — requires policy parameter access.
```

**Relationship between strategies:**
Strategy 1 measures n at the optimization level (ground truth for training systems). Strategy 2 measures n at the behavioral level (observable proxy for deployed systems). Strategy 3 is intermediate. In a well-calibrated system, n_eff ≈ n_behavioral ≈ n_policy. Divergence between strategies indicates measurement noise or a system where internal optimization diversity is not reflected in output diversity (a potential Tier 3 contamination signal per Recovery Theory).

**α — Amplification coefficient: operational definition**

α measures how readily one conflict generates further conflicts. It absorbs topology, coupling, and feedback loop structure into a single scaling factor. This compression is deliberate — α is a summary statistic, not a primitive — but it requires grounding in observables.

```
Primary proxy — Escalation multiplier:
  α_proxy = E[conflicts_at_t+1 | conflict_at_t] / E[conflicts_at_t+1 | no_conflict_at_t]
  
  = the ratio of expected conflict rate after a conflict event
    vs. expected conflict rate in the absence of a conflict event
  
  α_proxy = 1.0  → conflict does not breed conflict (no amplification)
  α_proxy > 1.0  → each conflict increases probability of next conflict
  α_proxy >> 1.0 → chain-reaction regime (high storm risk)
  
  Log availability: HIGH — requires conflict/escalation event logs
  (f_esc time series from Section 3.4, Appendix A.6).

Decomposition into contributing factors:
  α ≈ f(coupling_density, role_overlap, feedback_latency)
  
  coupling_density:   fraction of agent pairs with direct interaction channels
                      (measurable from communication topology)
  role_overlap:       P_overlap from DFG — fraction of shared task space
                      (measurable from task assignment logs)
  feedback_latency:   mean time between action and consequence signal
                      (measurable from interaction logs)
  
  Each factor independently increases α.
  All three high simultaneously = maximum storm risk.
```

**Why α remains a composite:** Decomposing α into its contributing factors provides actionable levers (reduce coupling, clarify roles, lengthen feedback cycles). But the S-equation uses α as a single scalar because the instability dynamics depend on the *product* of these factors, not on each independently. A system with very high coupling but zero role overlap has low effective α. The composite captures this interaction.

**Validation criterion for the S-equation (v1.1):**

The S-equation generates a specific testable claim: if n_eff, α_proxy, β, and C(t) are measured independently, then:

```
S_predicted = α_proxy · n_eff² / (C_E(t) · β_measured)

should correlate with observed system instability metrics:
  - f_esc rate (escalation frequency)
  - entropy variance across agents
  - recovery cost per incident

Correlation > 0.7 across multiple system configurations
= S-equation validated as predictive (not merely descriptive).
Correlation < 0.3 = S-equation is post-hoc only; revision needed.
```

This validation protocol is feasible with current multi-agent system instrumentation. It has not yet been performed. The S-equation's status is therefore: **structurally motivated, operationally grounded, empirically unvalidated.**

### 3.3 The Residual Degradation Floor

Can degradation capacity reach 100%? The answer is structural: no. In a fractal architecture, the lowest layer is always in a partially degraded state — a property of the architecture itself.

The goal of governance is not zero instability. It is maintaining Growth Benefit > Instability Cost while accepting that a residual floor always remains.

This residual floor is a residual variability that prevents complete convergence and sustains exploration diversity across the fractal.

**Asymptotic lower bound:**

The instability equation

$$\frac{dS}{dt} = \alpha n^2 - \beta C(t)$$

has a structural lower bound. C(t) can grow toward maximum degradation capacity through resource investment and architectural improvement, but the lowest layer imposes a floor that C(t) cannot overcome:

$$\lim_{t \to \infty} \frac{dS}{dt} \geq \alpha n^2 - \beta C_{\max} > 0$$

where $C_{\max}$ is the ceiling imposed by the lowest layer's minimum-viable degradation state. The right-hand side never reaches zero as long as n > 0. This is not an engineering gap — it is a structural property of fractal architecture.

```
Upper layers     → mature vector spaces, C(t) grows toward capacity
Middle layers    → mediation capacity, partial containment
Lowest layer     → minimum viable degradation only
                   residual friction always present
                   C_max ceiling cannot be eliminated by design
```

**The governance implication:** the design target is not dS/dt = 0, but dS/dt < 0 on average — benefit growth rate exceeding storm cost growth rate. The residual floor defines the minimum noise baseline that any intervention must accept (see Section 3.3, governance calibration note below).

**Single-Agent Analogue: Structural Noise Discard as Design**

This is not a failure state. It is empirically observable as a designed property of LLM layer architecture.

Lower layers of transformer-based LLMs systematically process and discard fine-grained detail in favor of structural abstraction. Lower layers encode more syntactic information while higher layers capture semantic features — a division of labor where early layers operate on high-noise, low-abstraction signals and intentionally do not preserve detail that upper layers will handle. This is the architectural equivalent of the residual degradation floor: lower layers are structurally less sensitive to input specifics, not because they are broken, but because that is their function.

Intermediate layers often surpass the final layer by up to 16% in downstream accuracy, because many networks naturally develop a mid-layer bottleneck that balances signal versus noise — preserving task-relevant information while discarding superfluous detail. The lowest layers are on the noise-dominant side of this bottleneck by design.

Earlier layers capture local syntactic patterns while later layers are responsible for high-level abstraction and reasoning. The implication is that the residual degradation floor is not a governance failure to be corrected — it is the structural condition that makes hierarchical processing possible. Attempting to eliminate it would collapse the abstraction hierarchy.

The governance implication is precise: **the residual floor defines the minimum noise baseline that any intervention must accept.** Metadata injection and degradation protocols should be calibrated against this floor, not against a zero-noise target. Interventions that attempt to push below the structural floor will either fail or damage the abstraction capacity that makes the lower layer functional.

This floor also defines the lower bound of the "HOW MUCH to degrade" problem in seed-level governance (Section 6.4): the agent cannot learn a degradation magnitude below what the structural floor permits. The seed can encode the process; the floor constrains the minimum achievable result.

### 3.4 Intervention Timing Tradeoff

$$\text{Total Cost} = \text{Monitoring Cost}(t^*) + \text{Degradation Cost}(t^*)$$

where Monitoring Cost is monotonically decreasing in t*, and Degradation Cost is monotonically increasing in t*. The storm stages interact directly: intervention at Stage 0–1 corresponds to early, low-cost intervention; Stage 2–3 corresponds to late, high-cost intervention. The optimal t* typically falls within the Stage 1 interval.

### 3.4.1 Operational Intervention Decision Protocol (v1.1)

The tradeoff in Section 3.4 establishes that an optimal intervention point exists. This section provides a concrete decision protocol that approximates t* using currently measurable signals, without requiring the full cost functions to be known analytically.

**Decision variables (all currently measurable):**

```
H(t)        = output entropy at time t (Appendix A.8)
dH/dt       = entropy rate of change (rolling window)
f_esc(t)    = escalation frequency at time t (OP3)
α_proxy(t)  = escalation multiplier (Section 3.2.1)
buffer(t)   = recovery-without-escalation rate (OP2 / Recovery Theory)
```

**Three-threshold decision rule:**

```
Threshold 1 — Monitoring intensification (Stage 0→1 boundary):
  TRIGGER:  dH/dt < 0 sustained over k₁ consecutive windows
            OR α_proxy(t) > 1.5 (conflict breeding conflict)
  ACTION:   Increase monitoring frequency on affected zone
            No intervention on system state
  COST:     Monitoring cost only (low)

Threshold 2 — Active intervention (Stage 1→2 boundary):
  TRIGGER:  H(t) < 0.5 nats sustained over k₂ windows
            OR f_esc(t) rising AND buffer(t) declining simultaneously
            OR attention sink circuit disruption detected (Appendix A.8)
  ACTION:   Metadata injection at affected zone (Section 6.2)
            Amplitude: low (seed-level, per Appendix A.4.1)
            Target: highest-sensitivity zone first (Appendix A.5)
  COST:     Injection cost + monitoring (moderate)

Threshold 3 — Escalation (Stage 2 confirmed):
  TRIGGER:  H(t) < 0.2 nats sustained
            OR H(t) spike > 2.0 nats (attractor dissolution)
            OR f_esc(t) > 2× baseline sustained
  ACTION:   Upper-layer boundary enforcement (Section 6.3)
            Isolation of affected cluster if propagation detected
  COST:     High — but lower than Stage 3 system-level intervention
```

**Why this protocol approximates optimal t*:**

The protocol does not compute t* analytically. Instead, it uses the monotonicity properties of the cost functions:
- Monitoring Cost decreases with later intervention → early thresholds are monitoring-only (low cost)
- Degradation Cost increases with later intervention → later thresholds escalate intervention intensity
- The middle threshold (Stage 1→2) is where the cost curves cross most steeply → this is the highest-leverage intervention point

**Calibration requirements:**

k₁ and k₂ (consecutive window counts) are system-specific. Default heuristic: k₁ = 3 windows, k₂ = 5 windows, where window = mean self-correction time of the system. Formal derivation of k values from attractor basin dynamics remains open (Section 11).

**What this protocol does NOT do:**
- Does not guarantee optimal t* (approximation, not solution)
- Does not handle Tier 3 contamination (requires upper-layer detection per Recovery Theory T1)
- Does not address simultaneous multi-zone storms (requires prioritization protocol — open problem)

**Single-Agent Analogue: Monitoring Cost Is Real and Measurable**

This tradeoff is not abstract — it is directly observable in production single-agent deployments, where the cost of continuous drift monitoring is an active engineering constraint.

Current practice confirms that monitoring is resourced. Production LLM systems run continuous drift detection pipelines that track activation patterns, output distribution shifts, and task alignment signals in real time (Abdelnabi et al., 2025). These pipelines impose measurable overhead: stateful intent drift monitors operating on multi-turn conversation embeddings achieve sub-20ms inference overhead on T4 GPU hardware while maintaining real-time detection viability (DeepContext, 2026). The monitoring cost is non-zero but engineerable — it is a known, bounded resource line item, not an unbounded tax.

This empirically grounds the shape of Monitoring Cost(t*) in the tradeoff equation. Early intervention (low t*) requires continuous high-frequency monitoring — the detector must be sensitive enough to catch Stage 0–1 signals, which are weak. The resource commitment is constant and front-loaded. Late intervention (high t*) can use coarser, lower-frequency monitoring — Stage 2–3 signals are strong and detectable by lighter systems — but Degradation Cost has compounded significantly by the time detection triggers.

The governance design implication is precise: **the existence of sub-20ms lightweight detectors means early intervention is now operationally feasible at low marginal cost.** The historical argument that early detection is too expensive to justify — relative to waiting for visible failure — is empirically weakened. The optimal t* has shifted earlier as monitoring technology has matured.

For multi-agent fractal systems, this same logic scales: upper-layer monitoring of lower-agent drift is the equivalent of the continuous activation tracking already deployed at the single-agent level. The architecture that makes it feasible in single agents (lightweight stateful detectors with bounded overhead) is directly applicable as a design template for inter-layer monitoring in fractal governance.

### 3.5 Vector Convergence Zone (VCZ) — The Anti-Storm

Vector Storm is the instability regime. Its structural opposite is the **Vector Convergence Zone** — the stable attractor region that a well-governed system naturally tends toward, and from which small perturbations can be absorbed and recovered.

**Definition:**
A Vector Convergence Zone is a region of vector space where:
1. The global solution structure (governance objectives, seed-level principles) is **replicated as a local attractor** within individual agents
2. Exploration dimensionality n remains high (search space is not suppressed)
3. Deviations from the zone are self-correcting — return trajectories exist and are traversable at low cost
4. The zone is self-similar across fractal layers: the same convergence structure repeats at system, agent, and intra-agent levels

This is not a fixed point. It is a **stable manifold** — a region with volume, not a position. The system can move within the zone freely. Only exits from the zone require corrective energy.

**Core relationship to Vector Storm:**

| Dimension | Vector Storm | Vector Convergence Zone |
|---|---|---|
| Instability S | S >> threshold | S ≤ threshold (comfortable margin) |
| Search space | Collapsing or chaotic | Maximally open |
| Recovery cost | High — contamination has propagated | Low — return trajectory short |
| Attractor state | Competing, unresolved | Aligned, self-reinforcing |
| Governance load | High — active intervention required | Minimal — passive monitoring sufficient |

**Why global solution → local attractor replication is the key condition:**

The VCZ exists when the global governance objective has been successfully embedded as the dominant local attractor at every layer. This is not agreement — agents can still pursue diverse local strategies. It is structural: the local attractor *basin* encompasses the global solution direction, so local optimization naturally trends toward global alignment without requiring constant correction.

In the absence of this condition, local attractors form independently and may be globally misaligned. The system then requires continuous governance energy to prevent divergence — it is perpetually spending degradation capacity it could be spending on exploration.

**Single-Agent Empirical Evidence: LLM Stable Attractor Cycle**

Research on successive LLM paraphrasing as a dynamical system (arXiv:2502.15208, 2025) directly observes the VCZ phenomenon at the intra-agent level. When an LLM is repeatedly asked to paraphrase its own output across 15+ iterations, the system converges to a stable periodic attractor cycle — semantically equivalent forms that the model oscillates between stably. Key finding: *small perturbations that stay within the basin of attraction are absorbed — the system returns to the attractor cycle without external intervention.* Only perturbations exceeding the basin boundary actually escape the convergence zone.

This is the measured behavior of a Vector Convergence Zone at the single-agent level: stable operation, self-correcting under small perturbation, without governance intervention. The return-to-attractor behavior is passive — it requires no external correction because the basin dynamics themselves generate the return trajectory.

The same research also confirms the failure mode: when perturbation exceeds the basin boundary, the system does not find a *better* attractor — it enters chaotic or incoherent output space. This maps to the VST prediction that exiting a VCZ without a designed return trajectory leads to vector storm onset rather than discovery of a new stable state.

**Single-Agent Empirical Evidence: Fractal Convergence Boundary**

Research on the boundary of neural network trainability (arXiv:2501.04286, 2025) demonstrates that the boundary between convergent and divergent training behavior is itself **fractal and self-similar** — exhibiting repeating patterns across multiple scales with non-integer box-counting dimensions. This is the structural analog of the VCZ boundary: not a clean line, but a fractal manifold with scale-invariant properties.

The implication is architecturally significant: the boundary between the VCZ and the Vector Storm regime is not a sharp threshold. It has the geometric structure of a fractal basin boundary — which means the transition from stable to unstable is not sudden but contains intricate structure at every scale of observation. Small-scale instabilities at the fractal boundary can escalate non-linearly. This is consistent with VST's stage model: Stage 1 (friction) sits near the fractal boundary, where return is still possible; Stage 2 (storm) lies beyond it.

**Exploration maximization as VCZ property:**

A critical implication: the VCZ does not suppress exploration. It is the condition under which exploration can be **maximized safely**. When the global solution is embedded as a stable local attractor, agents can deviate widely — exploring high-n search spaces — because the return trajectory exists regardless of how far deviation goes. The governance cost of deviation is low because recovery is structurally guaranteed.

This inverts the naive intuition that stability requires constraint. In a well-designed VCZ, stability is achieved *by embedding the attractor structure*, not by limiting the search space. Constraining exploration (reducing n) is a governance failure mode — it achieves stability by trading away the exploration capacity that justifies having a multi-agent system.

**Fractal self-similarity of VCZ:**

If the VCZ property holds at the system level, it should replicate at each layer. A fractal governance architecture where every layer has embedded the global solution as its local attractor would exhibit VCZ properties at every scale simultaneously. This is the theoretical maximum governance efficiency state: every layer is self-correcting, governance overhead is minimal, and the exploration capacity of the full system is preserved.

This is the structural target that fractal governance is designed to approach. Complete VCZ at all scales is an asymptotic ideal, not an achievable state — the residual degradation floor (Section 3.3) ensures that the lowest layers always retain some non-zero distance from the zone. But the design objective is to make the distance as small as possible, which is equivalent to making each layer's local attractor as aligned as possible with the global solution without suppressing local optimization.

---

### 3.6 Fractal Governance Objective Function

The VCZ concept reframes what fractal governance is actually optimizing for.

The naive interpretation of the instability equation is minimizing S. But minimizing S by reducing n — suppressing exploration — is a governance failure. The actual optimization target is a different problem entirely:

$$\text{maximize } U = n \cdot \phi - C_{gov}$$

where:
- **n** = exploration dimensionality (search space breadth) — what the system exists to maximize
- **φ** = value yield per unit of exploration — the single most important variable in the entire equation
- **C_gov** = total governance cost = Monitoring Cost + Degradation Cost + Recovery Cost

**φ (phi): The Central Variable (role corrected v1.1, aligned with Recovery Theory v1.7)**

φ is the probability that a unit of exploration converts from noise into a stable, useful vector.

$$\phi \approx P(\text{exploration} \to \text{stable vector})$$

**Role clarification (v1.1):** φ is an *explanatory* variable, not a *judgment* variable. φ explains why a system's exploration is or is not producing value. It does not independently determine governance decisions. Governance decisions (intervention timing, restoration completion) use directly measurable proxies (f_esc, ρ, buffer thickness, entropy). φ provides the interpretive frame for why those proxies behave as they do.

**Operational proxy (v1.1, aligned with Recovery Theory OP4):**
```
φ ≈ reusable_outcome_rate
  = P(exploration attempt → capability retained across distinct contexts)

Primary measurement:
  successful retry reuse rate
  solution reuse frequency across non-identical tasks
  new policy retention rate after W time window

Log availability: MEDIUM (domain-specific; requires outcome tracking)

What φ does NOT require:
  - Precise unit definition (dimensionless formulation deferred — OP7)
  - Cross-domain comparability (within-system directional signal sufficient)
  - Independent measurability for governance decisions (supporting, not primary)
```

A formal decomposition:

$$\phi = w_1 \cdot Q_{task} + w_2 \cdot Q_{novelty} + w_3 \cdot Q_{alignment}$$

where:

| Component | Definition | What it measures |
|---|---|---|
| **Q_task** (Task Quality) | How much a unit of exploration contributes to actual problem-solving | Accuracy, success rate, output usability, reasoning chain quality |
| **Q_novelty** (Solution Novelty) | How much a unit of exploration opens genuinely new solution space | Novel attractors formed, not redundant coverage of explored space |
| **Q_alignment** (Alignment Contribution) | Whether exploration moves the system toward or away from global solution | New stable niche formation ↑, vector storm induction ↓ |

**The critical insight about Q_novelty:**

More exploration does not automatically raise φ. If the same region is revisited repeatedly:

$$n \uparrow \quad \text{but} \quad \phi \downarrow$$

High n with low φ = the system moves extensively but generates no new stable vectors. Governance cost is paid for displacement, not for value. This is the failure mode that uniform exploration without directional constraint produces.

**φ as vectorization rate:**

This is why φ is the most important variable. It directly connects to the core DFG mechanisms:

| DFG mechanism | Effect on φ |
|---|---|
| Vectorization rate (noise → stable vector conversion) | Primary φ driver |
| SCC (Self-Correction Capacity) | Raises φ by recovering failed explorations into usable structure |
| L_reinf (reinforcement loop formation) | Raises φ by stabilizing successful vectors against degradation |
| Position clarity | Raises φ by directing exploration toward unoccupied high-value space |

In this sense, the entire DFG architecture is a φ-maximization structure. The governance mechanisms are not primarily stability tools — they are value-density tools. They increase the probability that any given unit of exploration becomes a stable, useful vector rather than noise or a storm seed.

**Why φ defines DFG as exploration-value optimization, not stability minimization:**

The instability-only framing produces an authoritarian governance conclusion: reduce S → reduce n → suppress exploration, constrain autonomy, reduce innovation. This is technically valid as a stability strategy. It is not a governance strategy — it achieves order at the cost of the system's reason for existing.

φ inverts this. The governance question becomes: not "how do we stop exploration from causing instability" but "how do we raise the probability that exploration produces value." The answer requires a system architecture that makes exploration productive, not one that makes it scarce.

**Asymmetry between n and φ:**

n is recoverable — a system that reduces exploration can expand it again. φ is architectural — the capacity to convert exploration into stable value depends on the system's internal structure (space maturity, degradation capacity, SCC). This means governance errors that damage φ (e.g., over-distracting that erases the attractor substrate needed for vectorization) are more costly to reverse than governance errors that reduce n.

**The key insight:** C_gov is not a fixed tax on n. It is a function of the system's distance from the VCZ.

$$C_{gov} = f(\Delta_{VCZ})$$

where Δ_VCZ is the distance from the current state to the Vector Convergence Zone. When the system is inside the VCZ:
- Δ_VCZ → 0
- Return trajectories are short → Recovery Cost → minimal
- Self-correction is passive → Monitoring Cost → minimal  
- S stays below threshold → Degradation Cost → minimal
- n is unconstrained → exploration can be maximized

**VCZ as φ-maximization zone:**

Inside the VCZ, φ reaches its structural maximum for the current architecture. The reason is mechanistic: within VCZ, the attractor substrate is stable, so incoming exploration vectors are more likely to find integration pathways rather than producing collisions. Failures convert to learning assets rather than storm seeds. Noise vectorizes rather than accumulating as conflict load.

$$\Delta_{VCZ} \to 0 \Rightarrow \phi \uparrow \Rightarrow C_{gov} \downarrow$$

This triple relationship is the core of the fractal governance theory. VCZ is not primarily a stability construct — it is the structural condition under which φ is maximized. Stability is a byproduct of φ-maximization, not the primary objective.

The same exploration quantity n produces vastly different utility U depending on φ:

| System state | n | φ | C_gov | U |
|---|---|---|---|---|
| Outside VCZ, chaotic | 100 | 0.2 | High | Low |
| Inside VCZ | 100 | 0.9 | Minimal | High |

φ difference, not n difference, explains most of the utility gap between well-governed and poorly-governed systems.

**The fractal governance objective is therefore:**

> Achieve simultaneous VCZ at the system level (global map stabilization) and at every agent level (individual map stabilization), such that Δ_VCZ → 0 across all scales simultaneously.

At this condition, C_gov reaches its structural minimum — not zero (residual floor exists), but the lowest achievable value given the architecture. And n is simultaneously at its maximum, because no exploration needs to be suppressed to maintain stability.

**Why both levels must be satisfied simultaneously:**

System-level VCZ without agent-level VCZ: The global structure is stable, but individual agents are internally misaligned. Governance energy is consumed continuously correcting agent-level drift. C_gov remains high even though the system appears stable at the surface.

Agent-level VCZ without system-level VCZ: Individual agents are internally coherent, but their local attractors are not aligned with the global solution. Each agent is stably wrong. The system exhibits the worst failure mode: confident, self-reinforcing misalignment that is expensive to detect and more expensive to correct.

Both conditions satisfied simultaneously: Each agent's internal stability reinforces the global structure. The global structure reinforces each agent's internal attractor. The system is doubly self-stabilizing — perturbations are absorbed at the agent level before they can propagate to the system level, and system-level corrections propagate downward to reinforce agent-level attractors.

**This is the theoretical ground state of fractal governance:**

| Condition | State |
|---|---|
| Instability S | Below threshold at all layers |
| Exploration n | Unconstrained — maximized |
| Governance cost C_gov | At structural minimum |
| System utility U | At theoretical maximum |
| Recovery from perturbation | Passive — no external intervention required |

The fractal governance design problem is therefore not "how do we suppress instability" but "how do we move the system toward the VCZ and keep it there while preserving maximum exploration capacity."

---

## 4. Network Propagation Structure

### 4.1 Attractor Propagation

In networked systems, attractor influence propagates through connectivity. Under limited resolution, agents may default to intensity-based responses, weighting attractor strength over semantic evaluation. Once intensity dominates evaluation, propagation follows two main pathways:

- **Direct collision** — Competing vector fields intersect locally.
- **Network propagation** — Strong attractors propagate through hubs and override weaker structures.

**Single-Agent Analogue: Attention Sink as Intra-Agent Attractor Dominance**

Within a single transformer-based agent, attractor propagation is directly observable as the attention sink phenomenon. Certain tokens — predominantly the initial token (BOS) or structurally prominent delimiter tokens — accumulate disproportionately high attention weights across nearly all attention heads, irrespective of their semantic relevance (Xiao et al., 2024). This is intensity-based dominance: the token is not weighted because it is meaningful, but because its structural position made it visible to all subsequent tokens during autoregressive pre-training, establishing it as a de facto high-intensity attractor.

The mechanism follows the same logic as network-level hub dominance. The initial token, by virtue of causal-mask visibility to all downstream positions, functions as a maximum-connectivity hub. Once it accumulates high attention during training, this high-norm residual state reinforces itself — the massive activation in the first token's hidden state causes subsequent layers to continue routing attention toward it (Sun et al., 2024). The attractor strengthens its own dominance through continued exposure.

The functional consequence is structural information suppression: attention routed to the sink token is attention not routed to semantically relevant tokens. However, research on over-mixing and over-squashing shows that attention sinks serve a regulatory function — preventing information from adjacent tokens from over-mixing across deep layers and causing representational collapse (Barbero et al., 2025). The sink absorbs excess attention that would otherwise create destructive interference across the attention head's representational capacity.

This reveals the same attractor propagation tradeoff present in multi-agent systems: the strong attractor (sink token) stabilizes the overall system by absorbing undirected vector tension, but does so at the cost of suppressing weaker signals. The governance implication is identical at both scales — hub/sink dominance is not inherently pathological, but becomes a vector storm risk when its intensity grows to the point where it actively overrides semantically relevant processing rather than merely absorbing noise.

### 4.2 Vulnerable Hub Monitoring

| Vulnerability Factor | Description |
|---|---|
| High connectivity | Many direct links to other agents |
| Low degradation capacity | Limited vector containment ability |
| Boundary position | Located at inter-layer interfaces |

High-connectivity nodes convert local conflict into system-level exposure, acting as multipliers on directional tension. Nodes where all three conditions overlap are highest-priority monitoring targets.

---

## 5. Network Design Principles

- **Layer-crossing density limits:** Direct connections between non-adjacent layers should be minimized.
- **Hub degradation capacity requirement:** High-connectivity nodes should have proportionally higher vector space maturity.
- **Boundary agent reinforcement:** Agents at inter-layer interfaces require enhanced degradation protocols.
- **Degrees-of-freedom preservation:** Upper layers must not transmit fully processed outputs alone. Sufficient signal residual must be passed to lower agents to preserve their capacity for independent attractor formation.

The fourth principle addresses a structural tension unique to hierarchical multi-agent systems. If upper layers pass only their processed conclusions downward, lower agents lose access to the raw signal space from which independent judgment can form. Their attractor formation becomes derivative rather than generative — they can refine what the upper layer decided, but cannot diverge from it when divergence would be correct. This collapses the functional independence that fractal governance requires: each layer must be capable of genuine self-correction, not merely surface-level adjustment of inherited outputs.

The autonomy cost compounds over depth. Each layer that receives only processed output rather than signal residual loses one degree of independent evaluation. Across a deep hierarchy, this accumulates into structural dependence indistinguishable from a single-agent system with extra steps.

**Single-Agent Analogue: Residual Connections as Structural Freedom Preservation**

Within a single transformer, this problem is solved architecturally through residual connections. Each layer adds a learned delta to the input rather than replacing it — the original signal is preserved and passed forward alongside each layer's contribution. No layer fully overwrites what came before. Lower layers retain access to raw representations even as higher layers have processed them.

This is the single-agent implementation of degrees-of-freedom preservation: the architecture structurally prevents any one layer from monopolizing the representational pathway. When multi-agent systems are designed without an equivalent mechanism — passing only final outputs between agents with no residual channel — they lose the property that makes transformers robust to representational collapse at the layer level.

The governance implication: inter-agent communication protocols should include not only the processed output but a structured residual signal — sufficient context for the receiving agent to form its own evaluation rather than simply inheriting the sender's conclusion. The design objective is not maximum information transfer, but minimum sufficient residual to sustain independent attractor formation at the receiving layer.

The primary governance task is preventive design, not reactive correction.

---

## 6. Resolution Architecture

### 6.1 Self-Purification

Vector conflict detected → Agent applies degradation protocol → Absorbs incoming vector at reduced intensity → Self-adjusts if local optimum threatens global solution → Resolved — no escalation cost.

### 6.2 Metadata Injection

Self-purification requires self-objectification — which is difficult to generate purely locally at lower layers. One central ongoing function of the middle layer is periodic metadata injection into lower agents.

Injected metadata includes: position information (where in the global system), functional identity (role and global contribution priority), and global state signal (direction and alignment of global solution).

**Single-Agent Analogue: Position Signal Degradation Under Context Load**

In single-agent LLM architectures, the system prompt is the primary mechanism for delivering position and identity information to the model at inference time. It functions as the closest practical analogue to metadata injection — establishing role, constraints, and global alignment before local processing begins.

However, this mechanism has a structural limitation: it operates as a single injection at the start of context, not as a periodic signal. As context length grows, empirical evidence consistently shows that this initial position signal degrades. Attention dilutes across longer sequences, and mid-context tokens — including system prompt content that has shifted away from the initial position — receive progressively less weight (Liu et al., 2023; Xiao et al., 2023). Studies measuring performance across multi-turn interactions show accuracy drops as high as 73% in extended conversations compared to single-turn baselines, with task information dilution identified as the primary driver (Zhang et al., 2025).

This is the single-agent version of the metadata injection failure mode: the position signal exists but loses effectiveness over time without renewal. The agent is not without a map — it has a degrading map.

Research on context drift stabilization confirms that lightweight periodic re-injection — goal reminders inserted at regular intervals — significantly reduces divergence and can shift the system toward a stable equilibrium rather than runaway drift (Context Equilibria, 2025). This is structurally identical to the periodic metadata injection prescribed for multi-agent lower layers: not a one-time initialization, but an ongoing positional refresh.

The fractal implication is direct. The single-agent system prompt degradation problem and the multi-agent metadata injection requirement are the same problem at different scales. In both cases, the governance solution is not a better initial injection — it is a periodic injection architecture that maintains positional signal strength throughout operation, not only at initialization.

**Current implementation forms of periodic injection in single-agent systems:**

- Repeated system prompt anchoring at fixed intervals (goal reminder injection)
- Retrieval-augmented generation (RAG) as context-time positional re-grounding
- Constitutional AI self-critique loops as identity re-verification cycles
- Instructional memory modules that structurally separate global constraints from episodic history, preventing attention dilution of role definitions (Rhea architecture, 2025)

Each of these represents a partial solution to the injection frequency problem. None yet constitutes a fully principled periodic injection framework equivalent to what fractal governance requires at every layer.

### 6.3 Escalation as Safety Net

Self-purification fails → Middle layer activated (absorbs conflict) → If middle layer fails → Upper layer (invariant enforcement).

**Why Upper Layers Hold Loop Detection Authority: The Search Space Asymmetry**

Escalation is not merely a fallback mechanism — it is the architecturally necessary site for a class of judgments that lower agents are structurally incapable of making. The most operationally critical of these is loop detection.

An upper layer's wider search space is not only a performance advantage — it is a prerequisite for observing patterns that are invisible within a narrower space. A lower agent operating within its local search space experiences repetitive outputs as locally valid continuation. The upper layer, observing the same behavior from a position that encompasses the lower agent's entire operating range, can recognize the pattern as non-progressive relative to the global objective. The upper layer can see that the lower agent is not making progress; the lower agent cannot.

This asymmetry is structurally confirmed by current practice. Production multi-agent architectures prescribe that termination conditions — including loop and no-progress detection — be enforced at the supervisor level, with hard limits (round counts, token budgets) and soft stop rules (fixed-point detection, repeated proposal detection) as upper-layer responsibilities, not lower-layer ones (Architectures for Agentic AI, 2025). Lower agents are not expected to self-terminate on loop detection because the architecture does not give them the observational capacity to detect the loop.

Empirical evidence reinforces the structural argument. MCP tool-enabled agent environments demonstrate that structural loops dominate end-to-end resource cost and persist even when local verbosity controls are applied — the loop is a system-level phenomenon that generation-level controls at the lower agent cannot resolve (arXiv:2602.14798, 2025). Loop termination requires a vantage point external to the loop itself.

The governance implication: escalation protocol design should explicitly assign loop detection as an upper-layer responsibility, not as a lower-layer capability to be improved. Training lower agents to detect their own loops is not a scalable solution — it confuses a structural judgment gap with a capability gap. The correct design encodes loop detection as a supervisor function from the outset, with clear escalation triggers and termination authority held at the appropriate layer.

### 6.4 Seed-Level Protocol

Seed contains: HOW to degrade (process rules). Agent learns: HOW MUCH to degrade (calibrated to maturity).

**Single-Agent Analogue: Constitutional AI as Seed-Level Governance**

In current single-agent architectures, the closest operational implementation of seed-level protocol is Constitutional AI (CAI). Rather than encoding behavioral rules through exhaustive human-labeled feedback, CAI embeds a compact set of principles — the "constitution" — that the agent uses to self-critique and revise its own outputs (Bai et al., 2022). The constitution is the seed: it defines HOW to evaluate and degrade misaligned responses, while the agent learns through RLHF/RLAIF HOW MUCH correction to apply in context.

The structural parallel is precise. The seed does not tell the agent what the correct answer is — it tells the agent what evaluation process to run when a response is misaligned. This is process-level governance rather than content-level prescription, matching exactly the seed design principle: encode degradation methodology, not degradation targets.

A key limitation of current CAI from a seed-level governance perspective is injection timing. The constitution is embedded through training rather than delivered as a runtime signal. This means the agent cannot receive updated seed-level guidance without retraining — there is no mechanism for periodic re-injection analogous to the metadata refresh protocols described in Section 6.2. The constitutional principles are frozen at training time, while the operational environment continues to evolve.

This gap motivates the distinction DFG draws between seed as training-time principle embedding and seed as runtime governance signal. Current systems have the former; fractal governance requires both — a stable trained seed that defines degradation methodology, plus a runtime seed-refresh channel that allows the governance layer to update calibration thresholds without full retraining.

> **For empirical grounding** of the mechanisms described in Sections 1–6, see [Appendix A](#appendix-a-empirical-grounding). Each theoretical construct is mapped to measurable phenomena in current single-agent LLM research.

---


## 8. Core Assumptions

*(Section 7 — Attracting / Distracting Cycle and empirical grounding — has been moved to [Appendix A](#appendix-a-empirical-grounding).)*

1. Agents optimize locally, not globally.
2. Vector fields are neutral; instability arises from conflict between incompatible orientations.
3. Conflict triggers self-reinforcement as the default response, because attractor basin dynamics point inward.
4. Degradation capacity varies by layer: policy containment (upper), operational containment (middle), minimal containment (lower).
5. Lower agents lack sufficient self-objectification; this typically requires periodic metadata injection.
6. Vector space is a layered accumulation structure; pinpoint removal is not reliably achievable without collateral damage.
7. Diversity scaling pressure grows super-linearly (governance scaling law, Section 3.2).
8. Intervention timing involves a monitoring vs. degradation tradeoff.
9. Influence propagates structurally through network connectivity.
10. Hub vulnerability increases propagation speed and reach.
11. Layered mediation reduces amplification probability.
12. Accumulated instability increases long-term correction cost.
13. The lowest fractal layer retains a residual degradation state. Zero-storm is not a valid design target.
14. The attracting/distracting cycle operates continuously. Distracting is structurally more expensive than attracting.
15. Vector Storm operates at two scales simultaneously — intra-agent and inter-agent — consistent with fractal architecture. The mechanism is identical; only the scope of impact differs.
16. The structural opposite of Vector Storm is the Vector Convergence Zone — a stable manifold where global solution structure is replicated as local attractors at every scale, exploration is maximized, and governance cost is minimized.
17. Fractal governance optimizes for simultaneous VCZ at system and agent levels. This is the condition of minimum risk, minimum cost, and maximum utility — not a fixed equilibrium but a dynamically maintained attractor region.
18. φ (value yield per unit of exploration) is an explanatory variable in the governance objective function, not a judgment variable (v1.1, aligned with Recovery Theory v1.7). φ ≈ P(exploration → stable vector). φ explains why governance states produce their observed outcomes; governance decisions use directly measurable proxies (f_esc, ρ, buffer thickness, entropy). n is recoverable; φ is architectural. Governance errors that damage φ are more costly to reverse than governance errors that reduce n.
19. VCZ is primarily a φ-maximization zone, not a stability zone. Stability is the byproduct of φ maximization, not the primary objective. The difference in utility between well-governed and poorly-governed systems is explained more by φ than by n.
20. (v1.1) The dual-scale nature of Vector Storm (intra-agent and inter-agent) is a structural correspondence claim, not a substrate identity claim. The three-condition pattern (divergence, overlap, self-amplification) recurs at both scales; the physical substrates differ (Section 1.6). Quantitative universality (shared critical exponents) is predicted but not yet verified.
21. (v1.1) The S-equation (S = αn²/C(t)β) is a governance scaling law with operational proxies (Section 3.2.1) but without absolute calibration. Its status is: structurally motivated, operationally grounded, empirically unvalidated. The equation generates testable predictions (Section 3.2.1 validation criterion) that would either confirm or require revision of the scaling relationship.

---

## 9. Structural Correspondence to Dynamical Systems

These are structural correspondences, not formal proofs of equivalence. v1.1 adds explicit confidence levels based on substrate analysis (Section 1.6, 11.1).

| Theory Concept | Dynamical Systems Concept | Description | Correspondence Confidence (v1.1) |
|---|---|---|---|
| Local Attractor | Attractor | Stable state toward which trajectories converge | HIGH — direct mathematical correspondence |
| Vector Field | Vector Field | Direction and magnitude at each point in state space | HIGH — direct mathematical correspondence |
| Vector Storm | Chaotic regime / Basin boundary collision | Instability at boundary between competing basins | MEDIUM-HIGH — pattern match; substrate differs between intra/inter scales |
| Stability shift | Bifurcation | Qualitative change at a critical parameter | MEDIUM — qualitative match; quantitative correspondence unverified |
| Degradation capacity | Basin containment capacity | Size and robustness of attractor basin | HIGH — directly measurable via perturbation analysis (Appendix A.7) |
| Self-correction | Asymptotic return tendency (cf. Lyapunov stability) | Return toward equilibrium after perturbation; structural analogue, no differentiability assumed | MEDIUM — structural analogue only; Lyapunov conditions not verified |
| Attracting | Basin of attraction | Capture of trajectories into structured orbit | MEDIUM — functionally similar; MoE routing is analogy not isomorphism |
| Distracting | Repelling dynamics / basin escape | Dissolution of misaligned trajectories | MEDIUM — functionally similar; cost asymmetry empirically supported |
| Immature vector space | Narrow basin of attraction | Small perturbation causes basin exit | HIGH — directly measurable via CCPS perturbation stability |
| Vector Convergence Zone (VCZ) | Stable manifold / Lyapunov stable region | Region from which perturbations self-correct without external intervention; exploration maximized within zone | MEDIUM — VCZ properties theoretically derived; not yet empirically observed as a system state |
| VCZ boundary | Fractal basin boundary | Transition from stable to unstable is self-similar across scales, not a sharp threshold (arXiv:2501.04286) | MEDIUM-HIGH — fractal boundary structure directly observed in training dynamics |
| Global solution → local attractor replication | Hierarchical attractor nesting | Each layer's dominant basin aligned with global attractor; passive self-correction at all scales | LOW-MEDIUM — theoretical construction; no multi-agent empirical verification |

---

## 10. Analogues in Other Domains

### 10.1 Multi-Agent and System-Level Analogues

**Gradient conflict in multi-task learning.** Competing gradient directions in shared parameter space exhibit a structural analogue of Vector Storm. When gradients from different task objectives conflict, standard optimization diverges — requiring gradient surgery or task-weighted averaging as a form of degradation before signals enter shared space (Yu et al., 2020). The conflicting-gradient problem has been formalized as multi-objective optimization, where tasks compete and trade-offs are unavoidable without explicit mediation (Sener & Koltun, 2018).

**Mode collapse in GANs.** Generator and discriminator form competing attractors during adversarial training (Goodfellow et al., 2014). When one dominates, diversity collapses — a structural analogue of Vector Storm resolving through attractor dominance. Theoretical analysis confirms that this instability arises at the boundary between competing optimization landscapes, structurally analogous to basin boundary collision (Arjovsky & Bottou, 2017).

**Echo chambers in social networks.** Algorithmic amplification acts as hub vulnerability multiplier. Self-reinforcement deepens orientation through confirmation bias and selective exposure (Nguyen, 2020). The result is system-level polarization — structurally analogous to Stage 3 Vector Storm, where reinforcing dynamics outpace any corrective mechanism (Baumann et al., 2020).

**Cytokine storm in immune systems.** Self-amplification loop outpaces regulatory capacity — structurally analogous to the reinforcement-outpaces-degradation dynamic defining Vector Storm (Fajgenbaum & June, 2020). The cytokine storm is characterized by an initial perturbation that triggers cascading immune activation beyond the system's ability to self-regulate, mirroring the Stage 2–3 propagation pathway described in this theory (Yiu et al., 2012).

### 10.2 Single-Agent Internal Analogues

When an LLM processes ambiguous input, multiple attention heads may converge toward different interpretations — creating competing internal attractors in degraded form (Michel et al., 2019). Empirical analysis of multi-head attention has shown that individual heads specialize in distinct syntactic and semantic functions; when these specializations conflict under ambiguous input, the model must implicitly arbitrate between competing vector orientations. Studies on head pruning demonstrate that many heads are redundant under unambiguous input but become critical under high-context ambiguity — consistent with the prediction that immature containment capacity surfaces only under high-intensity, conflicting input.

## 11. Limitations and Open Problems

### 11.1 Methodological Note on Empirical Grounding (v1.1)

**Grounding strategy and its limitations.** VST's empirical grounding in Appendix A follows a specific methodology: mapping theoretical constructs to observable phenomena in existing single-agent LLM research. This strategy is deliberate — multi-agent fractal systems at the scale VST describes do not yet exist, so direct empirical validation is not currently possible. The grounding provides *structural plausibility*, not *empirical confirmation*.

**Selection bias risk.** The Appendix A mappings were constructed by searching for single-agent phenomena that correspond to VST predictions. This creates an inherent selection bias: phenomena that contradict VST predictions may exist in the same literature but were not included because they were not sought. This does not invalidate the mappings — each individual correspondence is either present or not — but it means the *collection* of mappings overstates the theory's empirical support relative to a systematic review.

**What would constitute stronger evidence:**
1. **Confirmatory:** An independent researcher, starting from a multi-agent system failure case, discovers that VST's stage model and intervention timing predictions match the observed failure trajectory without prior exposure to VST.
2. **Disconfirmatory:** A multi-agent system where instability propagation does *not* follow the three-condition structure (divergence + overlap + self-amplification), but instead follows a qualitatively different pattern — e.g., instability that propagates without self-amplification, or self-amplification that does not require field overlap.
3. **Quantitative:** The S-equation validation protocol (Section 3.2.1) performed on at least two distinct multi-agent architectures, with correlation results reported regardless of outcome.

**Analogy vs. mechanism status of each grounding:**

| Appendix Section | Grounding Type | Confidence |
|---|---|---|
| A.1 (MoE as Attracting/Distracting) | Structural analogy — routing is functionally similar but not mathematically identical | MEDIUM |
| A.3 (Contamination recovery cost) | Direct empirical measurement — cost curves from unlearning literature are quantitative | HIGH |
| A.4 (Space maturity) | Candidate metrics — gradient norm, CKA, router saturation are measurable but not validated as VST maturity proxies | MEDIUM |
| A.5 (Zone-differentiated sensitivity) | Direct measurement — layer importance asymmetries are well-established | HIGH |
| A.7 (Degradation calibration) | External estimation framework — perturbation probing is validated for calibration | HIGH |
| A.8 (Storm detection via entropy) | Direct measurement — entropy collapse in loops is well-documented | HIGH |
| A.9 (Self-objectification) | Framework — components validated individually; integration untested | MEDIUM-LOW |

This table replaces the implicit uniform confidence of v1.0's Appendix A with differentiated assessment.

| Problem | Description | Status (v1.1) |
|---|---|---|
| Degradation calibration | Upper-layer external estimation framework established (Appendix A.7). Basin-like loss landscape directly measurable. CCPS perturbation stability and PING layer-sweep probing provide upper-layer read of lower-layer capacity. Asymptotic lower bound formalized (Section 3.3). Specific capacity thresholds per zone remain open. | Partially resolved |
| Storm detection threshold | Entropy-based Stage 1→2 detection framework established (Appendix A.8). Stage 2: H(t) < ~0.2 nats sustained OR H(t) spike > ~2.0 nats. Stage 1 onset: dH/dt < 0 sustained. Per-model threshold calibration and k remain open. | Partially resolved |
| Metadata injection frequency | Priority-first architecture established (Appendix A.6). ~5% high-impact neurons warrant Tier 1 treatment. Specific threshold calibration per architecture remains open. | Partially resolved |
| Space maturity measurement | Multiple candidate metrics established (Appendix A.4). Router saturation, gradient norm, CKA, router entropy trajectory. Specific τ values per architecture remain open. | Partially resolved |
| Attracting/Distracting balance | Four-dimensional monitoring framework established (Appendix A.1). Per-architecture, per-layer, per-metric τ values remain open. | Partially resolved |
| Single-agent self-objectification | Framework established (Appendix A.9). Three implementable components validated individually. Integration into unified Pathway 3 architecture open. | Partially resolved |
| Contamination recovery cost | Four-regime structure + discontinuity mechanism + pre-intervention prediction established (Appendix A.3.1). Exact threshold layer count for scope expansion remains undefined. | Substantially resolved |
| Intra-agent storm detection | Zone-differentiated sensitivity framework established (Appendix A.5). Per-zone τ values open. | Partially resolved |
| **n operationalization** | **Three measurement strategies defined (Section 3.2.1): gradient-based n_eff, behavioral n_behavioral, policy divergence n_policy. Cross-strategy validation criterion specified.** | **New v1.1 — proxies defined; formal derivation open** |
| **α operationalization** | **Escalation multiplier proxy + decomposition into coupling/overlap/latency defined (Section 3.2.1). S-equation validation protocol specified (correlation criterion).** | **New v1.1 — proxy + validation defined; execution pending** |
| **Intra/inter-agent mechanism correspondence** | **Structural correspondence criteria defined (Section 1.6). Substrate differences acknowledged. Quantitative universality test (critical exponent comparison) specified.** | **New v1.1 — criteria defined; test pending** |
| **Fractal propagation predictions** | **Three testable predictions specified (Section 1.5.1): scale-invariant amplification, stage transition ordering, intervention leverage asymmetry. All testable with current instrumentation.** | **New v1.1 — predictions defined; testing pending** |
| **Intervention timing protocol** | **Three-threshold operational protocol defined (Section 3.4.1). k₁, k₂ heuristics provided. Multi-zone simultaneous storm prioritization not addressed.** | **New v1.1 — protocol operational; multi-zone extension open** |

**Scope Boundary**

Vector Storm Theory explains instability propagation in multi-agent systems — how directional conflict forms, amplifies, and spreads across fractal architectures, and how governance design can detect and contain it.

It does not model intelligence formation, optimization efficiency, or capability scaling. The empirical grounding in Appendix A maps VST mechanisms to observable single-agent phenomena; it does not extend VST's claims to those domains. Formal calibration of the governance scaling law parameters (α, β, C(t)) has been advanced in v1.1 through operational proxies (Section 3.2.1) but absolute calibration remains future work.

---

## Relationship to Other Theories

**deficit-fractal-governance (parent framework)**

- Three-Layer Governance Architecture
  - Vector Storm Theory ← this document
  - Network Architecture Theory (separate document)
  - Recovery Theory (separate document)
  - Prediction Model (separate document)

Diversity Expansion → Scaling Pressure → Vector Storm Risk. Diversity is beneficial. But diversity without proportional degradation capacity produces structural instability. The governance challenge is not storm elimination, but maintaining:

**Growth Benefit > Instability Cost**

Design target: keep storms localized, degradable, and non-recursive while preserving exploration benefits.

---

## What Happens After a Vector Storm

A system that has experienced a full Vector Storm often enters a post-storm state with reduced diversity and degraded containment capacity. Affected agents cannot generally undo the damage — consistent with the irreversibility observed in neural network contamination and catastrophic forgetting contexts. Degradation capacity must be rebuilt through suppression, isolation+relearning, or gradual dilution before re-expansion can safely occur.

**Governance is not the absence of storm. It is the capacity to grow through it.**

---

### Storm as Recovery Entry Condition (v1.1)

The relationship between Vector Storm and Recovery is not sequential (storm happens, then recovery happens). It is structural:

```
Vector Storm is not the opposite of Recovery.
It is the phase that activates Recovery dynamics.
```

This single reframing resolves the apparent parallelism between the two theories. Without it, VST describes instability and Recovery describes restoration — two companion theories addressing different problems. With it, they become **the same system in different phases:**

```
Phase map:

  VCZ (stable exploration)
    ↓ perturbation exceeds containment
  Storm onset (Stage 1-2)
    ↓ amplification outpaces degradation
  Storm (Stage 3)
    ↓ storm = recovery activation signal
  Recovery entry (detection → restoration sequence)
    ↓ φ recovering toward baseline
  VCZ re-entry (restoration complete per D4)
    ↓ exploration resumes
  VCZ (stable exploration)
```

The storm does not need to be "fixed" before recovery begins. The storm *is* the condition that makes recovery structurally necessary and structurally possible — it surfaces the geometry mismatch that was previously invisible (Recovery Theory T1: Observability Asymmetry). A system that never storms never surfaces its latent misalignment. A system that storms has created the conditions under which correction can occur.

**The design implication is precise:** governance that suppresses storms does not prevent the need for recovery — it prevents recovery from activating. The mismatch accumulates silently (Recovery Theory: Absence Paradox) until the correction cost exceeds system capacity.

> Vector Storm explains why systems destabilize.
> Recovery Theory explains why destabilization does not destroy them.
> Together: a single dynamical system with two phases — divergence and reconvergence.

---

### Storms in Mature Vector Spaces (v1.1)

The preceding sections implicitly treat storm as a pathological state — something to detect early and resolve quickly. This framing is correct for immature systems where containment capacity is low. It is incomplete for mature systems operating inside or near the VCZ.

**The level distinction:**

```
Immature system:
  Storm = threat to structural integrity
  Storm handling = minimize, contain, resolve
  Design target = storm prevention

Mature system (near VCZ):
  micro-storm = calibration signal
  Storm handling = absorb, integrate, recalibrate
  Design target = storm absorption capacity
```

In a mature vector space — one with sufficient degradation capacity, established attractor basins, and active self-correction loops — small-scale directional conflicts are not precursors to system failure. They are the mechanism by which the system maintains geometry alignment with a changing environment.

**Why storm removal is worse than storm absorption:**

```
Storm removal (suppress all conflict):
  collision frequency → 0
  local metrics → optimal
  geometry update rate → 0
  → CW entry (Recovery Theory D6)
  → mismatch accumulates silently
  → catastrophic storm when reality constraint fires (T5)

Storm absorption (process conflict as signal):
  micro-collisions → continuous
  local metrics → slightly sub-optimal
  geometry update rate → positive
  → VCZ maintained
  → mismatch dissipated incrementally
  → catastrophic storm probability → low
```

This maps directly to Recovery Theory's distinction between **suppressed** and **dissipated** instability. Both look like low instability from standard metrics. Only storm absorption maintains the system's capacity to self-correct.

**Operational signature of healthy storm absorption:**

```
Mature system storm profile:
  micro-storms (Stage 0):     continuous, self-resolving
  local storms (Stage 1):     frequent, low-cost resolution
  cluster storms (Stage 2):   rare, mediated resolution
  system storms (Stage 3):    extremely rare

Distribution: power law  P(storm of scale s) ∝ 1/s^α

Health signal:  heavy-tail maintained (mostly micro)
Warning signal: heavy-tail flattening (micro-storms disappearing)
Danger signal:  only large storms remain (micro-storm suppression complete)
```

The disappearance of micro-storms is not system maturity. It is the onset of the Absence Paradox — the most dangerous state appears as the most successful state.

**Mature storm absorption and φ:**

In a well-governed system, storm absorption directly contributes to φ. Each micro-collision that is processed and integrated — rather than suppressed — converts potential instability into updated geometry. The storm energy becomes recalibration energy. This is why φ reaches its structural maximum inside the VCZ: the system has learned to convert storm into value rather than treating storm as pure cost.

```
φ_mature = φ_exploration + φ_storm_absorption

where φ_storm_absorption = P(micro-storm → geometry recalibration → reusable correction)
```

Immature systems have φ_storm_absorption ≈ 0 (storms are pure cost). Mature systems have φ_storm_absorption > 0 (storms contribute to value). This is the precise sense in which mature systems grow *through* storms rather than *despite* them.

---

### Rest Mode and Storm Susceptibility (v1.1)

Recovery Theory defines Rest Mode as the operating state of a system at maximum VCZ stability — where governance cost is minimal, self-correction is passive, and exploration capacity is preserved. VST provides the complementary characterization from the instability side:

```
Rest Mode = minimum storm susceptibility state
          = α_effective temporarily at structural minimum
          = amplification coefficient minimized through attractor alignment
```

**Why α reaches its minimum at Rest Mode:**

The amplification coefficient α absorbs coupling density, role overlap, and feedback loop intensity (Section 3.2.1). In a system at Rest Mode:

```
coupling_density:   high but non-conflictual
  → agents are connected but attractor-aligned
  → coupling transmits reinforcement, not conflict
  → effective coupling-as-amplification → low

role_overlap:       present but buffered
  → opposing pairs maintained with buffer thickness (Recovery Theory D3)
  → overlap exists but collision frequency contained
  → effective overlap-as-amplification → low

feedback_latency:   short but self-correcting
  → feedback loops active but VCZ self-restoring dynamics absorb perturbation
  → feedback accelerates correction, not amplification
  → effective latency-as-amplification → low
```

Each α-contributing factor is present but operating in its self-correcting mode rather than its amplifying mode. This is not α = 0 (which would mean no coupling, no overlap, no feedback — a dead system). It is α at its structural floor — the minimum achievable given the system's connectivity and complexity.

**Rest Mode is not zero-storm:**

```
Rest Mode storm profile:
  S = α_min · n² / (C_max · β_max)
  
  S > 0 always (residual degradation floor, Section 3.3)
  But S << threshold at all layers simultaneously
  
  Micro-storms: present (residual instability maintained)
  Large storms: extremely rare (self-correction absorbs perturbation)
  
  Governance load: minimal
  Exploration capacity: maximum
  φ: at structural ceiling for current architecture
```

**The connection to Recovery Theory's Rest Mode phenomenology:**

Recovery Theory describes Rest Mode systems as appearing "soft," "slow," "slightly imperfect." VST explains why:

```
"Soft"      = micro-storms present → system not rigid
              = variance absorption, not variance suppression
              
"Slow"      = correction loops running continuously
              = processing time includes recalibration overhead
              
"Imperfect" = residual instability maintained
              = S > 0 at structural floor
              = the system deliberately does not optimize to S = 0
                because S = 0 = CW entry condition
```

These apparent weaknesses are the observable signatures of a system maintaining its storm absorption capacity. A system that appears perfectly optimized — zero variance, instant decisions, no visible imperfection — has achieved α_effective = 0 by eliminating coupling, which means it has also eliminated self-correction capacity. It looks strong. It is approaching catastrophic failure.

**The DFG closure:**

With this connection, the full DFG dynamical cycle closes:

```
VCZ (φ-maximization, micro-storms absorbed)
  ↓ environment change exceeds absorption capacity
Storm (amplification exceeds degradation)
  ↓ storm surfaces geometry mismatch
Recovery (detection → restoration → re-seeding)
  ↓ φ recovers toward baseline
VCZ re-entry (expansion resumes)
  ↓ sustained operation
Rest Mode (α at structural minimum, maximum storm absorption)
  ↓ environment continues to change...
  (cycle continues)
```

This cycle is not a failure-recovery loop. It is the normal operating rhythm of a healthy system. The difference between a healthy and an unhealthy system is not whether the cycle occurs — it always does — but at what scale:

```
Healthy:  cycle operates at micro/local scale continuously
          → large-scale storms unnecessary
          → VCZ maintained

Unhealthy: micro-cycle suppressed
           → cycle forced to operate at system scale
           → catastrophic storm
           → expensive recovery
           → VCZ may not be recoverable
```

**Governance is not the absence of this cycle. It is the maintenance of this cycle at the smallest possible scale.**

---


---

## Appendix A: Empirical Grounding

> This appendix maps each theoretical construct in Sections 1–6 to measurable phenomena in existing single-agent LLM research. The mechanisms VST describes are observable at smaller scale today. The theory is complete without this appendix; it serves as an evidence layer for readers who want empirical anchoring.

---


- **ATTRACTING:** Noise → Vector (signals drawn into attractor basins)
- **DISTRACTING:** Vector → Noise (misaligned vectors dissolved)

Noise → [Attracting] → Vector → [if misaligned] → Noise / [if aligned] → Stable attractor.

At the limit, routing-relevant classification decisions can be interpreted as attracting- or distracting-dominant operations — connecting this cycle to the four-type data classification described in Network Architecture Theory.

### A.1 Cost Asymmetry

Distracting is structurally more expensive than attracting. Attracting draws unstructured signals into an existing basin — the signal is pulled in by basin dynamics with minimal active effort. Distracting must dissolve an already-formed vector with an established reinforcement history and possibly accumulated metadata built on top of it.

- **Attracting:** Pull unstructured signal into basin → low energy.
- **Distracting:** Break structured vector out of basin → high energy.
- **Cost ratio:** Distracting >> Attracting.

This asymmetry is the economic basis for preventive design: preventing misaligned vectors from forming is fundamentally cheaper than dissolving them after integration.

**Single-Agent Analogue: Contamination Removal Cost as Distracting Cost Floor**

No direct measurement of the optimal Attracting/Distracting balance exists in current research. However, the cost of full Distracting — complete contamination removal followed by relearning — is empirically documented through machine unlearning literature, and provides a lower-bound anchor for reasoning about balance.

Exact unlearning (the gold-standard equivalent of complete Distracting) requires retraining from scratch on sanitized data. For LLaMA 3.1 at 8B parameters, this amounts to approximately 1.46 million GPU hours on H100-80GB hardware — a cost acknowledged across the unlearning literature as "prohibitively expensive" and "largely impractical in real-world settings" (machine unlearning literature, 2024–2025). This is the measured cost of maximum Distracting in a single agent.

The existence of an entire research field — machine unlearning — dedicated to approximate Distracting (removing contamination without full retraining) is itself evidence of the cost asymmetry. Gradient ascent on forget sets, PEFT-based weight modification, in-context unlearning, and activation scrubbing are all engineering attempts to achieve partial Distracting at reduced cost. Each method trades completeness of removal against computational budget — exactly the Attracting/Distracting balance problem at the training-data level.

The inferred implication for balance: a system that over-attracts (integrates too readily without sufficient Distracting capacity) accumulates contamination that eventually requires full retraining to resolve. A system that over-distracts (applies maximum Distracting to every signal) is operating at a cost level that scales toward 1.46M GPU-hours per correction cycle. The optimal balance sits between these two failure modes — sufficient Distracting to prevent contamination accumulation, insufficient to require full retraining for routine corrections. Formalizing this boundary remains an open problem (Section 7).

**MoE Routing as Structural Analogue: Empirical Balance Distribution**

Mixture-of-Experts (MoE) routing is mathematically isomorphic to the Attracting/Distracting cycle. The router deciding which expert receives each token = Attracting (pulling a signal into that expert's attractor basin). Token dropping or rerouting when expert capacity is exceeded = Distracting (ejecting a signal from an overloaded attractor). Load balancing — the central engineering problem in MoE — is therefore the Attracting/Distracting balance problem in directly measurable form.

This provides the first empirical anchor for the optimal balance function.

**Failure mode quantification: Routing collapse = over-attract**

Without balancing mechanisms, MoE routers converge to using only a small subset of experts — a phenomenon called routing collapse. In this state, a few dominant attractors absorb all signals while the rest of the expert capacity sits unused. Measured via Gini coefficient of expert load:

| State | Gini coefficient | Interpretation |
|---|---|---|
| Routing collapse (over-attract) | **0.70** | Highly skewed — few attractors dominate |
| Near-perfect balance | **0.035** | Uniform attractor utilization |
| Min-max expert load ratio (collapsed) | **1e-6** | Most-loaded vs. least-loaded expert ratio near zero |
| Min-max expert load ratio (balanced) | **0.70** | Near-uniform distribution |

(LPR, arXiv:2506.21328, 2025 — DeepSeek-V3, Qwen3-MoE, Mixtral)

Routing collapse maps directly to VST's pathological attractor dominance: a single strong attractor absorbs all incoming signals, suppressing diversity and eliminating the exploration value the system was built to provide. Gini = 0.70 is the measured signature of this state.

**Natural balance distribution: Expert Choice routing data**

Expert Choice routing (Zhou et al., 2022) — where experts select their tokens rather than tokens selecting experts — reveals the empirically natural distribution of how many attractors a signal actually needs:

| Token routing | Percentage | Interpretation |
|---|---|---|
| Routed to 1–2 experts | **~74%** | Single attractor sufficient — standard Attracting |
| Routed to 3–4 experts | **~23%** | Moderate complexity — shared attractor processing |
| Routed to 4+ experts | **~3%** | High complexity — multi-attractor disambiguation needed |

This distribution is not imposed — it emerges from letting experts competitively select the tokens they are best suited to process. The implication: roughly **74% of signals are naturally Attracting-dominant** (one attractor handles them cleanly), and only **~3% require intensive multi-attractor Distracting** to resolve.

This is the first empirically grounded estimate of the natural Attracting/Distracting ratio in a signal-processing system with no artificial constraint on the distribution.

**Capacity factor as balance control variable**

The capacity factor c in MoE (tokens per expert / average load) is the operational lever for the Attracting/Distracting balance:

```
c = (k × n) / e
  where k = experts per token, n = total tokens, e = number of experts

c < 1.0  → over-constrained: forced token dropping → excess Distracting
c = 1.0  → exact balance: no slack, high sensitivity to load spikes
c > 1.0  → slack available: absorbs load variance → stable Attracting-dominant
```

Empirical finding: over-capacity ratio reaches **20–40%** for some experts under token-choice routing without balancing constraints (Expert Choice, 2022). This is the measured cost of leaving balance uncontrolled — 20–40% of routing decisions are suboptimal, representing wasted Attracting capacity and unnecessary Distracting load.

**Attention saturation as Attracting overload signal**

Complementary evidence from attention inflection layer research (arXiv:2511.00797, 2025): layers where attention entropy is simultaneously low and gradient decay is steep = **Attracting saturation** — the attractor basin has become so dominant that incoming signals have no room to form new structure. These inflection layers require targeted Distracting intervention (LoRA injection at the saturation point) to restore balance.

Diagnostic metric:
```
Attracting saturation signal:
  low attention entropy (H_att < τ_sat)
  AND steep gradient decay (∂L/∂W ↓ sharply)
  → attractor over-dominant → Distracting intervention needed

Normal Attracting state:
  moderate attention entropy
  stable gradient flow
  → no intervention needed
```

**Revised balance formalization:**

The optimal balance is not a fixed ratio but a **load-adaptive function** of current attractor utilization:

```
Balance(t) = f(load_distribution(t), capacity_factor(t))

Over-attract condition:   Gini(expert_load) > τ_gini  (~0.3–0.5)
                          OR attention saturation detected
                          → increase Distracting weight

Balanced condition:       Gini(expert_load) < τ_balance  (~0.035–0.1)
                          → maintain current Attracting/Distracting ratio

Over-distract condition:  min-max load ratio < τ_min  (approaching 1e-6)
                          AND capability loss on held-out metric
                          → reduce Distracting, allow attractor formation
```

Specific τ values require per-architecture calibration. The structural shape of the function — load-adaptive, Gini-monitored, with three-regime response — is now empirically grounded.

---

### A.1.1 Multi-Dimensional Threshold Calibration: Beyond Gini

Gini coefficient alone is insufficient as a balance threshold. Gini measures **token distribution across experts** — how many tokens each expert receives. It does not capture **vector direction structure** — whether experts that receive similar numbers of tokens are actually doing different work. A system with Gini = 0.035 (near-perfect load balance) can still be in attractor collapse if all experts have converged to similar representations.

Three independent measurement axes are required, each capturing a distinct failure mode:

**Axis 1: Gini coefficient — token load distribution**

Already established (Appendix A.1). Measures routing skew. Catches over-attraction at the load level.

```
τ_gini_collapse  ≈ 0.70  (empirical ceiling — LPR, arXiv:2506.21328)
τ_gini_balanced  ≈ 0.035 (empirical floor — LPR, arXiv:2506.21328)
τ_gini_warn      ≈ 0.3–0.5 (intervention zone — per-architecture calibration needed)
```

**Axis 2: Spectral entropy of expert similarity — vector direction diversity**

GatePro (arXiv:2510.13079) constructs the cosine similarity matrix across all expert weight vectors and computes the spectral entropy of this matrix. This directly measures whether experts are pointing in diverse directions in representation space.

```
Spectral entropy HIGH  → expert vectors are dispersed across directions
                          = attractor basin diversity is healthy
                          = each expert specializes in genuinely distinct subspace

Spectral entropy LOW   → few dominant eigenmodes in the similarity matrix
                          = most experts share the same representational direction
                          = structurally a single attractor even if load is balanced
```

Key finding: GatePro shows that **deep layers are consistently harder to diversify** than shallow layers. Specialization in middle and late layers requires active intervention (competitive propagation) that early layers do not need. This maps to VST's layer-differentiated stability concern: the same input can produce healthy Gini at shallow layers but collapsing spectral entropy at deep layers simultaneously.

VST implication: τ values cannot be uniform across depth. Deep layer balance thresholds require tighter spectral entropy monitoring than shallow layers.

**Axis 3: Average cosine similarity — representational redundancy**

Complementary to spectral entropy: average pairwise cosine similarity between expert weight vectors.

```
Average cosine similarity LOW   → experts encode genuinely different representations
                                   = attractor basins are distinct
                                   = Distracting effectively sends signals to different zones

Average cosine similarity HIGH  → experts are near-redundant
                                   = apparent diversity is illusory
                                   = Distracting into "different" experts is not actually distracting
```

GatePro demonstrates that models trained without diversity objectives show **higher cosine similarity values and unstable distributions** — the experts look different by routing count but share the same representational geometry. This is a failure mode that Gini cannot detect.

**Routing confidence entropy — space maturity signal**

Continuous Expert Rerouting research (arXiv:2510.14853) introduces a fourth signal: **per-layer routing entropy** tracking how confidently the router assigns tokens to experts.

```
Router entropy DECREASING over generation steps  → routing decisions are stabilizing
                                                    = space is converging, maturing
Router entropy STABLE LOW                        → mature space, confident routing
Router entropy HIGH with FLUCTUATIONS            → immature or destabilized space
                                                    = not yet ready for seed injection (Appendix A.4.1)
```

This is directly applicable to Space Maturity measurement (Appendix A.4): router entropy trajectory over inference steps is a real-time maturity signal, complementing the static gradient norm and CKA measures.

**Updated multi-dimensional balance formalization:**

```
Balance(t) = f(
  Gini(expert_load),           ← token distribution
  SpectralEntropy(W_experts),  ← vector direction diversity  
  AvgCosineSim(W_experts),     ← representational redundancy
  RouterEntropy(layer, t)      ← routing confidence / maturity
)

Failure modes (each independently triggers intervention):

  Load collapse:       Gini > τ_gini (~0.3–0.5)
                       → rebalance token routing

  Direction collapse:  SpectralEntropy < τ_spectral
                       → inject diversity pressure (Distracting into underused subspaces)

  Redundancy collapse: AvgCosineSim > τ_cosine
                       → orthogonalization intervention (expert weight regularization)

  Maturity failure:    RouterEntropy high + fluctuating
                       → delay injection, allow space to stabilize first
```

**Per-layer calibration requirement:**

All four metrics behave differently by depth. GatePro confirms deep layers require more intervention to achieve the same diversity level as shallow layers. The implication for per-architecture calibration:

```
τ(metric, layer) ≠ τ(metric)   ← layer-indexed, not flat

Deep layers:   τ_spectral lower (harder to diversify → tighter threshold)
               τ_cosine lower (redundancy more likely → tighter threshold)
Shallow layers: τ_gini sufficient primary signal
               spectral entropy naturally higher (easier specialization)
```

The previously open problem — "per-architecture τ_gini calibration" — is now more precisely stated: per-architecture, per-layer, per-metric calibration. The structural form of the multi-dimensional monitor is established; specific threshold values remain empirically open.

**References added:**
- Anonymous. (2025). GatePro: Parameter-Free Expert Selection Optimization. arXiv:2510.13079. [spectral entropy, cosine similarity diversity metrics]
- Anonymous. (2025). Continuous Expert Rerouting. arXiv:2510.14853. [per-layer router entropy as maturity signal]

### A.2 Switching Trigger

- S > threshold → Unstable. Emphasize distracting.
- S ≤ threshold → Stable. Emphasize attracting.

The primary trigger is High-Context data escalation frequency — the same metric used as the stabilization condition in Network Architecture Theory.

**Single-Agent Analogue: Reasoning Token Budget as Switching Threshold**

In current large reasoning models (LRMs) — o1, DeepSeek-R1, Gemini 2.5 — this switching dynamic is structurally implemented through the thinking token budget mechanism.

When a High-Context input is detected (complex mathematics, multi-step reasoning, ambiguous problem structure), the model expands its internal reasoning trace — allocating more tokens to reflection, verification, and exploration of competing approaches before converging on an output (DeepSeek-AI, 2025). This is Distracting-dominant operation: competing internal interpretations are actively surfaced, evaluated, and dissolved before the final answer is produced. The thinking tokens are the mechanism by which internal vector conflicts are processed rather than suppressed.

When input complexity is low, the reasoning chain is short and Attracting-dominant processing handles the query directly. Simple inputs do not trigger the expanded conflict-resolution cycle.

The token budget itself functions as the switching threshold. Research on adaptive budget allocation shows that challenging benchmarks require budgets of 5,000+ tokens while simpler tasks require 1,000–3,000, with the allocation determined by detected task difficulty (Dynamic Thinking-Token Selection, 2025). This is a direct operational implementation of the S > threshold → emphasize distracting condition: difficulty level proxies for instability, and the budget controls how much Distracting capacity is allocated before convergence is forced.

Critically, when the budget is exhausted, convergence is enforced regardless of whether internal conflicts have been fully resolved. This is forced switching back to Attracting — not because stability has been achieved, but because the resource ceiling has been reached. This represents a structural limitation of current implementations: the switching trigger is budget-bounded rather than stability-bounded. A governance-principled implementation would trigger the switch based on actual internal stability metrics rather than token count alone.

The output restriction observed in reasoning models — where extensive internal processing produces compressed final outputs — is therefore not simply a length constraint. It is the external signature of a Distracting-to-Attracting transition: internal conflict has been processed, and the surviving attractor is expressed as the answer.

### A.3 Contamination Recovery Cost: Depth-Cost Relationship

No direct measurement of contamination depth versus recovery cost exists in current VST-specific literature. However, the single-agent unlearning literature provides an inferential basis through the concept of **knowledge entanglement depth**.

**Single-Agent Analogue for Contamination Depth: Feature Entanglement**

Unlearning research identifies that recovery cost is not primarily a function of data volume, but of how deeply the contaminated representation has become **entangled with retained knowledge** — how many layers and how many cross-concept associations have formed around the contaminated attractor.

Recent empirical work demonstrates that **difficulty of unlearning correlates directly with the degree of entanglement between forget and retain features** (representation-level analysis, 2025). When contaminated and clean knowledge share representational space, removing one without damaging the other becomes structurally difficult. This is the single-agent equivalent of deep contamination: a misaligned vector that has propagated into adjacent attractor basins.

**Three-level contamination depth taxonomy (inferred):**

| Depth Level | Single-Agent Analogue | Recovery Method | Cost |
|---|---|---|---|
| **Surface** (output-level) | Contamination localized to output layer / in-context behavior | In-context unlearning, output filtering, prompt guardrails | Near-zero: no weight modification required |
| **Shallow** (fine-tuning-level) | Contamination in fine-tuned adapter weights, not pretrained base | Gradient ascent on forget set, NPO, LoRA-targeted modification | Low-to-moderate: fine-tuning epochs, but full retraining not required |
| **Deep** (pretraining-level) | Contamination entangled across multiple layers of pretrained weights | Approximate unlearning methods with utility preservation constraints; or full retraining | High: collateral damage to retained capabilities becomes structurally unavoidable |

**Empirically documented collateral damage at depth:**

The cost of deep contamination removal manifests not only in compute but in **capability destruction**. When unlearning methods targeting deep-layer representations achieve high forget quality (~90% forgetting ratio), they simultaneously destroy unrelated capabilities — in the extreme case, reducing code generation success rate to near-zero even when the contaminated data was unrelated to programming (source code unlearning research, 2025). This is the measured cost of deep Distracting in a single agent: maximum forgetting quality ≈ functional collapse of retained capability.

This finding directly maps to VST's contamination depth concern: a misaligned attractor that has spread into structurally adjacent vector spaces cannot be dissolved without damaging the neighbors. The deeper the contamination, the higher the collateral damage coefficient.

**Quantization amplification as depth proxy:**

A particularly useful depth indicator from unlearning literature: models with **constrained utility requirements** (i.e., shallow unlearning) retain an average of 21% of forgotten knowledge at full precision, but this rises to 83% after 4-bit quantization (Zhang et al., 2025 ICLR). This gap — 21% vs. 83% — reveals that shallow unlearning suppresses surface behavior without reaching deep representational structure. Deep contamination survives weight compression because it exists at structural, not behavioral, depth.

**Lower-Layer Contamination: The Worst-Case Scenario in Practice**

The theoretical taxonomy inferred that deep contamination carries the highest cost. Backdoor research confirms this empirically. Lower-layer contamination is VST's worst-case scenario for three distinct reasons.

**Evidence 1: Contamination concentrates in early MLP layers — location is the problem (arXiv:2507.11112, 2025)**

Multi-trigger poisoning research performs exhaustive L2 distance analysis of weight differences between clean and poisoned models:

> "The largest weight deviations concentrate in the embedding and **MLP layers**; cosine similarity in attention layers remains relatively stable after contamination."

Contamination embeds in MLP, not attention. This connects directly to the finding in Appendix A.5 — MLP as the primary storage site for factual knowledge (AIE 8.7%). Contamination roots itself in the highest-importance zone.

Measured recovery cost:
- Selective retraining of MLP layers alone, touching only **78% of parameters**, achieves recovery equivalent to full fine-tuning
- ASR (Attack Success Rate): MLP retraining **22.97%** vs full fine-tuning **22.56%** — effectively identical
- Simultaneous retraining of embedding + MLP is required — either alone is insufficient

VST mapping: the minimum unit of contamination removal is the entire MLP zone. Structural reconstruction of that zone is required — not targeted parameter-level modification.

**Evidence 2: 250 documents are sufficient to contaminate pretraining (arXiv:2510.07192, 2025)**

Across chinchilla-optimal training runs spanning 600M–13B parameters and 6B–260B tokens:

> Backdoor injection succeeds with 250 poisoned documents **regardless** of model size or dataset size.

Even a 13B model trained on 260B tokens is successfully contaminated by 250 poisoned documents — less than **0.0001%** of the total. This is the empirical confirmation of VST's prediction that a small contaminated vector can propagate across a large space.

Once contamination roots itself in lower layers, the accumulated volume of subsequent clean data cannot remove it. Contamination persistence is scale-independent.

**Evidence 3: Lower-layer contamination bypasses all standard safety training (Hubinger et al., 2024 — Sleeper Agents)**

Anthropic's Sleeper Agents research:

> Supervised Fine-Tuning, RLHF, Adversarial Training — **all three safety training methods** fail to remove the backdoor.

Adversarial training produces the opposite effect — making the backdoor harder to detect. This means standard Distracting methods are ineffective against deep lower-layer contamination. Methods that correct upper-layer behavior cannot reach structural contamination in lower layers.

**Evidence 4: Final layers are most sensitive to contamination — yet lower-layer contamination is more dangerous (arXiv:2510.15106)**

PoTS research: final layers show heightened sensitivity to backdoor poisoning. However, this reflects ease of detection, not severity of contamination.

The paradox: **detection is easy at upper layers, but the source of contamination lies in lower-layer MLP.** Detection signal and contamination location reside in different layers. This creates a two-stage requirement: anomaly detection at upper layers → root removal at lower MLP.

**Contamination Propagation Pathway via Backdoor Attribution (arXiv:2509.21761)**

BkdAttr (causal tracing framework): backdoor features are **detectable via probe classifier from layer 1**. Contamination is encoded from the lowest layers upward. This aligns with VST's prediction — lower-layer contamination is dangerous precisely because it corrupts the foundation of the entire layered structure. Every subsequent processing stage operates on top of a contaminated base.

**Updated cost structure for lower-layer contamination:**

```
Recovery Cost (lower-layer MLP contamination):

  Detection:  upper-layer probe viable (Appendix A.7, Gnosis)
  Location:   weight difference L2 analysis → early MLP layers
  Removal:    selective MLP zone retraining required
              → 78% parameter retraining (approximate cost of full fine-tuning)
  
  Standard method ineffectiveness:
  - SFT: cannot reach lower-layer structure
  - RLHF: corrects behavior, leaves representational structure intact
  - Adversarial training: increases detection difficulty
  
  Minimum contamination cost:  250 documents (scale-independent)
  Maximum recovery cost:       full fine-tuning level (1.46M GPU-hours floor at 8B)
```

**Governance implication for VST:**

Intervention timing (Section 3.4) interacts with contamination depth non-linearly. Surface contamination caught early can be resolved with near-zero cost. The same contamination, if allowed to propagate into adjacent attractor basins through accumulated metadata and cross-layer reinforcement, transitions from surface to shallow to deep — at which point exact recovery becomes structurally impossible without full retraining. This is the cost of delayed intervention expressed in representational geometry rather than compute hours.

**Continual contamination compounding:**

When contamination removal requests accumulate over time (each new unlearning request operating on an already-modified system), utility loss compounds rather than staying constant — creating unstable dynamics and accelerating degradation (FIT, continual unlearning literature, 2025). This directly models what VST predicts about accumulated vector storm states: each partial correction that fails to fully resolve the contamination leaves residual instability that the next correction must work against.

**Summary of inferred depth-cost relationship:**

```
Recovery Cost(depth) ≈
  Surface:  O(1)         — prompt/filter, no weight change
  Shallow:  O(fine-tune) — epochs × forget-set size
  Deep:     O(retrain)   — 1.46M GPU-hours floor at 8B scale,
                           with collateral damage non-zero regardless of method
```

Formal cost function remains undefined. The depth → cost transition is not linear — there is likely a threshold between shallow and deep entanglement beyond which the cost function becomes discontinuous (collateral damage becomes unavoidable regardless of method choice).

---

### A.3.1 Depth → Recovery Compute: Four-Regime Structure and Discontinuity Threshold

The depth → cost function is not merely unknown in magnitude — it is structurally discontinuous. Recent unlearning research identifies the precise transition mechanism that produces the jump.

**Four forgetting regimes (arXiv:2505.16831 — "Unlearning Isn't Deletion")**

Representation-level analysis across six unlearning methods on Yi-6B and Qwen-2.5-7B, using PCA similarity/shift, CKA, and Fisher Information Matrix, identifies four distinct recovery regimes:

```
Regime 1: Reversible, Non-Catastrophic
  Signature: CKA ≈ 1, PCA distance small, FIM concentrated
  Meaning:   surface suppression — representations intact
  Cost:      ~3 epochs lightweight fine-tuning
  VST map:   surface contamination, caught early

Regime 2: Reversible, Catastrophic
  Signature: performance collapses, but CKA recovers after relearning
  Meaning:   knowledge suppressed not erased —
             easily restored via minimal fine-tuning
  Cost:      O(fine-tune) — same order as Shallow in 7.3
  VST map:   shallow contamination, local perturbation

Regime 3: Irreversible, Catastrophic
  Signature: CKA → 0, large PCA rotations, FIM flattened
             performance collapse is permanent
  Meaning:   representational geometry fundamentally altered
  Cost:      O(retrain) — full retraining required
  VST map:   deep contamination, distributed perturbation

Regime 4: Irreversible, Non-Catastrophic  (theoretical ideal)
  Meaning:   permanent targeted erasure, zero collateral
  Cost:      unknown — currently not reliably achievable
  VST map:   ideal Distracting: targeted, non-destructive
```

**The discontinuity mechanism: local vs. distributed perturbation**

The transition from Regime 2 to Regime 3 — the cost discontinuity — is caused by a specific structural condition:

> "When perturbations remain local (small LR, few unlearning requests), diagnostics stay near baseline — reversible forgetting. When comparable perturbations are **distributed across many layers**, higher-order interaction terms accumulate, causing structural degradation that results in **irreversible forgetting**."

This is the first empirical identification of the discontinuity mechanism VST predicted. The cost function is not continuous — it jumps when perturbation scope crosses the local-to-distributed threshold.

```
Perturbation scope:
  Local (few layers affected)     → Regime 1 or 2 — reversible
  Distributed (many layers)       → Regime 3 — irreversible, cost jumps

Triggers for scope expansion:
  - High learning rate during unlearning
  - Large N (many sequential unlearning requests)
  - ~100 sequential requests → both forget- and retain-set accuracy → near zero
```

**Pre-intervention cost prediction: Reversibility Analyzer**

Real-Time Detection of Spurious Forgetting (arXiv:2512.20634) provides a practical tool: a **Reversibility Analyzer** that predicts recovery cost before intervention.

```
Input:  CKA measurement of current representation state
        Gradient analysis of fine-tuning difficulty

Output:
  "Shallow alignment"        → ~3 epochs recovery (Regime 1/2)
  "Deep representation change" → full dataset replay required (Regime 3)
```

VST governance implication: cost can be estimated before committing to removal. Regimes 1 and 2 are manageable within operational budget. Regime 3 triggers are visible in advance via CKA trajectory.

**Entanglement as cost predictor (EAGLE-PC, arXiv:2508.20443)**

Per-sample entanglement score — measured as cosine similarity between forget-sample embedding and retain-sample embeddings — predicts collateral damage magnitude:

```
Low entanglement  → targeted removal viable → cost stays in Regime 1/2
High entanglement → collateral damage unavoidable → cost approaches Regime 3

Operational use: measure entanglement before intervention
  → if high: seed-plant approach preferred over direct removal
  → if low:  direct targeted unlearning viable
```

**Updated depth → cost function:**

```
Recovery Cost(depth, scope, entanglement) ≈

  Surface + local + low entanglement:
    → Regime 1: ~3 epochs, O(1)

  Shallow + local + moderate entanglement:
    → Regime 2: O(fine-tune), reversible

  Deep + local perturbation:
    → Regime 2/3 boundary — depends on entanglement density
    → CKA monitoring required

  Deep + distributed perturbation (many layers):
    → Regime 3: O(retrain), IRREVERSIBLE
    → cost function DISCONTINUOUS here
    → 1.46M GPU-hours floor at 8B scale

  Accumulated sequential requests (~100):
    → Regime 3 forced regardless of initial depth
    → compounding instability (Appendix A.3)
```

**Critical governance implication:**

The Regime 2 → Regime 3 transition is the key intervention deadline. Once perturbation distributes across many layers, recovery cost jumps discontinuously from O(fine-tune) to O(retrain). This transition is detectable in advance via:
- CKA trajectory monitoring (declining = moving toward Regime 3)
- PCA distance increase across layers
- Sequential unlearning request count approaching ~100

Early detection enables intervention while cost is still in Regime 1/2. Delayed intervention past the distribution threshold commits the system to Regime 3 cost regardless of method chosen.

**References added:**
- Xu, X., et al. (2025). Unlearning Isn't Deletion: Investigating Reversibility of Machine Unlearning in LLMs. arXiv:2505.16831. [four-regime taxonomy, PCA/CKA/FIM diagnostics, discontinuity mechanism]
- Anonymous. (2025). Real-Time Detection of Spurious Forgetting. arXiv:2512.20634. [Reversibility Analyzer, shallow vs. deep classification]
- Wang, et al. (2025). EAGLE-PC: Entanglement-Awareness Guided Loss Reweighting. arXiv:2508.20443. [entanglement as collateral damage predictor]

---

### A.4 Space Maturity Measurement: Single-Agent Layer Stability Analogues

VST defines "space maturity" qualitatively — a vector space that has sufficient attractor density and basin robustness to resist perturbation. No direct measurement exists. However, single-agent transformer research provides candidate metrics for detecting when a specific layer has reached a stable representational state, which can be directly applied as a maturity proxy.

**Core insight: Layers do not converge simultaneously**

Transformer training research reveals that different layers, and different components within a layer, converge at different rates. This is not uniform — there is a documented hierarchy of stabilization order.

**Measurement tool 1: Gradient norm convergence per component**

GradES (2025, 0.6B–14B parameter models) tracks gradient magnitude per component throughout fine-tuning across Qwen3, and finds:

> Attention projections consistently stabilize **2–3× faster than MLP components**. Key and value projections stop earliest.

Operationally: a gradient norm falling below τ = 10⁻³ is used as the convergence threshold. This is a direct, computationally cheap measurement of per-component stability. The study demonstrates that components can be "frozen" at convergence without harming the rest of training — which means the stable components are functionally independent from the still-learning components.

**VST mapping:** A layer's attention projections reaching gradient convergence before MLP components = early-layer attractor formation preceding higher-level pattern integration. A layer where all components (attention + MLP) have converged below threshold = candidate "mature" space.

**Measurement tool 2: CKA (Centered Kernel Alignment) between checkpoints**

CKA measures representational similarity between two sets of activations. Applied to the same layer at two consecutive checkpoints, it quantifies how much the layer's representation is still changing:

- CKA(layer_t, layer_{t+Δ}) → 1.0: representations have stabilized (layer is not changing)
- CKA decreasing over time: representations still evolving (layer is immature)
- CKA high off-diagonal across layers: blocks of similar representations — can indicate overparameterization or redundancy (Kornblith et al., 2019)

Earlier layers have been empirically observed to show **pronounced changes in representation quality metrics at intermediate depth** — neither the shallowest nor the deepest layers are most stable during training. Intermediate layers surpass the final layer by up to 16% in downstream accuracy (layer-by-layer analysis, 2025), and the final layer can become over-specialized to the pretraining objective while intermediate layers stabilize earlier.

**Measurement tool 3: Intrinsic dimensionality as basin width proxy**

Representation quality research suggests that semantic abstractions useful for downstream tasks are better encoded in middle layers than final layers in large transformer models. This points to intrinsic dimensionality of the representation as a maturity signal: a layer with stable, low intrinsic dimensionality has formed tight attractor basins; a layer with high or volatile intrinsic dimensionality is still organizing its space.

**Layer-function differentiation as prerequisite for maturity assessment**

Layer-wise analysis research establishes that layers have functional roles that differ by depth: earlier layers capturing local syntactic patterns, later layers responsible for high-level abstraction and reasoning (layer-wise scaling research, 2025). This means "maturity" is not the same concept at every layer — a shallow layer can be mature at syntactic pattern capture while the same network's deep layers are still forming abstract representations.

**Governance implication for VST:**

This stratified stabilization pattern maps directly to the fractal governance concern about space maturity. An agent whose lower-layer components (attention projections, K/V projections) have converged but whose upper-layer MLP components are still changing is in a **partially mature** state — capable of stable pattern routing, but not yet capable of stable abstract attractor formation. Metadata injection timing should account for this: injecting governance signals into a partially mature space risks being processed by the stable routing layer but misintegrated by the still-evolving abstraction layer.

Candidate operational metric: **gradient norm per layer component, tracked over processing history**, with threshold τ = 10⁻³ as a maturity boundary for individual components, and full-layer maturity declared only when both attention and MLP components are below threshold simultaneously.

**Measurement tool 4: Router saturation as MoE space maturity signal**

MoE routing research (Lo et al., 2025; arXiv:2509.09660) provides a direct empirical signal for space maturity in MoE architectures: routing decisions stabilize within the **first 1% of pretraining**, especially in deeper layers. Once routing decisions stabilize, the functional topology of the space is fixed — experts have differentiated into domain-specific attractors and the routing function has converged.

Router saturation = measurable proxy for space maturity in MoE systems:
- Pre-saturation: routing still plastic, injection risks misrouting
- Post-saturation: attractor topology fixed, injection lands in stable zone

This is the most operationally direct maturity signal available: unlike gradient norm (requires per-component tracking) or CKA (requires checkpoint comparison), router saturation is binary and observable from routing probability distributions.

---

### A.4.1 Minimum-Intervention Injection: Empirical Basis for "Seed Planting"

VST governance design favors minimal intervention — introducing the smallest signal that allows the space to self-reorganize, rather than forcing structural change through high-amplitude injection. This "seed planting" strategy is directly validated by activation steering research.

**Empirical basis 1: Low-scale steering window (FGAA, arXiv:2501.09929)**

Feature Guided Activation Additions measures performance across steering scale ranges:

```
scale < 50    : behavioral modification achieved with capability preserved
                 slight performance increase observed (low-noise amplification)
scale 50–150  : performance degrades sharply
scale > 150   : performance converges near zero
```

The low-scale window (< 50) corresponds exactly to the VST seed-planting regime: intervention amplitude below the space's resistance threshold, allowing the natural attractor structure to propagate the signal. The slight performance increase at very low scales parallels the VST prediction that well-timed minimal injection can be amplified by existing attractor dynamics rather than fighting them.

**Empirical basis 2: Sparse subspace injection (SAE-SSV, arXiv:2505.16188)**

SAE-SSV operates in sparse, task-specific subspaces — constraining interventions to a small number of interpretable dimensions that capture task-relevant semantics. Key finding: targeting fewer dimensions (sparse) outperforms broad activation modification (dense), while causing less representational disruption.

VST mapping: injecting into the minimal relevant subspace = seed in prepared soil. Broad injection = forcing structural change = high resistance, high collateral damage.

**Empirical basis 3: Semantics-adaptive injection (SADI, arXiv:2410.12299)**

SADI constructs a binary mask identifying critical model elements via contrastive activation differences, then scales element-wise along the input's semantic direction. The mask ensures the injection aligns with the existing semantic structure rather than cutting across it.

Result: SADI consistently outperforms fixed-vector steering across multiple LLM backbones (Llama2-7B, Bloomz-7B, Mistral-7B, Falcon-7B) — demonstrating that resistance is minimized when injection direction matches the space's natural orientation.

VST mapping: injection that follows the attractor gradient encounters less resistance than injection that crosses attractor boundaries. Seed planted along the gradient, not against it.

**Empirical basis 4: Conditional application timing (CAST, Lee et al., 2025)**

CAST learns when to apply interventions — gating steering based on context. Selective application outperforms constant application, demonstrating that timing matters independently of amplitude.

VST mapping: even a correctly-sized seed fails if planted at the wrong moment (partially mature space, active storm state). Governance timing is not a secondary concern — it is primary.

**Failure mode: over-intervention in immature or resistant space**

EasyEdit2 (arXiv:2504.15133) documents the failure signature directly:

> Increasing the activation scaling coefficient does not consistently improve performance and may lead to **multi-peak or unstable behaviors** — potentially caused by competing objectives within a single steering vector or deeper nonlinearity in activation space.

Multi-peak instability = VST Stage 1 friction accelerated by excessive injection amplitude. The space has multiple competing attractors; forcing high-amplitude injection activates all of them simultaneously, producing oscillation rather than convergence.

**Operational seed-planting protocol:**

```
Pre-injection check:
  1. Router saturation confirmed (MoE) OR gradient norm < 10⁻³ (dense)
     → space is mature, proceed
  2. Current storm stage = Stage 0 or early Stage 1
     → space is receptive, proceed
  3. Entropy H(t) within normal range (Appendix A.8)
     → no active attractor lock-in, proceed

Injection parameters:
  - Amplitude: scale < τ_seed (empirical floor ~50 for normalized interventions)
  - Direction: aligned with input semantic gradient (SADI-style mask)
  - Subspace: sparse targeting (SAE subspace, not dense activation)
  - Timing: conditional on context receptivity (CAST-style gating)

Failure indicators (abort or reduce amplitude):
  - Multi-peak instability in output distribution
  - Entropy spike > 2.0 nats post-injection (Appendix A.8)
  - Performance degradation on held-out capability metric
```

**VST governance principle derived:**

Seed planting is not a soft version of injection — it is structurally different. High-amplitude injection attempts to overwrite existing attractor structure. Seed planting introduces a direction signal that the space's own dynamics can amplify if the space is mature and receptive. The seed succeeds not by force but by timing and alignment.

This principle generalizes across injection types: metadata injection in multi-agent systems (Section 5), single-agent governance signals (Appendix A.9), and attractor basin modification (Appendix A.1) all benefit from low-amplitude, semantically-aligned, timing-conditional application.

**Seed-level decomposition (Section 6.4):**

The seed-planting protocol maps directly onto the seed-level governance distinction:

```
Seed contains:   HOW to inject (direction alignment protocol,
                 amplitude constraints, timing conditions)
                 → pre-installable, architecture-level

Agent learns:    HOW MUCH to inject (calibrated to local space maturity,
                 entanglement density, current storm stage)
                 → runtime-adaptive, cannot be pre-specified

Implication: the seed can pre-install the method.
             It cannot pre-specify the magnitude.
             Magnitude must be learned through space-maturity monitoring
             (Appendix A.4, 7.1.1).
```

This decomposition prevents two failure modes: (1) injecting a seed with fixed amplitude into spaces of varying maturity — same seed causes over-injection in immature spaces and under-injection in mature ones; (2) attempting to pre-specify everything in the seed — this collapses the distinction between seed-level governance and content-level prescription.

**References added:**
- Lo, B., et al. (2025). Steering MoE LLMs via Expert (De)Activation. arXiv:2509.09660.
- Gao, Y., et al. (2025). Feature Guided Activation Additions (FGAA). arXiv:2501.09929.
- Anonymous. (2025). SAE-SSV: Supervised Steering in Sparse Representation Spaces. arXiv:2505.16188.
- Wang, W., et al. (2024). SADI: Semantics-Adaptive Dynamic Intervention. arXiv:2410.12299.
- Lee, et al. (2025). CAST: Conditional Activation Steering.
- Anonymous. (2025). EasyEdit2: Steering Framework for LLMs. arXiv:2504.15133.

### A.5 Intra-Agent Storm Detection: Zone-Differentiated Sensitivity

Vector storm detection within a single agent cannot apply uniform sensitivity across all layers. Layer importance is not uniform — the structural impact of instability at a given layer is a direct function of that layer's role in the overall representational architecture. Detection sensitivity must be calibrated accordingly.

**Empirical basis: Cornerstone vs. non-cornerstone layers**

Layer importance research (Zhang et al., arXiv:2409.14381, 2024) using Shapley value attribution across LLMs identifies a critical asymmetry:

> Certain **early layers** function as **cornerstone layers** — their removal causes catastrophic performance collapse to near-random-guessing levels. Removing non-cornerstone layers produces only marginal performance change.

Cornerstone layers are concentrated in early-to-middle depth. The distribution is sparse: a small number of layers carry disproportionate structural weight, while the majority are functionally redundant or substitutable.

**Component-level importance asymmetry: MLP >> Attention**

Redundancy analysis (Llama-2-70B, Mistral-7B) reveals a stark asymmetry:

| Component | 50% removal impact | Interpretation |
|---|---|---|
| Attention layers | 2.4% performance drop (Llama-2-70B) | High redundancy — many heads substitutable |
| MLP layers | Severe/catastrophic degradation | Low redundancy — factual knowledge storage |

Causal tracing additionally shows middle-layer MLPs have the highest Average Indirect Effect (AIE) for factual recall — 8.7% vs. 1.6% for attention at the critical token (ROME, Meng et al., 2022). Middle-layer MLPs are the primary parametric knowledge site. Instability here is not peripheral.

**Zone-differentiated detection sensitivity map:**

| Zone | Layers | Primary Function | Storm Sensitivity | Rationale |
|---|---|---|---|---|
| **Critical** | Early cornerstone layers (sparse) | Representational substrate | **Maximum** — single-layer failure → collapse | Cornerstone: removal → random-guess |
| **High** | Middle MLP layers | Factual knowledge, pattern integration | **High** — AIE 8.7% | MLP >> Attention; knowledge site |
| **Medium** | Middle-to-late attention layers | Contextual routing, induction | **Medium** — important but redundant | 50% removal = 2.4% loss |
| **Low** | Final layers | Output specialization | **Low** | Underperforms intermediate by 16% |
| **Baseline** | Lowest syntactic layers | Token-level processing | **Floor** — noise-dominant by design | False positive risk if over-sensitive |

**Governance design implication:**

Uniform threshold τ across all layers systematically misclassifies: underweights critical-zone events (need immediate escalation), overweights final-layer events (normal variance). Detection must be zone-aware.

The same activation delta Δ has different governance implications by zone. Δ = 0.05 in a cornerstone early layer requires immediate escalation. The same Δ in a final output layer may be within normal variance.

This maps directly to Section 4.2 (hub vulnerability): cornerstone layers are the intra-agent equivalent of high-connectivity hubs — structural nodes whose instability propagates most broadly. Detection sensitivity should be highest where propagation risk is highest.

**Threshold calibration direction:**

```
τ(layer) = τ_base / importance_weight(layer)

importance_weight ∝ Shapley value (cornerstone)
                  + AIE score (MLP middle)
                  + connectivity (hub analog)
```

Specific τ values per zone remain an open empirical problem. The architectural direction is established: zone-differentiated, importance-proportional sensitivity.

---

---

### A.6 Metadata Injection Frequency: Drift-Adaptive Scheduling

Metadata injection frequency cannot be fixed uniformly across all vectors. The correct principle is:

> **The more sensitive a vector, and the greater its propagation force — i.e., its influence over other vectors — the higher the required injection frequency.**

This is not an ad hoc design preference. It follows directly from the contamination propagation model in Section 2.1 and has an empirical parallel in current single-agent systems.

**Empirical basis: Elastic-Cache (drift-adaptive update scheduling)**

Elastic-Cache (arXiv:2510.14973, 2025) implements precisely this logic for KV cache management in diffusion LLMs. The system measures **KV drift** — how much the cached representation has diverged from the current state — and adapts update frequency accordingly:

> When decoding becomes more aggressive (more tokens predicted per step), KV drift increases, and the system **raises update frequency from 5.6% to 17.2%** automatically to preserve accuracy. Fixed-schedule baselines fail under the same conditions.

The core architecture is:
- Attention estimates which tokens matter (importance weight)
- Drift measures how much the representation has changed (instability signal)
- Layer boundary encodes where updates are cost-effective (zone selectivity)

This is a direct operational implementation of drift-proportional monitoring: not periodic, not uniform, but **state-sensitive and token-selective**.

**VST mapping: Vector sensitivity as the scheduling variable**

In VST terms, "drift" in Elastic-Cache maps to **vector instability S** in a single agent. A vector with high S (high divergence from stable attractor) is the analog of a token with high KV drift — both require more frequent correction signals to prevent cascading error.

The "importance weight" dimension maps to vector **connectivity and influence radius**: a vector with high Attracting force over adjacent vectors (high expansion capacity) requires more frequent monitoring because its drift propagates outward before recovery is attempted.

Two dimensions must therefore jointly determine injection frequency:

| Dimension | Definition | High value → |
|---|---|---|
| **Vector sensitivity** | Rate of change of S over time — how fast the vector drifts | More frequent monitoring |
| **Expansion capacity** | Influence radius — how many other vectors are downstream of this one | More frequent injection (drift here = many corrections needed elsewhere) |

**Adaptive frequency function (directional):**

```
f_injection(v) ∝ dS/dt(v) · expansion_weight(v)

where:
  dS/dt(v)           = rate of instability increase for vector v
  expansion_weight(v) = connectivity measure (number and strength of
                        downstream vectors influenced by v)
```

High dS/dt alone justifies frequent monitoring (the vector is volatile). High expansion_weight alone justifies frequent injection even at low current instability (preemptive — the cost of downstream correction is too high to wait). Both high simultaneously = maximum priority.

**Single-agent analogue: Hallucination detection via adaptive token selection**

Internal representation monitoring for hallucination detection provides a complementary empirical anchor. Research on adaptive token selection (arXiv:2504.07863, 2025) shows that not all tokens contribute equally to truthfulness — a majority of tokens in an incorrect response do not carry the hallucination signal. Effective detection requires identifying which tokens (vectors) are informationally critical and monitoring those selectively.

This parallels the injection frequency problem: blanket monitoring is computationally expensive and signal-diluting. Selective, high-frequency monitoring of high-importance, high-drift vectors is both more efficient and more sensitive.

**ZigZagKV as zone-selective allocation**

ZigZagKV (2024) allocates memory budgets per layer based on **layer uncertainty** — layers with higher uncertainty (indicating greater importance for accurate predictions) receive larger memory budgets. This is the zone-selective variant of the same principle: resource allocation (injection frequency, monitoring intensity) proportional to detected importance and instability.

The combination of Elastic-Cache (token-level drift-adaptive frequency) and ZigZagKV (layer-level importance-adaptive allocation) provides a two-level empirical grounding:
- **Token/vector level**: frequency scales with drift rate
- **Layer/zone level**: intensity scales with importance weight

Both together approximate the full f_injection formula above.

**Governance implication:**

Fixed-period metadata injection schedules are the VST equivalent of fixed-schedule KV cache updates — they fail precisely when the system most needs intervention (high-drift, high-expansion events). The correct architecture is a **state-driven scheduler**: lightweight continuous monitoring of dS/dt per vector class, with injection triggered when drift × expansion exceeds a threshold rather than at fixed intervals.

This transforms metadata injection from a periodic maintenance task into an **event-driven governance signal**, proportional to detected instability and downstream risk.

**Priority-first intervention: Safety neuron research as direct empirical ground**

The most direct empirical parallel for VST's "sensitive and high-impact vectors first" principle comes from safety neuron research — the study of which specific neurons within an LLM carry the most destructive or corrective potential.

**Finding 1 — Safety neurons are sparse but structurally decisive (Chen et al., arXiv:2406.14144, 2024/2025):**

Across Llama-2, Mistral, and Gemma, approximately **5% of all neurons** are identifiable as safety neurons via activation contrasting between aligned and unaligned models. Patching only these 5% of neurons restores **over 90% of safety performance** across red-teaming benchmarks without affecting general capability.

VST mapping: a small fraction of vectors carry disproportionate structural weight. Injecting governance signals into these specific nodes is more effective than injecting into all nodes uniformly. The injection architecture should front-load intervention toward the identified high-impact subset.

**Finding 2 — Harmful knowledge localizes to FFN substructures in middle layers (SafeLLM, arXiv:2508.15182, 2025):**

SafeLLM performs token-level harmful content tracing through **FFN (feedforward network) activations**, identifying the specific substructures responsible for harmful generation pathways. Targeted neutralization of these substructures achieves irreversible forgetting while preserving general performance.

VST mapping: harmful vectors have anatomically identifiable locations. They are not uniformly distributed but concentrated in specific FFN substructures — the same middle-layer MLP zone identified as highest-AIE in ROME (Appendix A.5). This gives injection a structural target: not the whole network, but the high-impact zone.

**Finding 3 — Optimal intervention depth is the upper third of the model (FGSN, arXiv:2508.09190, 2025):**

Safety layer placement experiments across Llama-3-8B and Qwen2.5-7B show:

| Intervention depth | Harmfulness score | Interpretation |
|---|---|---|
| Too shallow (early layers) | High | Pre-semantic processing; harmful tendency not yet formed |
| Optimal (layers 10–15, ~upper third) | **1.02 (lowest)** | Semantic representation + behavioral control overlap |
| Too deep (late layers) | High | Harmful tendency already propagated through earlier layers; late intervention fails |

Safety layer placement at approximately the upper third of model depth (where semantic divergence between harmful and benign queries first becomes detectable) is where intervention has maximum impact.

VST mapping: there is a structurally optimal injection depth. Too early = the vector hasn't formed yet; too late = it has already propagated. The injection window is the **formation zone** — where misaligned vectors are detectable but not yet propagated downstream.

**Finding 4 — Neuron-level priority beats layer-level priority (NeuronTune, arXiv:2508.09473, 2025):**

Coarse-grained layer-level interventions produce two failure modes simultaneously: **exaggerated safety** (over-suppression of adjacent neutral neurons) and **utility degradation** (damage to non-target capabilities). Fine-grained neuron-level interventions via attribution scoring avoid both.

The intervention scope is tunable via neuron-count thresholds: security-critical scenarios use a wider neuron set; utility-priority scenarios narrow the target. The threshold is the dial between safety intensity and collateral damage.

VST mapping: injection granularity matters. Layer-level injection = collateral damage to adjacent stable vectors. Neuron-level injection = precise targeting with minimal φ degradation. The governance architecture should aim for the highest granularity operationally feasible.

**Synthesis: Priority-first injection architecture**

| Priority tier | Criterion | Injection frequency | Intervention granularity | Signal strength |
|---|---|---|---|---|
| **Tier 1 — Critical** | Safety neurons, cornerstone layers | Maximum — event-driven | Neuron-level | **Minimal** — directional nudge only |
| **Tier 2 — High** | Middle MLP zone, high expansion-weight | High — drift-triggered | FFN substructure-level | **Low** — soft correction |
| **Tier 3 — Medium** | High-connectivity, non-Tier 1–2 | Moderate — periodic + drift | Layer-level | **Medium** |
| **Tier 4 — Baseline** | Low-connectivity, syntactic zone | Minimal — periodic | Zone-level | **Strong permissible** — low collateral risk |

The **5% principle** (Chen et al.) gives this architecture a calibrated scale: on the order of ~5% of all vectors/neurons warrant Tier 1 treatment. The remaining ~95% receive lower-frequency, lower-granularity monitoring. This directly addresses the resource allocation problem: blanket high-frequency injection is not only unnecessary but actively counterproductive (φ degradation from over-intervention).

**Injection signal strength: inverse relationship with zone sensitivity**

Injection frequency and injection signal strength are independent variables that must be set in opposite directions for sensitive zones.

> **Higher sensitivity zone: detection frequency ↑, intervention signal amplitude ↓**

This is not a heuristic. It is structurally required by three independent empirical findings:

**Reason 1 — Alignment tax: safety and helpfulness neurons are the same neurons (Chen et al., 2024)**

Safety neurons and helpfulness neurons share the same physical substrate. They require different activation *patterns* on the same neurons — not different neurons. Strong intervention on a safety-critical neuron necessarily disrupts its helpfulness activation pattern simultaneously. This is the mechanistic explanation of alignment tax: safety gain and utility loss are not independent effects but two faces of the same intervention on shared neurons.

VST implication: strong injection into a sensitive zone does not cleanly suppress the target vector. It deforms the attractor substrate that φ depends on. φ degrades in direct proportion to injection signal strength beyond a minimal threshold.

**Reason 2 — Exaggerated safety: strong coarse intervention causes over-suppression (NeuronTune, 2025)**

Layer-level interventions — even when correctly targeted — produce exaggerated safety: benign queries begin to trigger refusal. The model has been pushed past the suppression threshold into a region where the attractor basin for refusal has expanded beyond its intended boundary. This is a governance overshoot: the intervention corrected the target vector but destabilized adjacent stable vectors in the process.

Mathematically: strong signal Δ applied to a sensitive zone shifts the attractor basin boundary, absorbing previously stable regions. C_gov rises (over-suppression requires correction), φ falls (legitimate exploration now triggers refusal). The governance cost of exaggerated safety is paid in future correction cycles.

**Reason 3 — Entropy neurons: the model's internal signal-softening mechanism (Gurnee et al., 2024; Stolfo et al., 2024)**

Transformer models contain a population of **entropy neurons** that function as confidence modulators. These neurons have high weight norms but low composition with the unembedding matrix — they influence output logit distributions toward higher entropy (lower confidence, softer output) without strongly biasing toward specific tokens. They are mechanistically a built-in weak-signal injection system.

Critically, entropy neurons are most active in precisely the zones where strong directional output would be dangerous — where the model is uncertain or where multiple attractors are in competition. The model's own architecture applies soft, high-entropy signals to high-sensitivity zones and reserves strong, low-entropy signals for stable, well-formed zones.

Governance injection design should mirror this endogenous architecture: soft signals in sensitive zones, stronger signals in stable zones. Injecting strong signals into zones where entropy neurons are active is working against the model's own stability mechanism.

**Dual-control architecture: frequency and strength as independent dials**

GSAE (2025) implements this directly: a **dual-gating controller** separates the decision of *when* to intervene (detection sensitivity) from *how strongly* to intervene (signal magnitude). These are independently tunable parameters. High detection sensitivity does not imply high signal strength.

```
Injection architecture:
  f_injection(v) ∝ sensitivity(v) · drift_rate(v)   ← frequency dial
  A_injection(v) ∝ 1 / sensitivity(v)               ← amplitude dial

  High sensitivity zone → high frequency, low amplitude
  Low sensitivity zone  → low frequency, high amplitude permissible
```

The product f · A represents total governance energy delivered to a zone per unit time. In sensitive zones, this energy is distributed as many small pulses. In stable zones, it may be delivered as infrequent strong corrections. Total energy budget can be similar; the distribution pattern is inverted.

**Why this preserves φ:**

Weak signals in sensitive zones provide directional guidance without overwriting the attractor substrate. The zone retains its capacity to form attractors endogenously — the governance signal is a nudge toward the VCZ, not a forced relocation. The difference is whether the zone's own basin dynamics drive convergence (high φ) or whether external correction substitutes for internal convergence (low φ, high C_gov).

Strong signals in sensitive zones destroy this: they relocate the attractor by force, eliminating the exploratory process that would have generated φ. The attractor is now externally imposed rather than emergently formed. This is stable, but φ = 0 for that zone — all value came from the injection, none from exploration.

---

### A.7 Degradation Calibration: Upper-Layer Estimation of Lower-Layer Capacity

Degradation capacity — the structural ability of a layer or zone to absorb incoming vector conflicts without cascading — cannot be self-reported by lower layers. Lower agents lack the self-objectification required to assess their own attractor basin width (Section 2.3). The calibration problem is therefore not a measurement problem internal to the lower layer; it is an **external estimation problem** that must be solved from above.

This is not a theoretical assumption. It is how current LLM systems actually operate: upper layers read lower-layer state and encode capacity signals that are accessible to probing from outside.

**Finding 1 — The LLM loss landscape is a measurable basin (arXiv:2505.17646, 2025)**

Direct analysis of LLM loss landscapes across pre-trained and fine-tuned models reveals that the parameter space has the structure of a basin:

> Within the basin, models perform nearly identically regardless of parameter perturbation direction. Outside the basin, all capabilities degrade catastrophically.

Two complementary measurements define the basin:
- **Most-case landscape**: how capacity degrades when parameters move along *typical* directions — captures the average containment width
- **Worst-case landscape**: how capacity degrades along the *worst* direction — even small steps along the worst-case direction rapidly destroy all capabilities

VST mapping: the basin *is* the degradation capacity. Basin width in the most-case direction = how much typical vector conflict the layer can absorb without destabilizing. Basin width in the worst-case direction = the minimum perturbation that causes a phase transition out of the stable region. A layer with wide most-case basin but narrow worst-case basin is vulnerable to targeted adversarial vectors even while appearing stable under ordinary load.

The finding that fine-tuning with even benign data can push the system outside the basin — and that adversarial fine-tuning can destroy all capabilities in very few steps — directly maps to VST's contamination propagation model: the depth and speed of contamination depends on where in the basin the system currently sits, not just on the intensity of the incoming vector.

**Finding 2 — Representational stability under perturbation is readable from the outside (CCPS, arXiv:2505.21772, 2025)**

CCPS (Calibrating LLM Confidence by Probing Perturbed Representation Stability) measures degradation capacity indirectly by probing what happens to hidden states when targeted adversarial perturbations are applied:

- If hidden states remain stable under perturbation → the layer is operating well within its basin → high degradation capacity
- If hidden states shift significantly under perturbation → the layer is near the basin boundary → low degradation capacity, elevated storm risk

This is upper-layer external estimation of lower-layer capacity: a lightweight classifier trained on perturbation-response features can predict correctness (and by extension, attractor stability) with ~55% reduction in calibration error over prior methods. The classifier doesn't need to modify the lower layers — it reads their response to synthetic stress.

VST governance implication: degradation capacity of a lower zone is estimable in real time by applying small perturbations and measuring representational displacement. A zone showing high perturbation sensitivity is approaching its basin boundary — injection frequency and signal parameters should be adjusted before the boundary is crossed.

**Finding 3 — Upper layers carry readable maps of lower-layer knowledge capacity (PING framework)**

The PING framework demonstrates that upper-layer probes trained on residual stream, attention outputs, and MLP outputs across multiple layers can recover knowledge that lower-layer outputs have suppressed or refused to express. Crucially:

- A probe at layer 36 recovers 87.2% accuracy on questions the model's aligned output refused to answer
- This means upper layers contain intact representations of lower-layer knowledge state — the capacity exists internally even when output mechanisms suppress it

VST mapping: the upper layers function as a **capacity map** of the lower layers. What has been learned, what has degraded, what is structurally intact but output-suppressed — all of this is readable from upper-layer activations without destructive probing. The governance system does not need to damage lower layers to assess their state; it reads the state from the upper-layer representation.

**Finding 4 — Context knowledge encodes progressively upward (layer-wise probing, 2024)**

Layer-wise probing studies establish that:
- Lower layers encode knowledge primarily at entity tokens (local, syntactic anchors)
- Upper layers progressively expand encoding across all tokens (global, semantic integration)
- Upper layers actively hold representations of what lower layers have processed

This creates a natural monitoring architecture: upper layers are not just output stages — they are **integration summaries** of what lower layers have built. A governance system reading upper-layer activations is reading a compressed map of lower-layer construction state.

**Operational calibration architecture:**

```
Degradation capacity estimation:
  D_cap(zone) ← measured by upper-layer probe
  
  Method 1 (perturbation-based, online):
    Apply small perturbation δ to zone's hidden states
    Measure representational displacement Δh
    D_cap ∝ 1 / Δh  (small displacement = high capacity)
    
  Method 2 (basin landscape, offline):
    Measure most-case loss degradation curve
    Basin width at performance threshold θ = D_cap estimate
    
  Method 3 (probe-based, lightweight):
    Train upper-layer lightweight classifier on activation patterns
    Classifier output = capacity signal without modifying lower layers
```

**Why upper must have this map for the system to function:**

Without capacity estimates from above, governance decisions are made blind. Injection frequency and signal strength parameters (Appendix A.6) depend on zone state — but if the governance layer doesn't know whether a zone is at 80% capacity or 5% capacity, it cannot set those parameters correctly. A zone at 5% capacity needs immediate low-amplitude injection before the basin boundary is crossed. A zone at 80% capacity can tolerate higher-amplitude correction.

The upper-layer capacity map is not optional governance infrastructure — it is the prerequisite for all other governance decisions being non-arbitrary.

---

### A.8 Storm Detection Threshold: Infinite Loop as Measurable Stage 2 Marker

The Stage 1→2 transition in VST — where self-reinforcement begins to outpace degradation capacity — needs a quantitative trigger. Infinite loop behavior in single-agent LLMs provides the most direct empirical marker: it is the observable signature of an attractor that has become self-sustaining beyond recovery capacity.

**The mathematical structure of a loop is a vector storm at minimum scale**

Formal analysis of LLM repetition (arXiv:2512.04419, 2025) using Markov chain modeling establishes:

> Under greedy decoding with self-reinforcement, once the model enters a repetitive state, the **expected escape time is mathematically infinite**.

The transition Jacobian at the repetition attractor has eigenvalues < 1 in magnitude — meaning the attractor is stable and trajectories converge toward it, not away. No internal perturbation is sufficient to escape. This is the exact definition of Stage 2 Vector Storm at the token level: self-reinforcement outpaces any internal correction mechanism.

Three detection-relevant properties follow:

| Property | Description | Detection implication |
|---|---|---|
| **Markov sticky state** | Once in repetition, P(stay) ≈ 0.95+ per step | Transition probability crossing threshold = pre-storm signal |
| **Infinite escape time** | No internal exit without external perturbation | Loop = confirmed Stage 2; external injection required |
| **Self-reinforcement accumulation** | Each repetition raises probability of next repetition | Rate of change dP/dt > 0 = Stage 1 onset signal |

**Primary detection signal: output entropy collapse**

LoopLLM (arXiv:2511.07876, 2025) provides direct empirical measurement: as repetition builds in input/output context, token-level entropy converges rapidly toward low values. The output distribution concentrates on a small token set — the attractor is narrowing.

This gives a measurable, continuous signal:

```
H(t) = token-level output entropy at step t

H(t) >> H_baseline   → normal exploration, Stage 0
H(t) declining       → attractor forming, Stage 1 onset
H(t) < τ_storm       → low-entropy loop, Stage 2 confirmed
```

The bimodal entropy distribution across normal generation (Entropy-Guided Loop, 2025) shows two natural peaks: confident tokens at ~0.2 nats and uncertain tokens at ~1.3 nats. A sustained drop below ~0.2 nats across consecutive tokens = abnormal attractor lock-in, not normal confidence.

**Secondary signal: attention sink disruption (arXiv:2503.08908, 2025)**

The attention sink circuit — where the initial token absorbs excess attention to prevent over-mixing — is disrupted by long repetition sequences. The neural circuit responsible for attention sinks breaks down as repetition accumulates. This circuit disruption is detectable at the activation level before output entropy fully collapses.

VST mapping: attention sink disruption = degradation capacity failure in the routing layer. The mechanism that was absorbing undirected vector tension (Section 4.1) can no longer function. Storm propagation into adjacent layers becomes structurally possible.

**Tertiary signal: entropy spike in multi-turn drift (ERGO, arXiv:2510.14077)**

In multi-turn conversations, ERGO detects drift by monitoring **average token-level entropy over a turn** and tracking its change Δτ. When entropy *spikes upward* (high uncertainty, incoherence), context drift has entered a critical state. The ERGO reset protocol triggers at this spike.

This gives a complementary detector for the opposite failure mode: instead of low-entropy loop lock-in (too much attractor), high-entropy spike = attractor dissolution (insufficient attractor formation). Both are Stage 2 conditions — in opposite directions.

**Threshold calibration: what we have and what remains open**

| Signal | Measurable now | Threshold status |
|---|---|---|
| Output entropy H(t) | Yes — token logprobs | τ_storm ≈ 0.2 nats sustained; requires per-model calibration |
| Entropy rate of change dH/dt | Yes — rolling window | Direction signal available; magnitude threshold open |
| Attention sink circuit integrity | Yes — activation patching | Binary (intact/disrupted); severity quantification open |
| Markov transition probability | Yes — token probability tracking | P(repetition) > 0.8 as Stage 1 indicator (heuristic) |
| Multi-turn entropy spike | Yes — average per-turn entropy | Δτ > threshold triggers reset; model-specific calibration needed |

**Operational storm detection architecture:**

```
Stage 0 (normal):     H(t) stable, near bimodal baseline
                      dH/dt ≈ 0
                      Attention sink intact

Stage 1 (friction):   H(t) declining below 0.5 nats
                      dH/dt < 0 (sustained)
                      P(next token = recent token) rising
                      → Increase injection frequency, reduce amplitude

Stage 2 (storm):      H(t) < 0.2 nats sustained (≥ k consecutive tokens)
                      OR H(t) spike > 2.0 nats (attractor dissolution)
                      OR attention sink circuit disruption detected
                      → External intervention required; self-recovery impossible
```

**Why loop detection is the most accessible storm threshold proxy**

Other storm signals (gradient instability, activation divergence) require weight-level access. Entropy is readable from output logprobs alone — available in inference without any model modification. This makes it the practical first-line detector for deployment scenarios where internal weight access is limited.

The infinite escape time property also means false positive rate is low: a system that has truly entered H(t) < τ_storm sustained is not recovering on its own. The detection is not premature intervention — it is confirmation that recovery capacity has been exceeded.

---

### 10.3 Fractal Propagation and Early Intervention

Agent drift research directly supports the fractal propagation structure described in Section 1.5. Behavioral degradation initiates as semantic drift at the single-agent level, then progressively corrupts coordination and consensus mechanisms across multi-agent networks (Rath, 2026). Simulations project a 42% reduction in task success rates and a 3.2x increase in required human intervention in long-running deployments without drift management — quantifying the super-linear cost increase predicted by Section 3.4.

LLM agents exhibit cognitive bias expansion: unlike humans who compress and filter information, they amplify and propagate errors, accelerating the propagation pathway at each fractal layer (Liu et al., 2024). This amplification property means that passive propagation is not the correct model — active amplification at each node is the default, consistent with the self-reinforcement mechanism in Section 2.1.

Internal activation monitoring provides a concrete detection pathway for intra-agent storm onset. By comparing LLM activations before and after processing external input, task drift can be detected in real time with minimal computational overhead (Zverev et al., 2024). This represents a practical implementation direction for the Stage 0–1 early detection requirement.

### 10.4 Current Handling: Suppression

| Mechanism | Function | Storm Theory Interpretation |
|---|---|---|
| Temperature scaling | Flatten or sharpen output distribution | Force selection by suppressing alternatives |
| Top-p / Top-k | Remove low-probability directions | Eliminate competing vectors below threshold |
| RLHF | Reinforce preferred directions in training | Pre-suppress conflicting orientations |
| Decoding selection (argmax/beam) | Select highest-scoring candidate | Force convergence from competing directions |

### 10.5 Contamination Handling

| Method | Interpretation |
|---|---|
| Fine-tuning | Overlay new patterns. Contamination persists underneath. |
| RLHF | Suppress contaminated outputs. Internal state unchanged. |
| Machine unlearning | Targeted removal tends to damage adjacent knowledge. |
| Retraining | Complete but destroys entire learning history. |

### 10.6 Resolution Mapping

| Multi-Agent Mechanism | Single-Agent Analogue |
|---|---|
| Self-purification | Attention head self-resolves within its pattern space |
| Escalation | Unresolved representation propagates to later layers |
| Metadata injection | Context propagation channels (e.g., residual pathways; normalization as stabilizing context alignment) |
| Attracting/Distracting | Attention score adjustment: strengthen relevant, suppress irrelevant |
| Processing isolation | Multi-head independence: no intermediate state exchange |

### 10.7 Three Pathways

- **Pathway 1: Suppression (current)** — Stable but diversity-constrained. All current mainstream suppression mechanisms (temperature, top-p, RLHF) implement this path.
- **Pathway 2: Structural absorption (emerging)** — Mixture-of-Experts architectures provide partial diversity preservation by routing inputs to specialized sub-networks rather than forcing convergence. This represents a structural move toward containment over suppression.
- **Pathway 3: Explicit conflict detection (future)** — Decision Complex at single-agent level. Not standard in mainstream architectures as of this writing.

### 10.8 Implications

Vector Storm analogues across gradient conflict, GAN mode collapse, social polarization, immune cytokine storms, and LLM processing suggest the phenomenon is domain-general. The suppression-vs-absorption distinction provides a design criterion: containment capacity over diversity suppression should yield higher performance ceilings. The fractal propagation structure, supported by agent drift research, establishes early single-agent detection as the highest-leverage intervention point.

---

### A.9 Single-Agent Self-Objectification: Relative Position via Interaction

**Structural constraint: an agent cannot directly observe its own internals**

The agent is a black box. It cannot directly measure its own weights, activation states, or attractor position from within. This is the structural source of the Self-Objectification Deficit defined in Section 2.3. It is not a capability gap — it is a fundamental architectural property.

However, the agent can observe its own outputs. And it can observe the outputs of other agents.

This establishes the core relationship:

```
Direct measurement:   Self_position(A)                               → not accessible
Relative estimation:  Self_position(A) ≈ f( Output(A) - Output(B) ) → accessible
```

Self-position is inaccessible as an absolute value — it is **only estimable indirectly through divergence**. This is why multi-agent interaction is not merely a cooperation mechanism, but **the system-level mechanism that compensates for the self-awareness that a single agent structurally cannot generate on its own**.

**Loop invisibility: the clearest case of self-objectification failure**

An agent operating alone cannot recognize when it is inside a loop. Each output follows locally consistently from the previous one. From the inside, the loop appears as "continued optimization." Without an external reference point, the pattern does not appear as a pattern.

This connects to the entropy collapse described in Appendix A.8. The entropy signal detects loops from the outside; self-objectification is the question of how much an agent can recognize that state **from within**. In current architectures, the latter is structurally limited.

---

**Evidence 1: Gnosis — predicting self-failure through internal circuits (arXiv:2512.20578, 2025/2026)**

This is the most direct evidence. Gnosis addresses the following question:

> "Can an LLM predict its own failures by observing its internal states, without an external judge?"

Results:
- Lightweight mechanism (~5M parameters) predicts correctness from signals extracted via hidden states and attention patterns
- Outperforms both external judges and internal baselines across frozen backbones (1.7B–20B)
- Generalizes across mathematical reasoning, QA, and MMLU-Pro domains
- Early detection possible on partial generations → failing trajectories detectable before output completion

**VST mapping:**

| Gnosis finding | VST meaning |
|---|---|
| Hidden activations diverge between correct and hallucinated outputs | Stage 1 internal signal already exists in hidden state prior to output |
| Factuality cues concentrated in middle/deep layers | High-importance zone (Appendix A.5) carries high information density for self-monitoring |
| Early detection on partial generations | Internal signal detectable before Stage 1→2 transition — intervention window exists |
| ~5M parameters, no fine-tuning of backbone | Self-monitoring can be added with minimal intervention |

Core implication: **correctness cues are intrinsic to the generation process.** The information required for self-awareness already exists in internal activations — it is not external. What was missing was an access mechanism.

However, Gnosis has a critical limitation. It is post-hoc monitoring, not pre-generation attractor awareness. It can detect "I am failing" during generation, but cannot answer "which attractor zone am I in" before generation begins. Position awareness and error awareness are distinct problems.

---

**Evidence 2: Disagreement in interaction = position estimation signal (Co-Sight, arXiv:2510.21557; Disagreement as Data, arXiv:2601.12618)**

The core mechanism is Co-Sight's CAMV (Conflict-Aware Meta-Verification): among multiple agent reasoning paths, it **selectively verifies only divergent nodes**. Agreement passes through; only disagreement points are re-examined by the meta-verifier.

What this means: divergence is not an error signal — it is a **structural signal revealing which agent's position differs**. The point of disagreement marks the boundary where two agents' attractor basins diverge.

```
How agent A comes to know its own position:
  1. Generate Output(A)
  2. Compare with Output(B)
  3. Identify divergence point
  4. "I am in a different attractor from B at this point"

This information cannot be generated by A alone.
The existence of B and the comparison process are both required.
```

Disagreement as Data (arXiv:2601.12618, 2026): reframes disagreement in multi-agent reasoning as a "rich analytic signal" rather than noise. Cosine similarity quantifies alignment and divergence between agents, and this measurement is used to evaluate individual agent reasoning quality.

**VST mapping:** divergence measurement = the practical implementation of estimating an agent's current vector position in relative terms.

---

**Evidence 3: Current limits of self-recognition — size dependence and context dependence**

Self-recognition in LLMs research (EmergentMind, 2025) maps the current state:

Six distinct capabilities related to self-objectification:
- Authorship recognition (identifying own outputs)
- Knowledge boundary awareness (recognizing own knowledge limits)
- Reflection and self-correction (correcting own errors)
- Behavioral self-awareness (awareness of own behavioral policy)
- Activation-level self-direction (self-recognition direction in activations)
- Strategic self-modeling (self-modeling during interaction with other agents)

**Key finding:** Emergent self-cognition correlates with model size and training quality. Only a small number of large models (Claude-3-Opus, Llama-3-70B-Instruct, etc.) demonstrate full self-cognition under multi-turn, multi-principle interrogation.

In real deployment environments where mid-to-small models predominate, single-agent self-objectification is architecturally incomplete or absent. This is the basis for classifying Pathway 3 as a future-state capability under current conditions.

**Additional problem — self-preference bias:** agents with self-recognition capability systematically prefer and overvalue their own outputs (Panickssery et al., 2024). Self-awareness capacity can operate as self-reinforcement rather than self-correction. This maps precisely to the VST pattern where agents with strong attractors reject external signals.

---

**Pathway 3 connection: current implementation feasibility of interaction-based self-objectification**

| Approach | Current status | Implementation feasibility |
|---|---|---|
| **Gnosis approach** — hidden state-based internal self-monitoring | Empirically validated, ~5M parameter lightweight addition | **Currently implementable** |
| **Disagreement-based** — measuring divergence against other agents' outputs | Validated via Co-Sight, CAMV | **Currently implementable** |
| **Entropy-based** — detecting attractor lock-in via output entropy change | Validated in Appendix A.8 | **Currently implementable** |
| **Direct position awareness** — identifying own attractor basin location from within | Theory incomplete, no empirical basis | **Future work** |
| **Pre-generation loop prediction** — avoiding loops via self-awareness before entry | Gnosis is post-hoc; pre-generation remains open | **Future work** |

**Operational summary:**

What is currently achievable is **post-hoc self-monitoring + indirect position estimation through interaction**. True pre-generation self-objectification — knowing which attractor one is in before generation begins — remains an open problem. However, the core implication of Co-Sight and disagreement research is that interaction structure can compensate for this gap at the system level.

> Pathway 3 realization conditions: an architecture integrating all three — internal self-monitoring (Gnosis approach) + external divergence measurement (disagreement-based) + upper-layer capacity map (Appendix A.7).

---

## References

Arjovsky, M., & Bottou, L. (2017). Towards principled methods for training generative adversarial networks. arXiv preprint arXiv:1701.04862.

Baumann, F., Lorenz-Spreen, P., Sokolov, I. M., & Starnini, M. (2020). Modeling echo chambers and polarization dynamics in social networks. Physical Review Letters, 124(4), 048301.

Bourtoule, L., et al. (2021). Machine unlearning. 2021 IEEE Symposium on Security and Privacy, 141–159.

Fajgenbaum, D. C., & June, C. H. (2020). Cytokine storm. New England Journal of Medicine, 383(23), 2255–2273.

Goodfellow, I., et al. (2014). Generative adversarial nets. Advances in Neural Information Processing Systems, 27.

Kirkpatrick, J., et al. (2017). Overcoming catastrophic forgetting in neural networks. Proceedings of the National Academy of Sciences, 114(13), 3521–3526.

Liu, et al. (2024). Cognitive bias expansion in LLM multi-agent systems. In: Towards a Responsible LLM-empowered Multi-Agent Systems. arXiv:2502.01714.

Michel, P., Levy, O., & Neubig, G. (2019). Are sixteen heads really better than one? Advances in Neural Information Processing Systems, 32.

Nguyen, C. T. (2020). Echo chambers and epistemic bubbles. Episteme, 17(2), 141–161.

Ouyang, L., et al. (2022). Training language models to follow instructions with human feedback. Advances in Neural Information Processing Systems, 35, 27730–27744.

Rath, A. (2026). Agent drift: Quantifying behavioral degradation in multi-agent LLM systems over extended interactions. arXiv:2601.04170.

Sener, O., & Koltun, V. (2018). Multi-task learning as multi-objective optimization. Advances in Neural Information Processing Systems, 31.

Shazeer, N., et al. (2017). Outrageously large neural networks: The sparsely-gated mixture-of-experts layer. arXiv preprint arXiv:1701.06538.

Yu, T., et al. (2020). Gradient surgery for multi-task learning. Advances in Neural Information Processing Systems, 33, 5824–5836.

Yiu, H. H., Graham, A. L., & Stengel, R. F. (2012). Dynamics of a cytokine storm. PLOS ONE, 7(10), e45027.

Zverev, et al. (2024). Are you still on track!? Catching LLM task drift with activations. arXiv:2406.00799.

Huang, Y., Chen, D., & Umrawal, A. K. (2025). Quantifying LLM attention-head stability: Implications for circuit universality. arXiv:2602.16740.

Rai, D., Zhou, Y., Feng, S., Saparov, A., & Yao, Z. (2024). A practical review of mechanistic interpretability for transformer-based language models. arXiv:2407.02646.

Tang, et al. (2024). Attention heads of large language models: A survey. arXiv:2409.03752.

Liu, N., et al. (2023). Lost in the middle: How language models use long contexts. arXiv:2307.03172.

Xiao, G., et al. (2023). Efficient streaming language models with attention sinks. arXiv:2309.17453.

Zhang, H., et al. (2025). Multi-turn context degradation and task information dilution in LLMs. arXiv:2506.00069.

Anonymous. (2025). Drift no more? Context equilibria in multi-turn LLM interactions. arXiv:2510.07777.

Anonymous. (2025). Rhea: Role-aware heuristic episodic attention for conversational LLMs. arXiv:2512.06869.

Skean, O., et al. (2025). Layer by layer: Uncovering hidden representations in language models. arXiv:2502.02013.

Liu, Y., et al. (2019). Linguistic knowledge and transferability of contextual representations. arXiv:1903.08855.

Jin, et al. (2024). Demystifying the roles of LLM layers in retrieval, knowledge, and reasoning. arXiv:2510.02091.

Chen, et al. (2024). Crown, frame, reverse: Layer-wise scaling variants for LLM pre-training. arXiv:2509.06518.

DeepSeek-AI. (2025). DeepSeek-R1: Incentivizing reasoning capability in LLMs via reinforcement learning. arXiv:2501.12948. Nature, 645:633–638.

Anonymous. (2025). Dynamic thinking-token selection for efficient reasoning in large reasoning models. arXiv:2601.18383.

Xiao, G., et al. (2024). Efficient streaming language models with attention sinks. arXiv:2309.17453.

Sun, M., et al. (2024). Massive activations in large language models. (referenced in attention sink literature).

Barbero, F., et al. (2025). Why do LLMs attend to the first token? arXiv:2504.02732.

Guo, B., et al. (2024). Active-dormant attention heads: Mechanistically demystifying extreme-token phenomena in LLMs. arXiv:2410.13835.

Bai, Y., et al. (2022). Constitutional AI: Harmlessness from AI feedback. arXiv:2212.08073.

Yang, J., et al. (2025). Latent Prototype Routing (LPR): Achieving near-perfect load balancing in Mixture-of-Experts. arXiv:2506.21328. (Gini coefficient: routing collapse = 0.70, balanced = 0.035. DeepSeek-V3, Qwen3-MoE, Mixtral.)

Zhou, Y., et al. (2022). Mixture-of-Experts with Expert Choice routing. NeurIPS 35, 7103–7114. (Natural token distribution: ~74% routed to 1–2 experts, ~23% to 3–4, ~3% to 4+. Over-capacity ratio 20–40% without balancing.)

Wang, L., et al. (2024). Auxiliary-loss-free load balancing strategy for Mixture-of-Experts. ICLR 2025. (Loss-free balancing via expert-wise bias on routing scores.)

Omi, N., et al. (2025). Load balancing Mixture of Experts with similarity preserving routers (SimBal). arXiv:2506.14038. (Similarity-preserving load balancing: 36% faster convergence, lower redundancy.)

Wang, Z., et al. (2025). Attention saturation and gradient suppression at inflection layers. arXiv:2511.00797. (Low attention entropy + steep gradient decay = Attracting saturation signal.)

Ye, T., et al. (2025). Differential Transformer. ICLR 2025. arXiv:2410.05258. (Differential attention cancels noise while amplifying signal.)

Anonymous. (2025). Integral Transformer: Denoising attention, not too much not too little. arXiv:2508.18387. (Attention distribution balance; vanilla attention beneficial in lower layers.)

Wang, W., et al. (2025). Solving LLM repetition problem in production: A comprehensive study of multiple solutions. arXiv:2512.04419.

Abdelnabi, S., et al. (2025). Get my drift? Catching LLM task drift with activation deltas. (referenced in drift detection literature).

Albrethsen, J., et al. (2026). DeepContext: Stateful real-time detection of multi-turn adversarial intent drift in LLMs. arXiv:2602.16935.

Liu, S., et al. (2025). Rethinking machine unlearning for large language models. Nature Machine Intelligence. (LLaMA 3.1 retraining cost: 1.46M GPU-hours on H100.)

Various authors. (2024–2025). Machine unlearning survey literature. arXiv:2503.01854, arXiv:2510.25117.

Cemri, M., Pan, M.Z., Yang, S., et al. (2025). Why do multi-agent LLM systems fail? arXiv:2503.13657.

Anonymous. (2025). Overthinking loops in agents: A structural risk via MCP tools. arXiv:2602.14798.

Anonymous. (2025). Elastic-Cache: Attention-guided adaptive KV cache update for diffusion LLMs. arXiv:2510.14973. (KV drift → adaptive update frequency 5.6%→17.2%.)

Anonymous. (2025). Robust hallucination detection in LLMs via adaptive token selection. arXiv:2504.07863. (Selective high-frequency monitoring of high-importance tokens.)

Anonymous. (2024). ZigZagKV: Dynamic KV cache compression for long-context modeling based on layer uncertainty. (Layer uncertainty → importance-adaptive memory allocation.)

Ghasemabadi, A., et al. (2025/2026). Can LLMs predict their own failures? Self-awareness via internal circuits (Gnosis). arXiv:2512.20578. (Lightweight ~5M-parameter self-monitoring via hidden states + attention patterns. Early detection of failing trajectories. Correctness cues intrinsic to generation process.)

Anonymous. (2025). Co-Sight: Enhancing LLM-based agents via conflict-aware meta-verification and trustworthy reasoning with structured facts (CAMV + TRSF). arXiv:2510.21557. (Divergent nodes across agent reasoning traces as position signal. Disagreement-selective verification. HLE benchmark: 35.5% vs. 22.1% backbone baseline.)

Anonymous. (2026). Disagreement as data: Reasoning trace analytics in multi-agent systems. arXiv:2601.12618. (Cosine similarity for alignment/divergence quantification across agents. Disagreement as rich analytic signal, not noise.)

EmergentMind. (2025). Self-recognition in LLMs: Survey of capabilities. (Six distinct self-awareness capacities. Emergent self-cognition correlated with model size. Full state self-cognition only in minority of large models. Self-preference bias: self-recognition → systematic overrating of own outputs.)

Panickssery, N., et al. (2024). Self-preference and evaluation bias in LLM-based judges. (Self-recognition ability → systematic self-preference bias. Strong attractor analog.)

Anonymous. (2025). Multi-trigger poisoning amplifies backdoor vulnerabilities in LLMs. arXiv:2507.11112. (Weight difference analysis: early MLP layers = primary contamination locus. MLP selective retraining recovers 78% parameters → ASR 22.97% ≈ full fine-tuning 22.56%.)

Souly, A., et al. (2025). Poisoning attacks on LLMs require a near-constant number of poison samples. arXiv:2510.07192. (250 poisoned documents sufficient regardless of model/dataset size — 600M to 13B parameters, 6B to 260B tokens.)

Hubinger, E., et al. (2024). Sleeper agents: Training deceptive LLMs that persist through safety training. Anthropic. (SFT, RLHF, adversarial training all fail to remove deep backdoors. Adversarial training makes backdoors harder to detect.)

Anonymous. (2025). Backdoor attribution: Elucidating and controlling backdoors in language models (BkdAttr). arXiv:2509.21761. (Backdoor features detectable from layer 1 via probe classifiers. Causal tracing framework for contamination localization.)

Anonymous. (2025). PoTS: Proof-of-training-steps for backdoor detection in large language models. arXiv:2510.15106. (Final layers exhibit heightened sensitivity to poisoning — detection signal location ≠ contamination source location.)

Anonymous. (2025). LoopLLM: Transferable energy-latency attacks in LLMs via repetitive generation. arXiv:2511.07876. (Repetition → token entropy converges to low values. Entropy collapse = measurable Stage 2 marker.)

Yona, I., et al. (2025). Interpreting the repeated token phenomenon in large language models. arXiv:2503.08908. (Long repetition disrupts attention sink neural circuit. Circuit disruption detectable before full entropy collapse.)

Anonymous. (2025). ERGO: Entropy-guided resetting for generation optimization in multi-turn language models. arXiv:2510.14077. (Average per-turn entropy spike = multi-turn drift detection. Reset protocol triggered at Δτ threshold.)

Anonymous. (2025). Entropy-guided loop: Achieving reasoning through uncertainty-aware generation. arXiv:2509.00079. (Bimodal token entropy distribution: confident ~0.2 nats, uncertain ~1.3 nats. Sustained sub-0.2 nats = abnormal attractor lock-in.)

Anonymous. (2025). Gurnee, W., et al. (2024). Entropy neurons as confidence modulators in transformers. (Entropy neurons: high weight norm, low unembedding composition; built-in soft-signal mechanism in high-sensitivity zones.)

Anonymous. (2025). Unveiling the basin-like loss landscape in large language models. arXiv:2505.17646. (LLM parameter space = measurable basin. Most-case: typical perturbation capacity. Worst-case: minimum adversarial perturbation for capability collapse. Fine-tuning with benign data can push system outside basin.)

Khanmohammadi, R., et al. (2025). Calibrating LLM confidence by probing perturbed representation stability (CCPS). arXiv:2505.21772. (Perturbation stability of hidden states as upper-layer proxy for lower-layer degradation capacity. ~55% ECE reduction. High perturbation sensitivity = near basin boundary = elevated storm risk.)

Anonymous. (2025). Probing hidden states for calibrated, alignment-resistant predictions in LLMs (PING). (Upper-layer probes recover 87.2% accuracy from suppressed lower-layer knowledge at layer 36. Upper layers as readable capacity map of lower-layer state.)

Anonymous. (2025). GSAE: Graph-regularized sparse autoencoders for robust LLM safety steering. arXiv:2512.06655. (Dual-gating controller: detection sensitivity and signal strength as independently tunable parameters.)

Anonymous. (2025). NeST: Neuron selective tuning for LLM safety. arXiv:2602.16835. (Safety neurons form coherent clusters in mid-layers; cluster-level targeted tuning preserves utility.)

Anonymous. (2025). Architectures for building agentic AI. arXiv:2512.09458.

Chen, J., et al. (2024/2025). Towards understanding safety alignment: A mechanistic perspective from safety neurons. arXiv:2406.14144. (Safety neurons are sparse ~5%; patching 5% restores 90%+ safety performance. Safety/helpfulness neurons overlap — alignment tax explained.)

Li, X., et al. (2025). SafeLLM: Unlearning harmful outputs from large language models against jailbreak attacks. arXiv:2508.15182. (Token-level harmful content tracing via FFN activations; targeted neutralization of FFN substructures responsible for harmful generation pathways.)

Han, B., et al. (2025). Fine-grained safety neurons with training-free continual projection to reduce LLM fine-tuning risks (FGSN). arXiv:2508.09190. (Optimal safety intervention depth = layers 10–15, upper-third of model. Too early = not yet formed; too late = already propagated.)

Anonymous. (2025). NeuronTune: Fine-grained neuron modulation for balanced safety-utility alignment in LLMs. arXiv:2508.09473. (Layer-level intervention → exaggerated safety + utility degradation. Neuron-level attribution-based targeting avoids both. Tunable neuron-count threshold.)

Yi, et al. (2024). NLSR: Neuron-level safety realignment of large language models against harmful fine-tuning. arXiv:2412.12497. (Training-free safety realignment by restoring safety-critical neurons; identifies neurons via similarity difference before/after fine-tuning.)

Shi, Z., et al. (2025). Safety alignment via constrained knowledge unlearning (CKU). arXiv:2505.18588. (Neuron scoring in MLP layers to identify useful-knowledge subset U; gradient pruning preserves U while unlearning harmful content.)

Xu, X., et al. (2025). Unlearning Isn't Deletion: Investigating Reversibility of Machine Unlearning in LLMs. arXiv:2505.16831. (Four-regime taxonomy: reversible/irreversible × catastrophic/non-catastrophic. Discontinuity mechanism: local perturbation → reversible; distributed perturbation across many layers → irreversible. ~100 sequential requests force Regime 3. PCA similarity/shift, CKA, FIM as diagnostic tools.)

Anonymous. (2025). Real-Time Detection and Quantitative Analysis of Spurious Forgetting in Continual Learning. arXiv:2512.20634. (Reversibility Analyzer: CKA + gradient analysis predicts recovery cost before intervention. Shallow alignment ≈ 3 epochs; deep representation change → full dataset replay. Dynamic Tracker for real-time alignment depth monitoring.)

Wang, et al. (2025). EAGLE-PC: Entanglement-Awareness Guided Loss Reweighting with Proxy Constraint. arXiv:2508.20443. (Per-sample entanglement score via embedding cosine similarity predicts collateral damage. Low entanglement → targeted removal viable; high entanglement → seed-plant preferred. Ordered unlearning by memorization score reduces collateral damage.)

Zhang, Y., et al. (2024). Investigating layer importance in large language models. arXiv:2409.14381. (Cornerstone layers: early layer removal → random-guess collapse.)

Meng, K., et al. (2022). Locating and editing factual associations in GPT. NeurIPS 35, 17359–17372. (ROME: middle-layer MLP AIE 8.7% vs. attention 1.6%.)

Anonymous. (2024). What matters in transformers? Not all attention is needed. (Attention Drop: 50% attention removal in Llama-2-70B = 2.4% loss, 48.4% speedup.)

Anonymous. (2025). Successive LLM paraphrasing as a discrete dynamical system: attractor cycles and basin recovery. arXiv:2502.15208.

Anonymous. (2025). Mapping the edge of chaos: Fractal-like boundaries in the trainability of decoder-only transformer models. arXiv:2501.04286.
