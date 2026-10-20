# Stationary Strings XIII — Yayın Paketi

> **English:** [README.md](./README.md)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE)

**Stationary Strings XIII: Navier–Stokes Girdap Doyumundan 4B SU(3) Yang–Mills Kütle Aralığına İzomorfizm ve Lattice QCD Glueball Spektrumu**

Yazar: Fahri Meral · Tarih: 19 Ekim 2026 · Sürüm: v1 (Stationary Strings XIII)

> **Durum:** Yayımlanmamış ön-baskı (v1). Hakem denetiminden geçmemiştir. *[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23517479-blue.svg)](https://doi.org/10.5281/zenodo.23517479)*

## İçerik

| Dosya | Açıklama |
|---|---|
| `paper/stationary_strings_XIII_yang_mills_kutle_araligi.tex` | Ana makale, Türkçe (Tablo 1–3, Şekil 1 2×2) |
| `paper/stationary_strings_XIII_yang_mills_mass_gap_EN.tex` | İngilizce sürüm |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.pdf` | T32–T34 şekli (TR, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.png` | T32–T34 şekil önizlemesi (TR) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.pdf` | T32–T34 şekli (EN, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.png` | T32–T34 şekil önizlemesi (EN) |
| `CITATION.cff` | Atıf kaydı |
| `LICENSE` | CC BY 4.0 |

## Ana bulgular

- **T32 (Teorem XIII.1):** tekilliksiz akı-tüpü potansiyeli
  `V_eff(x) = (1+β₀²)/(x²+β₀²) + C_univ²(1+µ_s)x²` ile **analitik ve
  ızgaradan bağımsız** Temple–Kato çerçevelemesi
  `λ₀ ∈ [5,4806777821, 5,7674115648]` (sabit-`α`) ve
  `λ₀ ∈ [5,3686426884, 5,6467530803]` (optimize sınır); sonlu-hacim süreklilik
  limiti `λ₀^cont = 5,6102039939` (bağımsız shooting ile `5,6102039940`) her
  ikisinin de içindedir; Richardson mertebesi `p = 1,99995`. Kapalı-form aralık
  `Δm_gap/√σ = 3,3914463`, Lattice QCD `3,405 ± 0,021` ile %0,40 (0,65σ).
- **T33 (Teorem XIII.2):** `0^{++}`, `2^{++}`, topolojik `0^{-+}`, `0^{*++}`
  glueball spektrumu Lattice QCD ile ortalama %1,56 sapma; kiral giydirme ve
  topolojik çarpanlar *türetilmiş değil, ek model yorumu* olarak etiketlidir.
- **T34 (Teorem XIII.3):** `γ_Meral = (π/12)(1+4κ/5) = 0,29847153` Cornell
  katsayısı `0,295 ± 0,010` ile 0,35σ; Yukawa-perdelemeli çekirdek
  `δγ = µ_s/1,25` ile charmonium `2S−1S` 596,89 MeV (%1,31), bottomonium
  522,25 MeV (%7,24); `C_F = 4/3` Casimir sütunu 602,92 / 550,62 MeV.

## Sayısal yeniden-üretim

T32–T34 testleri **Makale V deposundaki** çözücüyle üretilir
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py     # T1–T34 (34/34 PASS)
python duran_sicimler_sim/mini_check_gp2.py    # bağımsız çapraz kontrol (17/17 PASS)
python duran_sicimler_sim/mini_check_audit.py # seri geneli denetim (9/9 PASS)
```

Bağımsız çapraz kontroller çözücüyü import etmez. Şekil 1,
`duran_sicimler_sim/generate_figures.py` içindeki `fig14` işleviyle üretilir.

## Atıf

```bibtex
@misc{meral2026grandproofii,
  author = {Fahri Meral},
  title  = {Stationary Strings XIII: Navier-Stokes Girdap Doyumundan 4B SU(3) Yang-Mills Kitle Araligina Izomorfizm ve Lattice QCD Glueball Spektrumu},
  year   = {2026},
  url    = {https://github.com/fahrim/stationary-strings-xiii},
  doi    = {10.5281/zenodo.23517479},
}
```

Ayrıca bkz. `CITATION.cff`.

## İlgili çalışmalar

- `stationary-strings-i` … `stationary-strings-x` — Teoremler I–X (ana seri).
- `stationary-strings-xii` — Karanlık-maddesiz galaktik dinamik, SPARC, EHT halkaları.
- `stationary-strings-xiv` — Masaüstü girdap PIV, Vela glitch, Na-22 pozitronyum.

## Lisans

CC BY 4.0 — bkz. `LICENSE`. İçerik hakem denetiminden geçmemiştir.
