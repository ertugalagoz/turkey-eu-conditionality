# Conditionality and Its Limits

**EU accession and democratic change in Turkey, 1990-2025**

A short reproducible analysis of Turkey's democratic trajectory across the EU accession
process, using the Varieties of Democracy indices.

📄 **[Read the analysis](https://KULLANICI-ADIN.github.io/DEPO-ADI/)**

## Summary

Turkey's electoral democracy score rises from the 1999 Helsinki European Council, peaks in
2004 when the Council decided that accession negotiations would open, and falls from the
moment negotiations actually began in October 2005. Estimating the structural breaks rather
than imposing them places the single sharpest break in 2007, immediately after eight
negotiating chapters were suspended in December 2006. The liberal components of democracy,
which EU conditionality addressed most directly, fell proportionally twice as far as the
electoral components.

The comparative section argues that the post-communist candidate countries cannot carry the
weight usually placed on them, since their democratic levels were established in 1989 rather
than by anything the Union did afterwards. Croatia is the exception, and the comparison rests
on it.

## Reproducing the analysis

Requires R (4.1 or later) and Quarto, which ships with recent versions of RStudio.

```r
install.packages(c("tidyverse", "strucchange", "modelsummary", "remotes"))
remotes::install_github("vdeminstitute/vdemdata")
```

Then render the document, either with the Render button in RStudio or from a terminal:

```
quarto render index.qmd
```

The V-Dem data is loaded directly from the `vdemdata` package, so nothing needs to be
downloaded separately. The analysis uses version 16 of the dataset.

## Files

| File | Contents |
| --- | --- |
| `index.qmd` | Source document: prose and analysis code |
| `index.html` | Rendered output, served by GitHub Pages |
| `references.bib` | Bibliography |

## Data

Coppedge, Michael, John Gerring, Carl Henrik Knutsen, Staffan I. Lindberg, Jan Teorell, et al.
2026. *V-Dem Country-Year Dataset v16*. Varieties of Democracy (V-Dem) Project.
<https://doi.org/10.23696/vdemds26>

## Author

Ertuğ Alagöz

## Licence

Text and figures are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Code is released under the MIT Licence.
