# Density-Dependent Spectral Distortion in Extreme Dense Environments

**Evidence from 260 High-Redshift Little Red Dots**

Xin Tan — Independent Researcher, IAIP

[![MNRAS Submission](https://img.shields.io/badge/MNRAS-submitted-blue)](https://academic.oup.com/mnras)
[![arXiv](https://img.shields.io/badge/arXiv-coming%20soon-green)](https://arxiv.org)
[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.19587085-blue)](https://doi.org/10.5281/zenodo.19587085)

---

## 📄 Paper

**"Density-Dependent Spectral Distortion in Extreme Dense Environments:
Evidence from 260 High-Redshift Little Red Dots"**

Submitted to *The Astrophysical Journal Letters* (APJL)

> **TL;DR:** We analyzed 260 JWST-observed Little Red Dots (LRDs) and found a **5.6σ correlation** between F444W/F150W color and bolometric surface density (Σ), even after controlling for redshift and luminosity. A control experiment (F444W/F356W) confirms the signal is specific to Balmer-jump-spanning colors. This Σ–color relation constitutes a previously unrecognized, SED-fitting-independent empirical constraint on LRD models.

📄 **[Read the paper](./paper/PAPER_DRAFT_EN.pdf)** |
📋 **[Outline](./paper/APJL_OUTLINE_v3.md)** |
📝 **[双语文档](./paper/PAPER_DRAFT_ZH.md)**

---

## 🗂️ Repository Structure

```
├── paper/
│   ├── PAPER_DRAFT_EN.tex      # LaTeX source (AASTeX 7.0)
│   ├── PAPER_DRAFT_EN.pdf      # Compiled PDF
│   ├── APJL_OUTLINE_v3.md      # Paper outline
│   ├── PAPER_DRAFT_ZH.md       # 中文说明
│   └── DUAL_PATH_ANALYSIS_REPORT.md
├── figures/
│   ├── Figure1_PubQuality_DensityFluxRatio.pdf  # Main result (4-panel)
│   └── Figure2_ConceptSketch_DensityDependentReddening.pdf
├── data/
│   └── Kokorev_LRDs_Full.csv   # Public LRD catalog (Kokorev et al. 2024)
├── code/
│   ├── pathA_flux_ratio_analysis.py   # Path A: Partial correlation
│   ├── pathB_free_zdist_fitting.py    # Path B: Free z_dist fitting
│   ├── Figure1_pubquality_pathA.py    # Plot: Figure 1
│   ├── Figure2_ConceptSketch.py       # Plot: Figure 2
│   └── LRD_Gravity_Simulator.html     # Interactive web simulator
└── latex/
    ├── aastex701.cls           # AASTeX 7.0 document class
    └── aasjournalv7.bst        # AASTeX bibliography style
```

---

## 🔬 Key Results

### Main Finding
| Metric | Value |
|--------|-------|
| Partial correlation (ρₚ) | +0.341 |
| Significance | **5.6σ** |
| KS statistic (D) | 0.574 |
| KS significance | **6.2σ** |
| Control experiment (F444W/F356W) | < 1σ (signal absent) |

### Robustness
- Outlier rejection: +0.332 (5.4σ) ✓
- Alt. mass proxy: +0.298 (4.8σ) ✓
- High-z subsample: +0.310 (4.2σ) ✓
- Exclude brightest 10%: +0.335 (5.5σ) ✓

---

## 💡 Physics Interpretation (Working Hypothesis)

The observed Σ–color correlation can be phenomenologically described as:

```
Δλ/λ|_excess ≡ z_eff(Σ) ∝ f(Σ) · (M / R · c²)
```

where deeper potential wells produce stronger intrinsic spectral shifts and more efficient dust retention. This is a **density-dependent effective correction** to gravitational redshift and/or dust geometry.

> ⚠️ **Speculative framework.** The core value lies in the empirical observation (Section 2), not the specific mechanism interpretation.

---

## 📦 Data & Software

- **LRD Catalog**: Kokorev et al. (2024), via [GitHub](https://github.com/Vlas-Sokolov/Kokorev-LRD-catalog)
- **Analysis code**: Python 3, NumPy, SciPy, Matplotlib, Pandas
- **LaTeX**: AASTeX 7.0 (`aastex701.cls`)

---

## 📚 Citation

```bibtex
@article{Tan2026LRD,
  author = {Xin Tan},
  title = {Density-Dependent Spectral Distortion in Extreme Dense Environments:
           Evidence from 260 High-Redshift Little Red Dots},
  journal = {The Astrophysical Journal Letters},
  year = {2026},
  note = {Submitted to APJL}
}
```

---

## 📦 Zenodo Archive

**DOI:** [10.5281/zenodo.19587085](https://doi.org/10.5281/zenodo.19587085)

This GitHub repository is archived on Zenodo to ensure a persistent, citable snapshot.

## 📜 License

This project is available for academic use. Please contact the author for permissions beyond academic citation.
