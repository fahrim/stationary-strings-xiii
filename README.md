# Stationary Strings XIII — Publication Package

> **Türkçe:** [README_TR.md](./README_TR.md)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)

**Stationary Strings XIII: From Navier–Stokes Vortex Saturation to the 4D SU(3) Yang–Mills Mass-Gap Isomorphism and the Lattice QCD Glueball Spectrum**

Author: Fahri Meral · Date: October 19, 2026 · Version: v1 (Stationary Strings XIII)

> **Status:** Unpublished preprint (v1). Not peer-reviewed. *[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23517479-blue.svg)](https://doi.org/10.5281/zenodo.23517479)*

## Contents

| File | Description |
|---|---|
| `paper/stationary_strings_XIII_yang_mills_kutle_araligi.tex` | Main paper, Turkish (Tables 1–3, Figure 1 2×2) |
| `paper/stationary_strings_XIII_yang_mills_mass_gap_EN.tex` | English version |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.pdf` | Tests T32–T34 figure (TR, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.png` | Tests T32–T34 figure preview (TR) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.pdf` | Tests T32–T34 figure (EN, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.png` | Tests T32–T34 figure preview (EN) |
| `CITATION.cff` | Citation record |
| `LICENSE` | CC BY 4.0 |

## Key findings

- **T32 (Theorem XIII.1):** nonsingular flux-tube potential
  `V_eff(x) = (1+β₀²)/(x²+β₀²) + C_univ²(1+µ_s)x²` with the **analytic,
  grid-independent** Temple–Kato enclosure
  `λ₀ ∈ [5.4806777821, 5.7674115648]` (fixed-`α`) and
  `λ₀ ∈ [5.3686426884, 5.6467530803]` (optimized bound); the finite-volume
  continuum limit `λ₀^cont = 5.6102039939` (independently confirmed by
  shooting: `5.6102039940`) lies inside both, with Richardson order
  `p = 1.99995`. The closed-form gap `Δm_gap/√σ = 3.3914463` differs from
  Lattice QCD `3.405 ± 0.021` by 0.40 % (0.65 σ).
- **T33 (Theorem XIII.2):** glueball spectrum `0^{++}`, `2^{++}`, topological
  `0^{-+}`, `0^{*++}` with 1.56 % mean deviation from Lattice QCD; the
  chiral-dressing and topological factors are labelled *extra model
  interpretations*, not derived relations.
- **T34 (Theorem XIII.3):** `γ_Meral = (π/12)(1+4κ/5) = 0.29847153` versus
  the Cornell coefficient `0.295 ± 0.010` (0.35 σ); with the Yukawa-screened
  core `δγ = µ_s/1.25` the charmonium `2S−1S` splitting is 596.89 MeV
  (1.31 %) and the bottomonium 522.25 MeV (7.24 %); the `C_F = 4/3` Casimir
  column gives 602.92 / 550.62 MeV.

## Numerical reproduction

Tests T32–T34 are produced with the solver in the **Paper V repository**
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py     # T1–T34 (34/34 PASS)
python duran_sicimler_sim/mini_check_gp2.py    # independent cross-check (17/17 PASS)
python duran_sicimler_sim/mini_check_audit.py # series-wide audit (9/9 PASS)
```

The independent cross-checks never import the solver. Figure 1 is produced by
the `fig14` function in `duran_sicimler_sim/generate_figures.py`.

## Citation

```bibtex
@misc{meral2026grandproofii,
  author = {Fahri Meral},
  title  = {Stationary Strings XIII: From Navier-Stokes Vortex Saturation to the 4D SU(3) Yang-Mills Mass-Gap Isomorphism and the Lattice QCD Glueball Spectrum},
  year   = {2026},
  url    = {https://github.com/fahrim/stationary-strings-xiii}
  doi    = {10.5281/zenodo.23517479},
}
```

See also `CITATION.cff`.

## Related work

- `stationary-strings-i` … `stationary-strings-x` — Theorems I–X (the parent series).
- `stationary-strings-xii` — Dark-matter-free galactic dynamics, SPARC, EHT rings.
- `stationary-strings-xiv` — Benchtop vortex PIV, Vela glitches, Na-22 positronium.

## License

CC BY 4.0 — see `LICENSE`. Content is not peer-reviewed.
