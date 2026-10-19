# Grand Proof II — Yayın Paketi (Büyük Kanıt Serisi II)

> **English:** [README.md](./README.md)

**Grand Proof II: Navier–Stokes Girdap Doyumundan 4B SU(3) Yang–Mills Kütle Aralığına İzomorfizm ve Lattice QCD Glueball Spektrumu**

Yazar: Fahri Meral · Tarih: 19 Ekim 2026 · Sürüm: v1 (Grand Proof II)

> **Durum:** Yayımlanmamış ön-baskı (v1). Hakem denetiminden geçmemiştir.

## İçerik

| Dosya | Açıklama |
|---|---|
| `paper/grand_proof_II_yang_mills_kutle_araligi.tex` | Ana makale, Türkçe (Tablo 1–3, Şekil 1 2×2) |
| `paper/grand_proof_II_yang_mills_mass_gap_EN.tex` | İngilizce sürüm |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.pdf` | T32–T34 şekli (TR, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement.png` | T32–T34 şekil önizlemesi (TR) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.pdf` | T32–T34 şekli (EN, 2×2) |
| `figs/fig14_yang_mills_mass_gap_glueballs_and_confinement_en.png` | T32–T34 şekil önizlemesi (EN) |
| `CITATION.cff` | Atıf kaydı |
| `LICENSE` | CC BY 4.0 |

## Sonuçlar (sıfır serbest parametre)

- Akı-tüpü operatörü (FV, p = 2,0000): λ₀^cont = 5,610204; sayısal köprü
  √(2λ₀) = 3,349688 (kapalı-formla %1,23); aralık(0⁺⁺) = 3,3914463,
  LQCD 3,405 ± 0,021 ile %0,40 (0,65σ). AÇIK GERİ ÇEKME: GP-II/GP-II.1
  `u`-formu λ₀ = 5,9158 yanlıştı (varyasyonel sınır 5,6468 ihlali).
- Glueball spektrumu 0⁺⁺/2⁺⁺/topolojik 0⁻⁺/0*⁺⁺ ortalama %1,56 (topolojisiz
  klasik 4,8803 karşılaştırma için korunur).
- γ_Meral = 0,29847153, Cornell 0,295 ± 0,010 ile 0,35σ; Yukawa-perdelemeli
  çekirdek (δγ = 0,16352706, Rc = 1,136364 GeV⁻¹): charmonium 596,89 MeV (%1,31),
  bottomonium 522,25 MeV (%7,24), ikisi de aynı işaretli.

## Sayısal yeniden-üretim

T32–T34 testleri **Makale V deposundaki** çözücüyle üretilir
([`stationary-strings-v`](https://github.com/fahrim/stationary-strings-v)):

```bash
git clone https://github.com/fahrim/stationary-strings-v
pip install numpy scipy matplotlib
python duran_sicimler_sim/solver_engine.py   # T1–T34 (34/34 PASS)
python duran_sicimler_sim/mini_check_gp2.py  # bağımsız çapraz kontrol (15/15 PASS)
```

Bağımsız çapraz kontrol çözücüyü import etmez.
Şekil 1, `generate_figures.py` içindeki `fig14` işleviyle üretilir.
