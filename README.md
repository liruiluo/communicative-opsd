# COPD project page

Static page for the arXiv release of *Communicative On-Policy Distillation*.
It mirrors the CAMP-II project page (same `styles.css` / `script.js`) and uses
numbers from the paper itself.

## Files

- `index.html` — the page
- `styles.css`, `script.js` — shared visual system, unchanged from the CAMP-II site
- `assets/` — figures exported from the paper (`figures/*.png`) and `paper.pdf`
  (the arXiv build, main text only)

## Local preview

```sh
python3 -m http.server 8765
# then open http://127.0.0.1:8765/
```

## Publishing

1. Create a repository `communicative-opsd` under the account that hosts the
   CAMP-II page, and push the contents of this directory to its default branch.
2. Enable GitHub Pages for that repository (root of the default branch).
3. The page then lives at `https://liruiluo.github.io/communicative-opsd/`.
4. Update the paper's `\checkdata[Project website]{...}` line in
   `main_arxiv.tex` to that URL, rebuild, and re-upload to arXiv.

## Content policy

- Code is not released yet: the page says "Code will be released after the
  review period" and carries no repository link.
- Every number on the page comes from the current manuscript: Table 1
  (per-domain and averages), Table 2 (external transfer), the ablation figure,
  the reply-content figure, the adviser-access figure, and the case study.
- The author list follows the paper (no Pu Yao).
