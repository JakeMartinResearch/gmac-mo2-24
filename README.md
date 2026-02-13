# The impact of isosmotic conditions on the metabolism and hypoxia tolerance of a purportedly oxyconforming teleost (gmac-mo2-24)  

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). You are free to reuse, redistribute, and adapt the material, provided appropriate credit is given.

------------------------------------------------------------------------

## 📄 Project Summary

-   **Title**: The impact of isosmotic conditions on the metabolism and hypoxia tolerance of a purportedly oxyconforming teleost
-   **Authors**: Timothy D. Clark^1^, Luis L. Kuchenmüller^1^, Elizabeth C. Hoots^1^, Maryane Gradito^1^, and Jake M. Martin^1,2^ <br>
-   **Institutions**:\
    ^1^ School of Life and Environmental Sciences, Deakin University, Geelong, VIC, Australia\
    ^2^ Department of Wildlife, Fish and Environmental Studies, Swedish University of Agricultural Sciences, Umeå, Sweden\

This project tests:\
1. Whether *G. maculatus* exhibits oxyregulation\
2. Whether isosmotic conditions reduce resting oxygen uptake and improve hypoxia tolerance

The study compares SMR, RMR, and estimated O2crit values across salinity treatments (0 ppt vs 9 ppt), using data collected from intermittent-flow respirometry and analysed in R (v4.2.3).

📍 [Browse the HTML output](https://jakemartinresearch.github.io/gmac-mo2-24/)

------------------------------------------------------------------------

## 📁 Repository Structure

```         
📁 gmac-mo2-24/
├── 📂 input-data/                 Raw and cleaned input data
├── 📂 mod-data/                   Intermediate summaries for modelling
├── 📂 output-fig/                 Final figures used in the manuscript
├── 📂 output-mod/                 Model outputs (.rds files)
├── 📄 gmac-labchart-24.Rmd        Main analysis and figure script
├── 📄 index.html                  R script for Git page 
├── 📄 supplementary-file-1.pdf    R script as supplementary file 1
└── 📄 EXP-2024-gmac-labchart.Rproj RStudio project file
```

------------------------------------------------------------------------

## 📦 R Dependencies

This project uses the following key R packages:

**🔹 Data Visualisation**\
- `ggthemes`\
- `bayesplot`\
- `gt`\
- `gtsummary`\
- `plotly`\
- `qqplotr`

**🔹 Tidy Data & Wrangling**\
- `tidyverse`\
- `janitor`\
- `readxl`\
- `broom.mixed`\
- `data.table`\
- `hms`\
- `devtools`\
- `mclust`

**🔹 Modelling & Statistical Analysis**\
- `brms`\
- `rstan`\
- `marginaleffects`\
- `performance`\
- `emmeans`\
- `tidybayes`\
- `respirometry`\
- `future`

These are installed and loaded in the `.Rmd` using `pacman::p_load(...)`.

------------------------------------------------------------------------

## 🔍 Key Methods

-   **SMR estimation**: Using a custom version of the `calcSMR` method (Chabot et al., 2016)

-   **Incremental regression**: Polynomial Bayesian models to describe ṀO₂--DO relationships (Urbina et al., 2012)

-   **Model comparison**: Leave-one-out cross-validation (LOO-CV) for evaluating best-fit regressions

-   **O₂crit detection**: Rule-based detection method (Claireaux & Chabot, 2016) paried with visual validation

------------------------------------------------------------------------

## 📊 Outputs

-   HTML-rendered results and figures are available at:\
    📍 <https://jakemartinresearch.github.io/gmac-mo2-24/>

-   Bayesian model outputs are saved as `.rds` files and stored in the `/output-mod/` folder.

-   For plots presented per individual fish, output figures are saved as `.PDF` in  `/output-fig/` folder.

------------------------------------------------------------------------

## 📥 Download or Pull This Repository into R

To work with this project in RStudio:

1.  Open RStudio → **File** → **New Project** → **Version Control** → **Git**

2.  Paste this URL in the **Repository URL** field:

```{=html}
<pre>https://github.com/JakeMartinResearch/gmac-mo2-24.git</pre>
```
3.  Choose a folder on your computer

4.  Click **Create Project**

RStudio will now pull the GitHub repo into a new local folder.

📺 [Watch this 2-min tutorial on YouTube](https://www.youtube.com/watch?v=HzTqHk4XjQQ)

------------------------------------------------------------------------

## 📥 Download from OSF

All data and code is also available on the Open Science Framework (OSF)

🌐 [Click here for the page](https://www.youtube.com/watch?v=HzTqHk4XjQQ)

This is the DOI **10.17605/OSF.IO/GFXCA** 

------------------------------------------------------------------------

## 📘 Sharing/accessing and citing

1.  **Licenses/restrictions placed on the data:** CC-BY 4.0

2.  **Link to the associated publication:**\
    🚧 ***To be added*** 🚧

3.  **Recommended citation for this data:**\

Clark, T. D., Kuchenmüller, L. L.,  Hoots, E. C., Gradito, M., & Martin, J. M. (2025, May 28). TThe role of osmorespiratory compromise in metabolism and hypoxia tolerance of a purportedly oxyconforming teleost. https://doi.org/10.17605/OSF.IO/GFXCA

------------------------------------------------------------------------

## 📩 Contact

**Jake M. Martin**

📧 **Email:** [jake.martin\@deakin.edu.au](mailto:jake.martin@deakin.edu.au)

📧 **Alt Email:** [jake.martin.research\@gmail.com](mailto:jake.martin.research@gmail.com)

🌐 **Web:** [jakemartin.org](https://jakemartin.org/)

🧪 **ORCID**: [0000-0001-9544-9094](https://orcid.org/0000-0001-9544-9094)

------------------------------------------------------------------------
