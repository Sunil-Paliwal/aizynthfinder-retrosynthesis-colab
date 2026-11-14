# AiZynthFinder-Based Retrosynthesis Workflow

> ## This notebook has moved
>
> It now lives as **module 04** of
> **[AI-Enabled Drug Discovery and Synthesis](https://github.com/Sunil-Paliwal/ai-enabled-drug-discovery-and-synthesis)**, alongside three other
> modules: molecular interactions, structure validation and alerts, and
> bioisosteric replacement.
>
> **New home:** [`04_aizynthfinder_retrosynthesis`](https://github.com/Sunil-Paliwal/ai-enabled-drug-discovery-and-synthesis/tree/main/04_aizynthfinder_retrosynthesis)
>
> This repository is no longer updated. The notebook here is kept only so that
> existing links do not break. Please use the link above.

---

**Dr. Sunil Paliwal**
Department of Chemistry and Chemical Biology
Stevens Institute of Technology

---

## What the maintained module adds

The copy in this repository is superseded. Module 04 adds:

- **Reaction names on every step of a route.** The public AiZynthFinder release
  ships its templates with the classification field empty, so routes come back
  as unlabelled arrows. The module classifies each step and prints the name.
- **A PDF report** of the chosen routes, with structures, step labels and the
  catalogue each starting material was found in.
- **ChemDraw-ready export** — routes as `.cdxml` reaction schemes, with arrows
  and labels, that open as editable reactions rather than flat pictures.
- **A student worksheet** built around the module.
- **Per-catalogue stock reporting**, and a companion notebook for building your
  own stock file from a supplier catalogue.

Setup instructions, troubleshooting and the Colab launch link are kept current
in the module's own README.

## Citing this work

Please cite the curriculum repository rather than this one:

> Paliwal, S. *AI-Enabled Drug Discovery and Synthesis.* GitHub, 2026.
> https://github.com/Sunil-Paliwal/ai-enabled-drug-discovery-and-synthesis

See `CITATION.cff` in that repository for the current version and DOI.

---

## Attribution and licensing

This work builds on the open-source **AiZynthFinder** software, which uses a
Monte Carlo tree search and a neural network policy to break molecules down
into purchasable precursors.

- **Software licence:** AiZynthFinder is distributed under the MIT Licence.
- **Article licence:** the original article is licensed CC BY 4.0.
- **Data waiver:** the data from the original article is provided under the
  Creative Commons Public Domain Dedication waiver.

Modifications were made to adapt the original workflow to Google Colab.

## Reference

Genheden, S.; Thakkar, A.; Chadimová, V. et al. AiZynthFinder: a fast, robust
and flexible open-source software for retrosynthetic planning. *J. Cheminform.*
**2020**, *12*, 70. <https://doi.org/10.1186/s13321-020-00472-1>
