# Social³ Source

LaTeX source for the Social³ Source position paper, developed from
`Social3_Source_Paper_Brief.pdf` (23 September 2026).

`main.tex` defines the concept and its three social dimensions, illustrates them
with a hypothetical migrant-services application, proposes a model-based
development framework using BESSER, and discusses related work and a research
roadmap. Jordi Cabot is the single author. The introduction's quotation is
explicitly labeled as a paraphrase; proposed capabilities and evaluation needs
are distinguished from demonstrated results.

`references.bib` contains cited sources and retained reference leads from the
brief. Only cited sources appear in the paper, using BibTeX's standard `unsrt`
style (numbered references in citation order). The editorial pass checks citation
keys and cross-references; it does not independently verify bibliographic
metadata or source claims.

Build with a standard LaTeX installation:

```sh
pdflatex -interaction=nonstopmode -halt-on-error main.tex
bibtex main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

The source uses standard packages and figures stored in `figures/`.
Keep that directory alongside `main.tex` and `references.bib`.

Compilation could not be checked in the current environment because system
policy blocks the installed `pdflatex` executable. No compiled PDF is included.
