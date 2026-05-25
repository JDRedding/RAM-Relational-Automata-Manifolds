# RAM : Relational Automata Manifolds
## RDG–MFE–Q: Generalized Cellular Automata  
*A strict extension of Conway’s Life, Wolfram CA, graph CA, asynchronous CA, and constrained CA*

This repository contains the theory, proofs, demos, and minimal Python implementations showing how **RDG–MFE–Q** strictly generalizes classical cellular automata by adding:

- **RDG** — generative relational geometry  
- **MFE** — field‑based dynamics (Life-like, Maxwell-like, PDE-like)  
- **Q** — admissibility, SID stability, quotienting  

Classic CA appear as the degenerate case:

```
CA ≃ (Γ_fixed grid, f_lookup table, Q_∅)
```

RDG–MFE–Q provides geometry, dynamics, and admissibility as *separate, composable layers*.

---

## Repository Structure

```
CA-Extensions-RDG-MFE-Q/
│
├── README.md
│   ├── Overview
│   ├── Classic CA → RDG–MFE–Q reduction
│   ├── Why RDG–MFE–Q strictly generalizes CA
│   ├── Glider embedding theorem
│   ├── Emergent geometry demo
│   └── Maxwell–Quaternion appendix
│
├── theory/
│   ├── RDG-MFE-Q_CA_Generalization.md
│   ├── Universality_Theorem.md
│   ├── Emergent_Manifolds.md
│   └── Maxwell_Quaternion_Appendix.md
│
├── code/
│   ├── rdg_mfe_q_minimal.py
│   ├── rdg_mfe_q_life_exact.py
│   ├── rdg_mfe_q_glider_preserved.py
│   └── utils.py
│
├── examples/
│   ├── glider_exact/
│   ├── glider_preserved/
│   └── emergent_grid/
│
└── LICENSE
```

---

## Suggested README.md Outline

````markdown
# RDG–MFE–Q: Generalized Cellular Automata

RDG–MFE–Q is a **three‑layer generalization** of classical cellular automata:

- **RDG** — Relational Dynamic Geometry  
- **MFE** — Momentum‑Flux Engine (field dynamics)  
- **Q** — Quotient / Admissibility (SID stability)

Classic CA (Life, Rule 110, Wolfram ECA) appear as the degenerate case:

```
Γ_t = Γ_grid  
δ = f_rule  
Q = id  
```

This repository contains:

- A formal reduction of CA → RDG–MFE–Q  
- A universality theorem (glider embedding)  
- Emergent geometry demos (RDG induces quasi‑2D grids)  
- Minimal Python implementations  
- A Maxwell–Quaternion appendix showing how MFE generalizes field dynamics  

---

## Highlights

### ✔ Strict containment  
RDG–MFE–Q strictly extends CA:

```
Classic CA ⊂ Graph CA ⊂ Async CA ⊂ Constrained CA ⊂ RDG–MFE–Q
```

### ✔ Universality preserved  
Life’s glider orbit `{g0,g1,g2,g3}` embeds as an admissible RDG–MFE–Q trajectory when:

```
Q(gk) = gk   for k = 0..3
```

### ✔ Emergent manifolds  
RDG induces quasi‑2D grids from random graphs, enabling Life‑like attractors.

### ✔ Minimal working code  
Includes:

- exact Life specialization  
- RDG‑perturbed geometry with Q‑preserved glider  
- coherence metrics (degree variance, cycle ratios)

---

## License

MIT or Apache‑2.0 recommended.
