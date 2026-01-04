
{% raw %}
<!-- Drop this anywhere in your README.md or page HTML -->
<script>
  window.MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$','$$'], ['\\[','\\]']],
      processEscapes: true
    },
    options: {
      skipHtmlTags: ['script','noscript','style','textarea','pre','code']
    }
  };
</script>
<script id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>
{% endraw %}  

**Ukubona LLC** is an identity infrastructure company.

We model the human subject as a **trajectory**, not a profile.

Our core insight is that identity is not declared, authenticated, or narrated—it is **integrated**.

---

### Neurocomputational Stack (A Priori → Audit)

* **[Corticothalamic](https://ukb-dt.github.io/mcgilchrist-00/) (A Priori)**
  The routing layer. What *can* be perceived, acted upon, or even rendered computable.

* **[Thalamus](https://ukb-dt.github.io/mcgilchrist-XX/) (Body / Claim / Audit)**
  The claim surface. Signals enter here as embodied assertions requiring routing, not belief.

* **[Prefrontal Cortex](https://ukb-dt.github.io/mcgilchrist-YY/) (Mind / Validate)**
  [Constraint satisfaction](https://ukb-dt.github.io/dt/). Local coherence, decision validation, and executive gating.

* **[Default Mode Network](https://ukb-dt.github.io/mcgilchrist-ZZ/) (Invariant / Rigor / Adversarial)**    
  The adversary. Identity stress-testing, counterfactuals, and invariance detection.

* **Hippocampus (Credibility / Path-Dependence / Longitudinal UX)**
  Memory as proof. Credibility emerges only through time, sequence, and consequence.

---

### Product Stack (Landscape → UX)

* **LS — Landscape**
  The environment of affordances and constraints. What gradients exist.

* **UB — User Behavior + Loss**
  Perturbation. Every action updates the loss surface.

* **SGD — Stochastic Gradient Descent**
  Both literal and lived. Learning occurs through noisy, embodied updates.

* **UI — Curvature**
  Second derivatives must exist and be non-zero.
  Health, motion, sleep, stress: trajectories, not metrics.

* **UX — Integral**
  Ethics, aesthetics, and computation ([*posteriori*](https://en.wikipedia.org/wiki/Bayesian_statistics)) converge as accumulated activity.
  Power → energy. Steps → distance. Time → credibility.

---

### The API Thesis

Ukubona develops **authorization-first APIs** that allow individuals to:

* Bind embodied data streams (e.g. Apple Watch, HealthKit, sensors)
* To a **digital twin that exists a priori**
* Which is *updated*, not rewritten
* And remains identity **only insofar as it remains faithful to embodiment**

Passcodes authorize access.
Time authorizes truth.

Identity is not stored.
It is **re-derived**.

---

Ukubona does not ask *who are you?*
It asks:

**What curvature have you sustained?**
**What trajectories can be audited?**
**What invariants survived perturbation?**

---

Here is a clean Bayesian formalization that fits your stack and keeps **ethics, aesthetics, and computation** as *posteriori* quantities emerging from lived data (trajectory), not priors.

---

### 1. Posterior over integrated judgment

Let

* (E) = Ethics
* (A) = Aesthetics
* (C) = Computation
* $\mathcal{T}$ = embodied trajectory (actions, consequences, time)

Then the joint *posteriori* is

$$
P(E, A, C \mid \mathcal{T})
\propto
P(\mathcal{T} \mid E, A, C); P(E, A, C)
$$

Interpretation:

* **Likelihood** $P(\mathcal{T} \mid E, A, C)$:
  How well a candidate ethical–aesthetic–computational configuration *explains the observed life path*.
* **Prior** $P(E, A, C)$:
  Structural constraints (biology, culture, architecture), not moral declarations.

---

### 2. Factorization aligned with your stack

A natural conditional ordering (not independence):

$$
P(E, A, C \mid \mathcal{T})
\propto
P(\mathcal{T} \mid C, A, E)
P(C \mid A, E)
P(A \mid E)
P(E)
$$

**Reading downward:**

* $P(\mathcal{T} \mid C, A, E)$
  → Does the lived trajectory *execute*?
* $P(C \mid A, E)$
  → Computation is constrained by form and value.
* $P(A \mid E)$
  → Aesthetics emerges from ethical constraint.
* $P(E)$
  → Sparse, weak, often wrong a priori.

---

### 3. Longitudinal update (credibility over time)

For sequential time $t = 1 \dots T$:

$$
P(E, A, C \mid \mathcal{T}*{1:T})
\propto
\prod*{t=1}^{T}
P(\tau_t \mid E, A, C)
P(E, A, C)
$$

This encodes your dictum:

$$
\textbf{Time authorizes truth.}
$$

No single action validates ethics.
Only accumulated likelihood does.

---

### 4. Collapse to UX (your integral)

If UX is the observable scalar summary:

$$
\text{UX} = \int_{\mathcal{T}} f(E, A, C)\, dt
$$

then inference runs *backwards*:

$$
P(E, A, C \mid \text{UX})
\propto
P(\text{UX} \mid E, A, C) P(E, A, C)
$$

Ethics is not asserted.
Aesthetics is not styled.
Computation is not optimized.

They are **inferred**.

---

If you want, next we can:

* enforce **curvature** explicitly via second derivatives in the likelihood, or
* map this directly onto **DMN as adversarial prior stress-testing**, or
* collapse (E, A, C) into an invariant manifold and show when identity fails.
