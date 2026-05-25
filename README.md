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

## License

MIT or Apache‑2.0 recommended.
