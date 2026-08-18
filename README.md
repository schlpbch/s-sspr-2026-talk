# Orthogonality and Dimensionality in Airline Cluster Analysis using PCA and Kernel PCA

Talk for [S+SSPR 2026](https://sspr2026.github.io/) (IAPR Joint International
Workshops on Statistical Techniques in Pattern Recognition and Structural and
Syntactic Pattern Recognition), Bern, August 24–26, 2026.

**Paper:** [arXiv:2606.08322](https://arxiv.org/abs/2606.08322) — a copy is
included as `2606.08322v2.pdf`.

## Abstract of the talk

Kernel PCA is usually asked *which* kernel reveals a dataset's nonlinearity.
This talk asks the opposite question: how do you **certify that a dataset
contains none**? Auditing a published study of US airline profit cycles
(Renold et al., *J. Air Transport Management*, 2023), we show that the
seven collinear input variables span only ≈2.5 effective dimensions, that
cluster assignments are invariant between raw and PCA space (ARI = 1.0), and
that six kernels from three fundamentally different families — distance-based,
information-geometric, and graph-based — all agree with linear PCA. The
absence of nonlinear structure is itself the finding: a *linearity
certificate* that licenses every linear tool downstream.

## Building the slides

Requires TeX Live with LuaLaTeX (the talk loads the bundled IBM Plex Sans
fonts via `fontspec`).

```bash
cd talk
make          # builds talk.pdf
make clean    # removes auxiliary files
```

## Contents

- `talk/talk.tex` — the beamer source (16:9, LuaLaTeX)
- `talk/asc-theme.sty` — slide theme
- `talk/fonts/` — IBM Plex Sans (SIL Open Font License 1.1)
- `2606.08322v2.pdf` — the accompanying paper

## Author

Andreas Schlapbach — [asc.engineering](https://asc.engineering)

*The views expressed are the author's own and do not necessarily reflect the
views or policies of SBB.*
