# Grand Proof II — Publication Package (Grand Proof Series II)

> **Türkçe:** [README_TR.md](./README_TR.md)

**Grand Proof II: From Navier–Stokes Vortex Saturation to the 4D SU(3) Yang–Mills Mass-Gap Isomorphism and the Lattice QCD Glueball Spectrum**

Author: Fahri Meral · Date: October 19, 2026 · Version: v1 (Grand Proof II)

> **Status:** Unpublished preprint (v1). Not peer-reviewed.

## Contents

| File | Description |
|---|---|
| `paper/grand_proof_II_yang_mills_kutle_araligi.tex` | Main paper, Turkish (Tables 1–3, Figure 1 2×2) |
| `paper/grand_proof_II_yang_mills_mass_gap_EN.tex` | English version |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.pdf` | Tests T32–T34 figure (TR, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.png` | Tests T32–T34 figure preview (TR) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.pdf` | Tests T32–T34 figure (EN, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.png` | Tests T32–T34 figure preview (EN) |
| `CITATION.cff` | Citation record |
| `LICENSE` | CC BY 4.0 |

## Results (zero free parameters)

- Flux-tube operator (FV, p = 2.0000): λ₀^cont = 5.610204; numeric bridge
  √(2λ₀) = 3.349688 (1.23% from closed form); gap(0⁺⁺) = 3.3914463
  vs LQCD 3.405 ± 0.021 (0.40%, 0.65σ). OPEN RETRACTION: the GP-II/GP-II.1
  u-form λ₀ = 5.9158 was wrong (violated the variational bound 5.6468).
- Glueball spectrum 0⁺⁺/2⁺⁺/topological 0⁻⁺/0*⁺⁺ mean 1.56% (non-topological
  classic 4.8803 kept for comparison).
- γ_Meral = 0.29847153 vs Cornell 0.295 ± 0.010 (0.35σ); Yukawa-screened core
  (δγ = 0.16352706, Rc = 1.136364 GeV⁻¹): charmonium 596.89 MeV (1.31%),
  bottomonium 522.25 MeV (7.24%), both same-sided; C_F = 4/3 Casimir companion
  column: c-c̄ 602.92 (2.33%), b-b̄ 550.62 (2.19%).

## Numerical reproduction

Tests T32–T34 are produced with the solver in the **Paper V repository**
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py   # T1–T34 (34/34 PASS)
python duran_sicimler_sim/mini_check_gp2.py  # independent cross-check (15/15 PASS)
```

The independent cross-check never imports the solver.
Figure 1 is produced by the `fig14` function in `generate_figures.py`.
