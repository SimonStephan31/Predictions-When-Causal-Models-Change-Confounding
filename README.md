# Making Predictions When Causal Models Change – The Role of Confounding

Experiment materials, data, and analysis scripts for Stephan, Placì, & Waldmann (JEP:LMC).

## Contents

| Path | Content |
|---|---|
| `Exp1_Analysis.qmd` | Results of Experiment 1 and Figure 5 |
| `Exp2_Analysis.qmd` | Results of Experiment 2 and Figure 8 |
| `Exp3_Analysis.qmd` | Results of Experiment 3 and Figure 10 |
| `Appendix_FigureA1.qmd` | Figure A1 (normative predictions under generative and preventive confounding) |
| `*.html` | Rendered versions of the four scripts, including all output |
| `data/` | Raw data of Experiments 1–3 |
| `CODEBOOK.md` | Description of all variables in the data files |
| `figures/` | Figures 5, 8, 10, and A1 as written by the scripts |
| `experimental-materials/` | jsPsych code of Experiments 1–3 |

## Reproducing the results

The analyses were run in R 4.5.1. Required packages:

```r
install.packages(c("tidyverse", "afex", "emmeans", "lme4", "lmerTest", "pbkrtest",
                   "binom", "Hmisc", "ggpubr", "showtext"))
```

The rendered `.html` files can be opened in any browser without installing
anything. To reproduce the results yourself, render each script with Quarto
from the repository root, e.g. `quarto render Exp1_Analysis.qmd`, or open it
in RStudio and run all chunks.
Each script reads its data from `data/`, prints all statistics reported in
the manuscript, and saves the corresponding figure to `figures/`. The package
versions used are listed at the end of each rendered script (`sessionInfo()`).

The figures use the Google fonts Outfit and Cabin, which are downloaded when
the script runs. Without an internet connection the scripts fall back to the
default sans font; all statistics are unaffected.

## Experiment materials

The folder `experiment-materials/` contains the jsPsych (de Leeuw, Gilbert, &
Luchterhandt, 2023) code of all three experiments. The experiments can be
downloaded and run offline in a web browser. Open the .html file in a browser to start the experiment.
