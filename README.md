# Social³ Source

Point-only LaTeX scaffold for the position paper, copied from
`Social3_Source_Paper_Brief.pdf` (23 September 2026).

`main.tex` contains the ten agreed sections and the detailed points mapped to
their corresponding sections, without elaboration. It uses the brief's first
candidate title as a working title, Jordi Cabot as the single author, and the
brief's definition as the abstract. The opening quotation is explicitly labeled
as an adaptation. Working proposals and unresolved questions retain the brief's
wording.

The 13 reference leads are stored in `references.bib`, using BibTeX's standard
`unsrt` style (numbered references in citation order). Their
metadata and claims have not been independently verified; the verification notes
from the brief are retained. This is a scaffold for further drafting, not a
finished submission.

Build with a standard LaTeX installation:

```sh
pdflatex -interaction=nonstopmode -halt-on-error main.tex
bibtex main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
```

The source uses standard packages and no custom styles or external figures.
Keep `main.tex` and `references.bib` together. All 13 reference leads are included,
including those not yet cited in a section, using `\nocite{*}`.

Compilation could not be checked in the current environment because system
policy blocks the installed `pdflatex` executable. No compiled PDF is included.
