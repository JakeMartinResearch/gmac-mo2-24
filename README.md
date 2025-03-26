---
title: "gmac-mo2-24: Oxygen Consumption and Hypoxia Tolerance in Galaxias maculatus"
---

This repository contains R code and data used to analyse metabolic responses to salinity and hypoxia in the Common Galaxias (*Galaxias maculatus*), with a focus on estimating critical oxygen thresholds (Pcrit) and understanding patterns of oxyregulation.

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/). You are free to reuse, redistribute, and adapt the material, provided appropriate credit is given.

---

## 📄 Project Summary

- **Title**: *The role of osmorespiratory compromise in hypoxia tolerance of the purportedly oxyconforming teleost Galaxias maculatus*
- **Authors**: Timothy D. Clark^1^, Luis L. Kuchenmüller^1^, Elizabeth C. Hoots^1^, Maryane Gradito^1^, and Jake M. Martin^1,2^  <br>
- **Institutions**:  
  ^1^ School of Life and Environmental Sciences, Deakin University, Geelong, VIC, Australia  
  ^2^ School of Biological Sciences, Monash University, Clayton, VIC, Australia  
- **Status**: 🚧 Unpublished and ongoing 🚧  

This project tests:  
1. Whether *G. maculatus* exhibits oxyregulation  
2. Whether isosmotic conditions reduce resting oxygen uptake and improve hypoxia tolerance  

The study compares SMR, RMR, and estimated Pcrit values across salinity treatments (0 ppt vs 9 ppt), using data collected from intermittent-flow respirometry and analysed in R (v4.2.3).

📍 [Browse the HTML output](https://jakemartinresearch.github.io/gmac-mo2-24/)

---

## 📁 Repository Structure

```
📁 gmac-mo2-24/
├── 📂 input-data/           Raw and cleaned input data
├── 📂 mod-data/             Intermediate summaries for modelling
├── 📂 output-fig/           Final figures used in the manuscript
├── 📂 output-mod/           Model outputs (.rds files)
├── 📄 gmac-labchart-24.Rmd  Main analysis and figure script
├── 📄 index.html            Rendered HTML results
└── 📄 EXP-2024-gmac-labchart.Rproj  RStudio project file
```
---

## 📦 R Dependencies

This project uses the following key R packages:

**🔹 Data Visualisation**  
- `ggthemes`  
- `bayesplot`  
- `gt`  
- `gtsummary`  
- `plotly`  
- `qqplotr`  

**🔹 Tidy Data & Wrangling**  
- `tidyverse`  
- `janitor`  
- `readxl`  
- `broom.mixed`  
- `data.table`  
- `hms`  
- `devtools`  
- `mclust`  

**🔹 Modelling & Statistical Analysis**  
- `brms`  
- `rstan`  
- `marginaleffects`  
- `performance`  
- `emmeans`  
- `tidybayes`  
- `respirometry`  
- `future`  

These are installed and loaded in the `.Rmd` using `pacman::p_load(...)`.

---

## 🔍 Key Methods
  
- **SMR estimation**: Using a custom version of the `calcSMR` method (Chabot et al., 2016)

- **Incremental regression**: Polynomial Bayesian models to describe ṀO₂–DO relationships (Urbina et al., 2012) 

- **Pcrit detection**: Rule-based detection method with visual validation (Claireaux & Chabot, 2016)  

- **Model comparison**: Leave-one-out cross-validation (LOO-CV) for evaluating best-fit models  

---

## 📊 Outputs

- HTML-rendered results and figures are available at:  
  📍 [https://jakemartinresearch.github.io/gmac-mo2-24/](https://jakemartinresearch.github.io/gmac-mo2-24/)
  
- Bayesian model outputs are saved as `.rds` files and stored in the `/output-mod/` folder.

---

## 📥 Download or Pull This Repository into R

To work with this project in RStudio:  

1. Open RStudio → **File** → **New Project** → **Version Control** → **Git**  

2. Paste this URL in the **Repository URL** field:  

<pre>https://github.com/JakeMartinResearch/gmac-mo2-24.git</pre>

3. Choose a folder on your computer  

4. Click **Create Project**  

RStudio will now pull the GitHub repo into a new local folder.  

📺 [Watch this 2-min tutorial on YouTube](https://www.youtube.com/watch?v=HzTqHk4XjQQ)

---

## 📘 Citation
  
🚧 *To be added* 🚧

---

## 📩 Contact

**Jake M. Martin**
  
📧 **Email:** [jake.martin@deakin.edu.au](mailto:jake.martin@deakin.edu.au)  
  
📧 **Alt Email:** [jake.martin.research@gmail.com](mailto:jake.martin.research@gmail.com) 
  
🌐 **Web:** [jakemartin.org](https://jakemartin.org/)  
  
🧪 **ORCID**: [0000-0001-9544-9094](https://orcid.org/0000-0001-9544-9094)  

---
