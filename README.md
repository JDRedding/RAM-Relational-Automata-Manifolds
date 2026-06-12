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

## Future Repository Structure

```
CA-Extensions-RDG-MFE-Q/
│
├── README.md
│   ├── Overview
│   ├── Classic CA → RDG–MFE–Q Reduction
│   ├── Why RDG–MFE–Q Strictly Generalizes CA
│   ├── Glider Embedding Theorem
│   ├── Emergent Geometry Demo
│   └── Maxwell–Quaternion Appendix
│
├── theory/
│   ├── RDG_MFE_Q_CA_Generalization.md
│   ├── Universality_Theorem.md
│   ├── Emergent_Manifolds.md
│   └── Maxwell_Quaternion_Appendix.md
│
├── rdg/                     # Geometry layer
│   ├── rdg_generators.md
│   ├── rdg_relations.md
│   └── rdg_examples.md
│
├── mfe/                     # Field-dynamics layer
│   ├── mfe_life.md
│   ├── mfe_maxwell.md
│   └── mfe_pde_extensions.md
│
├── q_layer/                 # Admissibility / SID / quotienting
│   ├── admissibility_axioms.md
│   ├── SID_stability.md
│   └── quotienting_rules.md
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
